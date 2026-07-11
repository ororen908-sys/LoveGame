<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="default">
<title>יש לי משהו להגיד לך 💌</title>
<link href="https://fonts.googleapis.com/css2?family=Heebo:wght@400;600;800;900&display=swap" rel="stylesheet">
<style>
  :root {
    --red: #ff4d6d;
    --red-dark: #e0416e;
    --pink: #ffc2d1;
    --pink-soft: #ffe4ea;
    --black: #1c1c1e;
    --white: #fffafb;
  }
  html { -webkit-text-size-adjust:100%; text-size-adjust:100%; }
  * { margin:0; padding:0; box-sizing:border-box; }
  body {
    font-family:'Heebo','Segoe UI',Arial,sans-serif;
    background: linear-gradient(160deg, #ffe9ec 0%, #ffd3dd 40%, #fff5f6 100%);
    color: var(--black);
    min-height:100vh;
    min-height:100dvh;
    /* רשת ביטחון ללפטופים נמוכים: אם כרטיס גבוה מהחלון — מגללים במקום לחתוך */
    overflow-x:hidden;
    overflow-y:auto;
    /* iOS Safari: מבטל הדגשת-הקשה כחולה, מונע בחירת טקסט בהקשות חוזרות, ומחליק גלילה */
    -webkit-tap-highlight-color: transparent;
    -webkit-user-select: none;
    user-select: none;
    -webkit-overflow-scrolling: touch;
    overscroll-behavior-y: none;
    /* מרווח בטוח לאזור ה-notch באייפון */
    padding: env(safe-area-inset-top) env(safe-area-inset-right) env(safe-area-inset-bottom) env(safe-area-inset-left);
  }

  /* ============ רקע לבבות מרחפים ============ */
  .bg-layer { position:fixed; inset:0; pointer-events:none; overflow:hidden; z-index:0; }
  .float-item {
    position:absolute; bottom:-12vh; opacity:0;
    animation: floatUp linear infinite;
    font-size:1.8rem;
    filter: drop-shadow(0 2px 6px rgba(255,77,109,.25));
  }
  @keyframes floatUp {
    0%   { transform:translateY(0) rotate(-5deg); opacity:0; }
    8%   { opacity:.85; }
    50%  { transform:translateY(-60vh) rotate(5deg); opacity:.85; }
    100% { transform:translateY(-125vh) rotate(-4deg); opacity:0; }
  }

  /* ============ מסכי המשחק ============ */
  .wrap {
    position:relative; z-index:2;
    min-height:100vh;      /* גיבוי לדפדפנים ישנים */
    min-height:100svh;     /* iOS Safari: גובה יציב שלא קופץ עם סרגלי הדפדפן */
    min-height:100dvh;
    display:flex; align-items:safe center; justify-content:center;
    padding:1.5rem 1rem;
  }
  .screen { display:none; width:min(94vw, 520px); }
  .screen.active { display:block; animation: pop .45s ease; }
  @keyframes pop { from { transform:scale(.86); opacity:0; } to { transform:scale(1); opacity:1; } }

  .game-card {
    background:rgba(255,255,255,.92);
    -webkit-backdrop-filter: blur(8px);
    backdrop-filter: blur(8px);
    border:2px solid var(--pink);
    border-radius:28px;
    box-shadow:0 20px 55px rgba(230,60,100,.28), inset 0 0 0 5px rgba(255,182,198,.22);
    padding:2.4rem 1.5rem 2.2rem;
    text-align:center;
  }
  .game-card .deco { font-size:1.3rem; letter-spacing:.35rem; margin-bottom:.6rem; }
  .game-card .q-num { color:#f06292; font-weight:600; font-size:.9rem; margin-bottom:.35rem; }
  .game-card h2 {
    color:#c2185b; font-weight:900;
    font-size:clamp(1.4rem, 5.5vw, 1.8rem);
    line-height:1.35; margin-bottom:1.4rem;
  }
  .row { display:flex; gap:.9rem; justify-content:center; flex-wrap:wrap; }

  .btn-yes, .btn-no {
    font-family:inherit; font-weight:800; font-size:1.1rem;
    border-radius:999px; padding:.8rem 2.1rem; cursor:pointer;
    transition: transform .15s ease, box-shadow .15s ease, left .15s ease, top .15s ease;
    /* בלי שבירת שורות — כפתור בורח עם טקסט ארוך שנשבר גדל בגובה וגולש מהמסך */
    white-space: nowrap;
    /* טלפון: מבטל השהיית דאבל-טאפ וזום על הקשה בכפתור */
    touch-action: manipulation;
    /* iOS Safari: איפוס עיצוב ברירת מחדל של הכפתור והדגשות הקשה */
    -webkit-appearance: none;
    appearance: none;
    -webkit-tap-highlight-color: transparent;
    -webkit-user-select: none;
    user-select: none;
  }
  .btn-yes {
    background:linear-gradient(135deg,#ff5c8a,var(--red-dark)); color:#fff;
    border:none;
    box-shadow:0 8px 20px rgba(224,65,110,.4);
    animation: heartbeat 1.4s ease-in-out infinite;
  }
  .btn-yes:hover { transform:scale(1.08); box-shadow:0 12px 28px rgba(224,65,110,.55); }
  .btn-no {
    background:#fff; color:var(--red-dark);
    border:2px solid var(--pink);
  }
  .btn-no:hover { transform:scale(1.06); }
  @keyframes heartbeat {
    0%,100% { transform:scale(1); }
    12% { transform:scale(1.06); }
    24% { transform:scale(1); }
    36% { transform:scale(1.04); }
    48% { transform:scale(1); }
  }

  /* הודעה שמופיעה על השאלה */
  .q-msg {
    min-height:2rem; margin-top:1.3rem;
    font-weight:900; font-size:1.25rem; color:var(--red-dark);
    opacity:0; transform:scale(.6);
    transition: opacity .3s ease, transform .3s ease;
  }
  .q-msg.show { opacity:1; transform:scale(1); animation: msgPop .4s ease; }
  @keyframes msgPop {
    0% { transform:scale(.4); }
    60% { transform:scale(1.15); }
    100% { transform:scale(1); }
  }

  /* ============ מסך המעטפה ============ */
  .final-caption {
    font-weight:900; color:#c2185b;
    font-size:clamp(1.5rem, 6vw, 2rem);
    line-height:1.4; margin-bottom:.6rem;
    animation: msgPop .6s ease;
  }
  .final-note {
    margin-top:1.2rem; font-weight:800; color:var(--red-dark); font-size:1.1rem;
    animation: heartbeat 1.6s ease-in-out infinite;
  }

  .envelope {
    position:relative;
    width:min(310px, 82%);
    height:200px;
    margin:1.4rem auto .4rem;
    cursor:pointer;
    animation: envFloat 2.6s ease-in-out infinite;
    transition: transform .2s ease;
  }
  .envelope:hover { animation-play-state:paused; transform:scale(1.05); }
  @keyframes envFloat {
    0%,100% { transform:translateY(0); }
    50% { transform:translateY(-8px); }
  }
  .env-back {
    position:absolute; inset:0;
    background:linear-gradient(170deg,#ff8fab,#ec5f8b);
    border-radius:12px;
    box-shadow:0 16px 38px rgba(224,65,110,.4);
  }
  .env-paper {
    position:absolute; left:6%; right:6%; top:9%; bottom:12%;
    background:linear-gradient(#fffdf8,#fff3ee);
    border-radius:7px;
    box-shadow:0 4px 14px rgba(120,30,60,.18);
    display:flex; align-items:center; justify-content:center;
    font-size:2.1rem;
    z-index:2;
    transition: transform .8s ease .45s;
  }
  .env-front {
    position:absolute; inset:0;
    background:linear-gradient(160deg,#ff9db6,#e75188);
    -webkit-clip-path: polygon(0 26%, 50% 64%, 100% 26%, 100% 100%, 0 100%);
    clip-path: polygon(0 26%, 50% 64%, 100% 26%, 100% 100%, 0 100%);
    border-radius:12px;
    z-index:3;
  }
  .env-flap {
    position:absolute; top:0; left:0; right:0; height:52%;
    background:linear-gradient(#f47a9e,#e0416e);
    -webkit-clip-path: polygon(0 0, 100% 0, 50% 100%);
    clip-path: polygon(0 0, 100% 0, 50% 100%);
    transform-origin: top center;
    transition: transform .6s ease;
    z-index:4;
  }
  .env-seal {
    position:absolute; top:44%; left:50%;
    transform:translateX(-50%);
    font-size:1.7rem; z-index:5;
    filter: drop-shadow(0 3px 6px rgba(120,10,40,.35));
    transition: opacity .35s ease;
  }
  .envelope.open { animation:none; cursor:default; }
  .envelope.open .env-flap { transform:rotateX(180deg); z-index:1; }
  .envelope.open .env-seal { opacity:0; }
  .envelope.open .env-paper { transform:translateY(-52%); }

  /* ============ מסך המכתב ============ */
  #letter { width:min(94vw, 560px); }
  .letter-card {
    background:linear-gradient(175deg,#fffdf8 0%, #fff4ef 70%, #ffeef2 100%);
    border:1.5px solid #f3c6d2;
    border-radius:20px;
    box-shadow:0 22px 55px rgba(230,60,100,.28);
    padding:2.4rem 2rem 2rem;
    text-align:center;
    animation: letterIn .8s ease;
    position:relative;
    overflow:hidden;
  }
  @keyframes letterIn {
    from { transform:translateY(46px) scale(.88); opacity:0; }
    to   { transform:translateY(0) scale(1); opacity:1; }
  }
  .letter-card::before {
    content:'💌';
    position:absolute; top:1rem; left:1.2rem;
    font-size:1.3rem; opacity:.55;
  }
  .letter-card::after {
    content:'🌹';
    position:absolute; bottom:1rem; right:1.2rem;
    font-size:1.3rem; opacity:.55;
  }
  .letter-head { font-size:2.2rem; margin-bottom:.4rem; animation: msgPop .8s ease; }
  .letter-title {
    font-weight:900; color:#c2185b;
    font-size:clamp(1.3rem, 5vw, 1.6rem);
    margin-bottom:1.2rem;
  }
  .letter-card p {
    color:#5c2333;
    font-size:1.04rem; font-weight:600;
    line-height:1.95;
    margin-bottom:1.05rem;
    text-align:right;
  }
  .letter-sign {
    margin-top:1.3rem;
    font-weight:900; color:var(--red-dark);
    font-size:clamp(1.25rem, 4.5vw, 1.5rem);
    animation: heartbeat 1.6s ease-in-out infinite;
  }

  /* ============ לבבות מתפוצצים ============ */
  .burst-heart {
    position:fixed; z-index:99; pointer-events:none;
    animation: burst 1.4s ease-out forwards;
    font-size:1.7rem;
  }
  @keyframes burst {
    0%   { transform:translate(0,0) scale(.4) rotate(0deg); opacity:1; }
    100% { transform:translate(var(--dx), var(--dy)) scale(1.4) rotate(var(--rot)); opacity:0; }
  }

  /* ============ התאמה למסכי לפטופ ============ */
  @media (max-height: 850px) {
    .screen { width:min(92vw, 450px); }
    .game-card { padding:1.7rem 1.2rem 1.5rem; border-radius:24px; }
    .game-card .deco { font-size:1.05rem; }
    .game-card h2 { font-size:clamp(1.15rem, 2.4vw, 1.4rem); margin-bottom:1rem; }
    .btn-yes, .btn-no { font-size:.98rem; padding:.65rem 1.7rem; }
    .q-msg { font-size:1.1rem; margin-top:1rem; min-height:1.6rem; }
    .final-caption { font-size:clamp(1.3rem, 3vw, 1.6rem); }
    .envelope { width:min(260px, 78%); height:168px; margin:1rem auto .3rem; }
    .final-note { font-size:1rem; margin-top:.9rem; }
    #letter { width:min(92vw, 540px); }
    .letter-card { padding:1.7rem 1.5rem 1.4rem; }
    .letter-card p { font-size:.95rem; line-height:1.8; margin-bottom:.85rem; }
    .letter-head { font-size:1.8rem; }
  }
  /* ============ התאמה לטלפון (מסך צר) ============ */
  @media (max-width: 480px) {
    .screen { width:94vw; }
    .game-card { padding:1.6rem 1rem 1.4rem; border-radius:22px; }
    .game-card h2 { font-size:clamp(1.2rem, 6vw, 1.45rem); margin-bottom:1rem; }
    .btn-yes, .btn-no { font-size:1rem; padding:.75rem 1.6rem; }
    .row { gap:.7rem; }
    .q-msg { font-size:1.05rem; }
    .envelope { height:170px; }
    .letter-card { padding:1.8rem 1.2rem 1.4rem; }
    .letter-card p { font-size:.97rem; line-height:1.85; }
  }
  /* מסכים נמוכים במיוחד (לפטופ עם סרגלים / זום) */
  @media (max-height: 620px) {
    .wrap { padding:.8rem 1rem; }
    .game-card { padding:1.1rem 1rem 1rem; }
    .game-card h2 { margin-bottom:.7rem; }
    .q-msg { margin-top:.7rem; }
    .envelope { width:210px; height:136px; margin:.7rem auto .2rem; }
    .env-paper { font-size:1.5rem; }
    .letter-card p { font-size:.88rem; line-height:1.7; margin-bottom:.7rem; }
    .letter-head { font-size:1.5rem; margin-bottom:.2rem; }
    .letter-title { margin-bottom:.7rem; }
  }
</style>
</head>
<body>

<div class="bg-layer" id="bg"></div>

<div class="wrap" id="gameWrap">

  <!-- פתיחה -->
  <div class="screen active" id="intro">
    <div class="game-card">
      <div class="deco">🤍💘🤍</div>
      <h2>היי אתה... 🥺<br>יש לי כמה שאלות אליך</h2>
      <div class="row">
        <button class="btn-yes" onclick="answer(event, 'q1')">בוא נתחיל 💘</button>
      </div>
    </div>
  </div>

  <!-- שאלה 1: אוהב אותי? — "לא" בורח -->
  <div class="screen" id="q1">
    <div class="game-card">
      <div class="deco">💘🌹💘</div>
      <div class="q-num">שאלה 1</div>
      <h2>האם אתה אוהב אותי?</h2>
      <div class="row">
        <button class="btn-yes" onclick="answerMsg(event, 'q1', 'msg1', 'q2')">כן 😍</button>
        <button class="btn-no" data-dodge>לא</button>
      </div>
      <div class="q-msg" id="msg1">ידעתי 🥰 גם אני אותך</div>
    </div>
  </div>

  <!-- שאלה 2: כועס עליי? — "כן" בורח -->
  <div class="screen" id="q2">
    <div class="game-card">
      <div class="deco">🥺💗🥺</div>
      <div class="q-num">שאלה 2</div>
      <h2>האם אתה כועס עליי?</h2>
      <div class="row">
        <button class="btn-yes" onclick="answerMsg(event, 'q2', 'msg2', 'q3')">ממש לא 🥰</button>
        <button class="btn-no" data-dodge>כן 😤</button>
      </div>
      <div class="q-msg" id="msg2">איזו הקלה 🥺 כי אי אפשר לכעוס עליי</div>
    </div>
  </div>

  <!-- שאלה 3: לראות אותי במוצש? — "לא יכול" בורח -->
  <div class="screen" id="q3">
    <div class="game-card">
      <div class="deco">🌙💫🌙</div>
      <div class="q-num">שאלה 3</div>
      <h2>אתה רוצה לראות אותי במוצש?</h2>
      <div class="row">
        <button class="btn-yes" onclick="answerMsg(event, 'q3', 'msg3', 'q4')">ברור 😍</button>
        <button class="btn-no" data-dodge>לא יכול 🙃</button>
      </div>
      <div class="q-msg" id="msg3">יש! כבר סופרת את השעות 🥰</div>
    </div>
  </div>

  <!-- שאלה 4: מיליון נשיקות — שתי תשובות מנצחות -->
  <div class="screen" id="q4">
    <div class="game-card">
      <div class="deco">💋😘💋</div>
      <div class="q-num">שאלה 4</div>
      <h2>אתה רוצה שאני אביא לך מיליון נשיקות?</h2>
      <div class="row">
        <button class="btn-yes" onclick="answerMsg(event, 'q4', 'msg4', 'q5')">כן 😘</button>
        <button class="btn-yes" onclick="answerMsg(event, 'q4', 'msg4', 'q5')">מיליון זה מעט 😏</button>
      </div>
      <div class="q-msg" id="msg4">תתכונן... מתחילה לספור 💋</div>
    </div>
  </div>

  <!-- שאלה 5: באלך שנשלים? — "לא" בורח -->
  <div class="screen" id="q5">
    <div class="game-card">
      <div class="deco">🤍🕊️🤍</div>
      <div class="q-num">שאלה אחרונה</div>
      <h2>באלך שנשלים?</h2>
      <div class="row">
        <button class="btn-yes" onclick="answerMsg(event, 'q5', 'msg5', 'final', 2600)">באלי 🫶</button>
        <button class="btn-no" data-dodge>לא</button>
      </div>
      <div class="q-msg" id="msg5">גם לי 🥺 בוא נשלים ❤️</div>
    </div>
  </div>

  <!-- מסך המעטפה — מכתב סגור שמחכה שיפתחו אותו -->
  <div class="screen" id="final">
    <div class="game-card">
      <div class="final-caption">אז השלמנו 🤍<br>ויש לי עוד משהו קטן בשבילך...</div>
      <div class="envelope" id="envelope" onclick="openEnvelope(event)">
        <div class="env-back"></div>
        <div class="env-paper">💌</div>
        <div class="env-front"></div>
        <div class="env-flap"></div>
        <div class="env-seal">❤️</div>
      </div>
      <div class="final-note">לחץ על המכתב כדי לפתוח אותו 💌</div>
    </div>
  </div>

  <!-- המכתב הפתוח -->
  <div class="screen" id="letter">
    <div class="letter-card">
      <div class="letter-head">💌</div>
      <div class="letter-title">מכתב בשבילך ❤️</div>
      <p>רציתי שתדע שגם אם יש בינינו רגעים פחות פשוטים, שום דבר לא משנה את מה שאני מרגישה כלפיך. אתה האדם שאני רוצה לצחוק איתו, להתווכח איתו, להשלים איתו ולבנות איתו את כל הזיכרונות הכי יפים.</p>
      <p>אתה נותן לי כוח, ביטחון ואהבה בדרך שרק אתה יודע. אני גאה בך, מעריכה אותך, ומודה על כל יום שאתה בחיים שלי.</p>
      <p>אני אוהבת אותך לא רק ברגעים הקלים, אלא גם ברגעים שבהם צריך לבחור אחד בשנייה מחדש. מבחינתי, אתה תמיד תהיה הבית שלי, המקום הבטוח שלי, והלב שלי.</p>
      <p>תודה שאתה אתה. אני אוהבת אותך יותר ממה שמילים יכולות לתאר.</p>
      <div class="letter-sign">אוהבת אותך ❤️</div>
    </div>
  </div>

</div>

<script>
/* ===================== רקע לבבות מרחפים ===================== */
const bg = document.getElementById('bg');
const emojis = ['💖','🌹','💘','🌸','❤️','🩷','💕','💗','🤍','🥀'];
for (let i = 0; i < 20; i++) {
  const s = document.createElement('span');
  s.className = 'float-item';
  s.textContent = emojis[i % emojis.length];
  s.style.left = Math.random() * 96 + 'vw';
  s.style.fontSize = (1.1 + Math.random() * 1.7) + 'rem';
  s.style.animationDuration = (9 + Math.random() * 10) + 's';
  s.style.animationDelay = (Math.random() * 13) + 's';
  bg.appendChild(s);
}

/* ===================== לבבות מתפוצצים ===================== */
function heartBurst(x, y, count = 18) {
  const hearts = ['💖','❤️','💕','💗','🩷','💘'];
  for (let i = 0; i < count; i++) {
    const h = document.createElement('span');
    h.className = 'burst-heart';
    h.textContent = hearts[Math.floor(Math.random() * hearts.length)];
    h.style.left = x + 'px';
    h.style.top = y + 'px';
    const ang = Math.random() * Math.PI * 2;
    const dist = 70 + Math.random() * 160;
    h.style.setProperty('--dx', Math.cos(ang) * dist + 'px');
    h.style.setProperty('--dy', (Math.sin(ang) * dist - 60) + 'px');
    h.style.setProperty('--rot', (Math.random() * 360 - 180) + 'deg');
    document.body.appendChild(h);
    setTimeout(() => h.remove(), 1500);
  }
}

/* ===================== מעבר בין מסכים ותשובות ===================== */
function show(id) {
  // מאפס כפתורים בורחים בכל החלפת מסך — שיופיעו תמיד במקומם הטבעי בכרטיס
  dodgeResets.forEach(fn => fn());
  document.querySelectorAll('.screen').forEach(s => s.classList.toggle('active', s.id === id));
}
function answer(e, nextId) {
  heartBurst(e.clientX || innerWidth / 2, e.clientY || innerHeight / 2, 14);
  show(nextId);
}
/* תשובה שמציגה הודעה קופצת ואז ממשיכה למסך הבא */
function answerMsg(e, screenId, msgId, nextId, delay = 2400) {
  heartBurst(e.clientX, e.clientY, 12);
  document.querySelectorAll('#' + screenId + ' button').forEach(b => b.disabled = true);
  document.getElementById(msgId).classList.add('show');
  setTimeout(() => show(nextId), delay);
}

/* ===================== כפתורים בורחים ===================== */
const dodgeResets = [];
document.querySelectorAll('[data-dodge]').forEach(btn => {
  let lastDodge = 0, ghost = null;
  dodgeResets.push(() => {
    // מחזיר את הכפתור למקומו המקורי בכרטיס
    if (ghost) { ghost.parentNode.insertBefore(btn, ghost); ghost.remove(); ghost = null; }
    btn.style.cssText = '';
    lastDodge = 0;
  });
  const dodge = e => {
    e.preventDefault();
    const now = Date.now();
    if (now - lastDodge < 300) return;
    lastDodge = now;
    if (btn.style.position !== 'fixed') {
      // מבטל אנימציות לפני המדידה כדי שהמיקום ההתחלתי יהיה מדויק
      btn.style.animation = 'none';
      const r = btn.getBoundingClientRect();
      // משאיר חור בגודל הכפתור כדי שהשורה לא תקפוץ
      ghost = document.createElement('span');
      ghost.style.display = 'inline-block';
      ghost.style.width = r.width + 'px';
      ghost.style.height = r.height + 'px';
      btn.parentNode.insertBefore(ghost, btn);
      btn.style.left = r.left + 'px';
      btn.style.top = r.top + 'px';
      btn.style.position = 'fixed';
      btn.style.zIndex = 50;
      btn.style.transition = 'left .3s ease, top .3s ease';
      // חובה: מוציאים את הכפתור מהכרטיס — backdrop-filter/transform על הכרטיס הופכים אותו
      // לעוגן של position:fixed, ואז הקואורדינטות (שמחושבות ביחס למסך) זורקות את הכפתור החוצה
      document.body.appendChild(btn);
    }
    // כלל קבוע: הכפתור לעולם לא עוזב את המסך — קופץ למקום אקראי חדש, כולו בתוך הגבולות.
    // בלי סיבוב (transform מגדיל את תיבת הגבולות) — offsetWidth/offsetHeight נותנים מדידה מדויקת.
    const bw = btn.offsetWidth, bh = btn.offsetHeight;
    const pad = 16;
    const maxX = Math.max(pad, innerWidth - bw - pad);
    const maxY = Math.max(pad, innerHeight - bh - pad);
    // מגריל נקודה בכל שטח המסך, ומוודא שהיא רחוקה מהעכבר כדי שלא ייתפס מיד
    let x = pad, y = pad;
    for (let i = 0; i < 25; i++) {
      x = pad + Math.random() * (maxX - pad);
      y = pad + Math.random() * (maxY - pad);
      if (Math.hypot(x + bw / 2 - e.clientX, y + bh / 2 - e.clientY) > 220) break;
    }
    btn.style.left = x + 'px';
    btn.style.top = y + 'px';
  };
  btn.addEventListener('pointerenter', dodge);
  btn.addEventListener('pointermove', dodge);
  btn.addEventListener('pointerdown', dodge);
  btn.addEventListener('click', e => { e.preventDefault(); dodge(e); });
});

/* אם גודל החלון משתנה בזמן שהכפתור ברח — מחזירים אותו לתוך המסך */
window.addEventListener('resize', () => {
  document.querySelectorAll('[data-dodge]').forEach(btn => {
    if (btn.style.position !== 'fixed') return;
    const pad = 16;
    const x = Math.min(Math.max(parseFloat(btn.style.left) || pad, pad), Math.max(pad, innerWidth - btn.offsetWidth - pad));
    const y = Math.min(Math.max(parseFloat(btn.style.top) || pad, pad), Math.max(pad, innerHeight - btn.offsetHeight - pad));
    btn.style.left = x + 'px';
    btn.style.top = y + 'px';
  });
});

/* ===================== פתיחת המעטפה ===================== */
let envelopeOpened = false;
function openEnvelope(e) {
  if (envelopeOpened) return;
  envelopeOpened = true;
  const env = document.getElementById('envelope');
  env.classList.add('open');
  const r = env.getBoundingClientRect();
  heartBurst(r.left + r.width / 2, r.top + r.height / 2, 20);
  // נותנים לאנימציית הפתיחה להסתיים ואז מציגים את המכתב המלא
  setTimeout(() => {
    show('letter');
    heartBurst(innerWidth / 2, innerHeight / 3, 14);
  }, 1600);
}
</script>
</body>
</html>
