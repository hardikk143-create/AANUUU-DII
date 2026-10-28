<!DOCTYPE html><html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#100810">
<title>For Aanu Dii | Happy Birthday</title><style>
:root {
    --bg: #100810;
    --rose: #f3c0d0;
    --gold: #e8c58c;
    --muted: #dfcedb;
    --glass: rgba(255,255,255,.055);
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html { scroll-behavior: smooth; }

body {
    background: var(--bg);
    color: #fff5f7;
    font-family: Georgia, serif;
    overflow-x: hidden;
}

body::before {
    content: "";
    position: fixed;
    inset: 0;
    z-index: -2;
    background:
        radial-gradient(ellipse at 15% 5%, #57213c, transparent 42%),
        radial-gradient(ellipse at 90% 50%, #342043, transparent 45%),
        radial-gradient(ellipse at 50% 100%, #40172e, transparent 45%);
}

#particles {
    position: fixed;
    inset: 0;
    pointer-events: none;
    z-index: -1;
    overflow: hidden;
}

.particle {
    position: absolute;
    color: var(--gold);
    animation: float 7s infinite ease-in-out;
    opacity: .55;
}

@keyframes float {
    0%,100% { transform: translateY(0) rotate(0); }
    50% { transform: translateY(-35px) rotate(25deg); }
}

nav {
    position: relative;
    z-index: 5;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 12px;
    padding: 20px 6%;
    border-bottom: 1px solid #ffffff0b;
    color: var(--gold);
    font: 10px Arial, sans-serif;
    letter-spacing: 2px;
}

nav span:last-child {
    color: #e8d4df;
    text-align: right;
}

.hero {
    min-height: 92vh;
    padding: 70px 22px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}

.eyebrow, .label {
    color: var(--gold);
    font: 10px Arial, sans-serif;
    letter-spacing: 4px;
    text-transform: uppercase;
    line-height: 1.8;
}

h1 {
    margin: 25px 0;
    font-size: clamp(65px, 15vw, 115px);
    font-weight: 400;
    letter-spacing: -4px;
    line-height: .91;
    color: var(--rose);
    background: linear-gradient(120deg,#fff8f1,#efb4ca,#e8c58c);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.subtitle {
    color: #f2d0dd;
    font-size: clamp(18px,4vw,25px);
    font-style: italic;
}

.rule {
    width: 100px;
    height: 1px;
    margin: 28px auto;
    background: linear-gradient(90deg,transparent,var(--gold),transparent);
}

.description {
    max-width: 450px;
    margin: auto;
    color: var(--muted);
    font: 13px/2 Arial, sans-serif;
}

button {
    padding: 15px 22px;
    margin-top: 24px;
    border: 1px solid #e8c58c88;
    border-radius: 40px;
    background: linear-gradient(120deg,#633149,#38203b);
    color: #fff4f5;
    font: 11px Arial, sans-serif;
    letter-spacing: 1px;
    cursor: pointer;
    transition: .3s;
}

button:active { transform: scale(.96); }

section {
    width: min(900px,100%);
    margin: auto;
    padding: 65px 22px;
}

h2 {
    margin: 20px 0 32px;
    color: #f3d3df;
    text-align: center;
    font-size: clamp(34px,8vw,54px);
    font-weight: 400;
}

.label { text-align: center; }

.card {
    padding: clamp(25px,6vw,45px);
    border: 1px solid #e8c58c30;
    border-radius: 24px;
    background: linear-gradient(145deg,#ffffff10,#ffffff03);
    box-shadow: 0 25px 80px #0003;
    backdrop-filter: blur(12px);
}

.card p {
    margin-bottom: 20px;
    color: #e7d8e2;
    font: 14px/2 Arial, sans-serif;
}

.card p:last-child { margin-bottom: 0; }

.signature {
    color: var(--rose) !important;
    font-style: italic;
}

.grid {
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(190px,1fr));
    gap: 15px;
}

.box {
    padding: 27px 20px;
    text-align: center;
    border: 1px solid #e8c58c30;
    border-radius: 20px;
    background: var(--glass);
}

.box .icon { font-size: 30px; margin-bottom: 15px; }

.box h3 {
    margin-bottom: 10px;
    color: var(--rose);
    font-size: 20px;
    font-weight: 400;
}

.box p {
    color: var(--muted);
    font: 12px/1.8 Arial, sans-serif;
}

.gallery {
    display: grid;
    grid-template-columns: repeat(2,minmax(0,1fr));
    gap: 12px;
}

.photo {
    min-height: 165px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 12px;
    overflow: hidden;
    text-align: center;
    border: 1px dashed #e8c58c88;
    border-radius: 20px;
    background: #ffffff08;
    color: #e8c58c;
    font: 12px/1.8 Arial,sans-serif;
}

.photo img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 12px;
}

.photo span { padding: 10px 0; }

.gift-area { text-align: center; }

.gift {
    display: inline-block;
    margin: 20px 0;
    font-size: 100px;
    cursor: pointer;
    filter: drop-shadow(0 0 25px #f2a6c255);
    animation: giftPulse 2s infinite ease-in-out;
}

@keyframes giftPulse {
    0%,100% { transform: translateY(0) scale(1); }
    50% { transform: translateY(-8px) scale(1.06); }
}

#giftMessage, #secretMessage {
    display: none;
    margin-top: 25px;
    padding: 25px;
    border: 1px solid #e8c58c55;
    border-radius: 20px;
    background: #e8c58c0c;
    color: #ffe8f0;
    font: 14px/2 Arial,sans-serif;
    animation: appear .7s ease;
}

@keyframes appear {
    from { opacity: 0; transform: translateY(12px); }
    to { opacity: 1; transform: translateY(0); }
}

.music-note {
    display: inline-block;
    margin-right: 5px;
}

.final { text-align: center; }

.final p {
    color: var(--muted);
    font: 13px/2 Arial,sans-serif;
}

#musicStatus {
    margin-top: 12px;
    color: var(--gold);
    font: 11px Arial,sans-serif;
}

footer {
    padding: 30px 15px;
    text-align: center;
    border-top: 1px solid #ffffff10;
    color: #c0aaba;
    font: 10px/2 Arial,sans-serif;
    letter-spacing: 2px;
}

#confetti {
    position: fixed;
    inset: 0;
    overflow: hidden;
    z-index: 20;
    pointer-events: none;
}

.confetti-piece {
    position: absolute;
    top: -15px;
    width: 8px;
    height: 12px;
    animation: fall 3.5s linear forwards;
}

@keyframes fall {
    to { transform: translateY(110vh) rotate(720deg); opacity: .1; }
}

@media(max-width:420px) {
    nav { font-size: 8px; letter-spacing: 1px; }
    .gallery { grid-template-columns: 1fr 1fr; }
    .photo { min-height: 130px; }
}
</style></head><body><div id="particles"></div>
<div id="confetti"></div><nav>
    <span>✦ A LITTLE MAGIC ✦</span>
    <span>FOR AANU · 29 OCT</span>
</nav><header class="hero">
    <div>
        <div class="eyebrow">A special celebration for someone extraordinary</div>    <h1>Happy<br>Birthday</h1>

    <div class="subtitle">My Favourite Dii, Aanu ♡</div>

    <div class="rule"></div>

    <p class="description">
        For the one who stands by me through every problem,
        supports me when things get difficult, and will
        always hold a special place in my heart.
    </p>

    <button onclick="goTo('letter')">OPEN YOUR LETTER ↓</button>
    <br>
    <button onclick="celebrate()">🎉 LET'S CELEBRATE</button>
</div>

</header><section id="letter">
    <div class="label">A message from my heart</div>
    <h2>Dear Aanu Dii,</h2><div class="card">
    <p>
        ❤️ Happy Birthday to my favourite sister,
        my Aanu, and one of the most special people
        in my life!
    </p>

    <p>
        Thank you for always standing beside me whenever
        I face a problem. Thank you for supporting me,
        listening to me and making difficult days feel
        a little easier.
    </p>

    <p>
        Maybe I don't express it every day, but your
        support means more to me than words can explain.
        I'm genuinely lucky to have a sister like you.
    </p>

    <p>
        You're not just my sister. You're my supporter,
        my comfort person and my forever favourite Dii.
        No matter what happens in life, you'll always
        have a special place in my heart.
    </p>

    <p>
        I wish you endless happiness, success, beautiful
        memories, peaceful days and all the love you
        deserve. May your dreams come true, one by one.
    </p>

    <p class="signature">
        Love you always, Aanu Dii. ♡<br>
        You'll forever be my favourite sister.
    </p>
</div>

</section><section>
    <div class="label">Three things that make you special</div>
    <h2>My Favourite Dii</h2><div class="grid">
    <div class="box">
        <div class="icon">♡</div>
        <h3>Your Support</h3>
        <p>You're there for me when I need someone by my side.</p>
    </div>

    <div class="box">
        <div class="icon">✧</div>
        <h3>Your Heart</h3>
        <p>Your care and kindness make our bond truly special.</p>
    </div>

    <div class="box">
        <div class="icon">∞</div>
        <h3>Forever Us</h3>
        <p>No difficult day can change what you mean to me.</p>
    </div>
</div>

</section><section id="gallery">
    <div class="label">Beautiful moments</div>
    <h2>Our Little Memories</h2><div class="gallery">
    <div class="photo">
        <span>📸</span>
        <span>Our favourite memory</span>
    </div>

    <div class="photo">
        <span>🌸</span>
        <span>A moment to remember</span>
    </div>

    <div class="photo">
        <span>💗</span>
        <span>My favourite Dii</span>
    </div>

    <div class="photo">
        <span>✨</span>
        <span>Memories forever</span>
    </div>
</div>

<p style="text-align:center;font:12px/2 Arial,sans-serif;color:#cbb7c6;margin-top:15px">
    To add photos, see the instructions below the code.
</p>

</section><section class="gift-area" id="gift">
    <div class="label">Something special awaits</div>
    <h2>A Little Gift For You</h2><p style="font:13px/2 Arial,sans-serif;color:#dfcedb">
    Aanu Dii, tap the gift to open your surprise!
</p>

<div class="gift" onclick="openGift()" role="button" aria-label="Open birthday gift">
    🎁
</div>

<div id="giftMessage">
    💖 SURPRISE, AANU DII! 💖
    <br><br>
    You deserve all the happiness in this world.
    Thank you for always supporting me and being
    such an important part of my life.
    <br><br>
    Whatever life brings, I'll always be grateful
    that you're my sister.
    <br><br>
    HAPPY BIRTHDAY, MY FAVOURITE DII! 👑
</div>

</section><section>
    <div class="label">A secret just for you</div>
    <h2>Open When You Need A Smile</h2><div style="text-align:center">
    <button onclick="openSecret()">🔐 OPEN YOUR SECRET LETTER</button>
</div>

<div id="secretMessage">
    Dear Aanu,
    <br><br>
    If you're reading this, I want you to remember
    that you're loved, appreciated and important.
    You have supported me through my problems,
    and I'll always cherish the bond we share.
    <br><br>
    You don't have to be perfect to be amazing.
    Just keep being yourself, keep smiling, and
    never forget how much you mean to me.
    <br><br>
    You're my favourite Dii today, tomorrow
    and always. ❤️
</div>

</section><section class="final">
    <div class="label">One last birthday wish</div>
    <h2>Make a Wish, Aanu ✨</h2><p>
    May your future be brighter than every star,<br>
    your heart be lighter than every cloud,<br>
    and your life be filled with genuine happiness.
</p>

<button onclick="celebrate()">🎂 BIRTHDAY MAGIC</button>

<br>

<button onclick="shareWebsite()">📤 SHARE THIS WEBSITE</button>

<br>

<button onclick="toggleMusic()">
    <span class="music-note">♫</span> PLAY / PAUSE MUSIC
</button>

<p id="musicStatus">Music is off. Tap to play the birthday tune.</p>

</section><footer>
    MADE WITH ALL MY LOVE FOR AANU ♡<br>
    29 OCTOBER · FOREVER MY FAVOURITE DII
</footer><audio id="birthdayMusic" loop preload="none">
    <source src="https://cdn.pixabay.com/audio/2022/10/25/audio_946b2c4f1a.mp3" type="audio/mpeg">
</audio><script>
const particles = document.getElementById("particles");

for (let i = 0; i < 65; i++) {
    const p = document.createElement("span");

    p.className = "particle";
    p.textContent = ["✦", "✧", "·", "♡"][Math.floor(Math.random() * 4)];

    p.style.left = Math.random() * 100 + "%";
    p.style.top = Math.random() * 100 + "%";
    p.style.fontSize = (8 + Math.random() * 14) + "px";
    p.style.animationDelay = Math.random() * 5 + "s";
    p.style.animationDuration = (4 + Math.random() * 6) + "s";

    particles.appendChild(p);
}

function goTo(id) {
    document.getElementById(id).scrollIntoView({
        behavior: "smooth"
    });
}

function openGift() {
    const msg = document.getElementById("giftMessage");

    msg.style.display = "block";
    celebrate();

    msg.scrollIntoView({
        behavior: "smooth",
        block: "center"
    });
}

function openSecret() {
    const msg = document.getElementById("secretMessage");

    msg.style.display = msg.style.display === "block" ? "none" : "block";
}

function celebrate() {
    const area = document.getElementById("confetti");
    const colors = ["#f3c0d0", "#e8c58c", "#ffffff", "#cda7e8"];

    for (let i = 0; i < 110; i++) {
        const piece = document.createElement("div");

        piece.className = "confetti-piece";
        piece.style.left = Math.random() * 100 + "%";
        piece.style.background = colors[Math.floor(Math.random() * colors.length)];
        piece.style.animationDelay = Math.random() * 1.2 + "s";
        piece.style.animationDuration = (2.5 + Math.random() * 2) + "s";

        area.appendChild(piece);

        setTimeout(() => piece.remove(), 5000);
    }
}

async function toggleMusic() {
    const audio = document.getElementById("birthdayMusic");
    const status = document.getElementById("musicStatus");

    if (audio.paused) {
        try {
            await audio.play();
            status.textContent = "♫ Music is playing!";
        } catch (error) {
            status.textContent = "Music needs internet. Try again or use your own audio file.";
        }
    } else {
        audio.pause();
        status.textContent = "Music paused.";
    }
}

async function shareWebsite() {
    const data = {
        title: "Happy Birthday Aanu Dii",
        text: "A special birthday surprise for my favourite Dii! ❤️"
    };

    if (navigator.share) {
        try {
            await navigator.share(data);
        } catch (error) {
            // Sharing was cancelled.
        }
    } else {
        alert("To share this website as a link, publish it online first.");
    }
}
</script></body>
</html># AANUUU-DII
