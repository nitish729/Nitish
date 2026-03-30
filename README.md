# Nitish
Student 
<!doctype html>

<html lang="hi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Simple Landing — आपकी वेबसाइट</title>
  <meta name="description" content="A clean, responsive single-file website (Hindi)." />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724; /* dark navy */
      --card:#0b1320;
      --accent:#06b6d4;
      --muted:#94a3b8;
      --glass: rgba(255,255,255,0.03);
      --radius:14px;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background:linear-gradient(180deg,#071021 0%, #071827 60%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.4;
      padding:24px;
    }
    .container{max-width:1100px;margin:0 auto}
    header{display:flex;align-items:center;justify-content:space-between;padding:12px 0}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:700}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:500}
    nav a:hover{color:var(--accent)}.hero{
  display:grid;grid-template-columns:1fr;gap:22px;padding:36px 0;align-items:center
}
.hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);border-radius:16px;padding:28px;box-shadow:0 8px 30px rgba(2,6,23,0.6)}
h1{font-size:clamp(24px,4vw,40px);margin:0 0 8px}
p.lead{color:var(--muted);margin:0 0 18px}

.cta{display:inline-block;background:linear-gradient(90deg,var(--accent),#7c3aed);padding:10px 16px;border-radius:12px;color:#021024;font-weight:700;text-decoration:none}
.secondary{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:9px 14px;border-radius:12px;color:var(--muted);margin-left:10px}

.features{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:16px;margin-top:20px}
.feature{background:var(--glass);padding:16px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
.feature h3{margin:6px 0 4px}
.feature p{margin:0;color:var(--muted);font-size:14px}

.screenshot{width:100%;height:220px;border-radius:12px;background:linear-gradient(90deg,#041826,#07202a);display:flex;align-items:center;justify-content:center;color:#6ee7b7;font-weight:600;letter-spacing:0.6px}

.contact{margin-top:26px;background:var(--card);padding:18px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
form{display:flex;flex-direction:column;gap:10px}
input,textarea{background:transparent;border:1px solid rgba(255,255,255,0.06);padding:12px;border-radius:10px;color:inherit;font-size:14px}
input::placeholder,textarea::placeholder{color:rgba(255,255,255,0.25)}
button{padding:10px 14px;border-radius:10px;border:none;font-weight:700;background:var(--accent);cursor:pointer}

footer{margin-top:28px;color:var(--muted);font-size:13px;text-align:center}

/* Responsive layout for large screens */
@media(min-width:880px){
  .hero{grid-template-columns:1fr 420px}
  .screenshot{height:320px}
}

/* Small UI niceties */
.pill{background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:999px;font-size:13px;color:var(--muted)}
.grid-row{display:flex;gap:12px;flex-wrap:wrap}

/* subtle fade-in */
.fade-in{animation:fadeUp .6s ease both}
@keyframes fadeUp{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}

  </style>
</head>
<body>
  <div class="container">
    <header class="fade-in">
      <div class="brand">
        <div class="logo">GPT</div>
        <div>
          <div style="font-weight:700">Aapki Website</div>
          <div style="font-size:12px;color:var(--muted)">Simple • Tez • Responsive</div>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#features">Features</a>
        <a href="#contact">Contact</a>
      </nav>
    </header><main>
  <section class="hero">
    <div class="hero-card fade-in">
      <div class="pill">Free single-file template</div>
      <h1>Ek modern, responsive website — turant tayaar</h1>
      <p class="lead">Yeh template aapke chhote business, portfolio, ya personal project ke liye banaaya gaya hai. Simple, tez aur mobile-friendly design.</p>
      <div style="margin-top:14px">
        <a class="cta" href="#contact">Contact Karein</a>
        <a class="secondary" href="#features">Features dekhain</a>
      </div>

      <div class="features" style="margin-top:18px">
        <div class="feature">
          <div style="font-size:20px">🚀</div>
          <h3>Fast & lightweight</h3>
          <p>Sirf ek HTML file, koi heavy library nahi. Jaldi load hota hai.</p>
        </div>
        <div class="feature">
          <div style="font-size:20px">📱</div>
          <h3>Mobile-friendly</h3>
          <p>Responsive layout — phone se bhi acha dikhega.</p>
        </div>
        <div class="feature">
          <div style="font-size:20px">✏️</div>
          <h3>Asaan customization</h3>
          <p>Colors, text aur sections aap apne hisaab se badal sakte hain.</p>
        </div>
      </div>
    </div>

    <aside class="fade-in">
      <div class="screenshot">Preview: Aapka content yahin dalein</div>
      <div class="contact" id="contact" style="margin-top:12px">
        <strong>Contact form</strong>
        <form onsubmit="sendDemo(event)">
          <input type="text" id="name" placeholder="Naam" required />
          <input type="email" id="email" placeholder="Email" required />
          <textarea id="message" rows="4" placeholder="Sandesh" required></textarea>
          <div style="display:flex;gap:8px">
            <button type="submit">Bhejein</button>
            <a class="secondary" href="mailto:you@example.com">Email karen</a>
          </div>
        </form>
      </div>
    </aside>
  </section>

  <section id="features" style="margin-top:18px">
    <div class="hero-card fade-in">
      <h2>Features</h2>
      <div class="grid-row" style="margin-top:12px">
        <div style="min-width:220px;flex:1">
          <h3>Custom sections</h3>
          <p class="lead" style="margin-top:6px;color:var(--muted)">Aap 'About', 'Services', 'Portfolio' waale sections aasani se add kar sakte hain.</p>
        </div>
        <div style="min-width:220px;flex:1">
          <h3>Easy edits</h3>
          <p class="lead" style="margin-top:6px;color:var(--muted)">HTML aur CSS seedhe edit karke aap layout aur colors change kar sakte hain.</p>
        </div>
        <div style="min-width:220px;flex:1">
          <h3>Deploy fast</h3>
          <p class="lead" style="margin-top:6px;color:var(--muted)">GitHub Pages, Netlify, ya Vercel pe seedha upload kijiye.</p>
        </div>
      </div>
    </div>
  </section>

</main>

<footer>
  © "Aapki Website" — Template by GPT • Customize kariye aur bataiye agar aur help chahiye.
</footer>

  </div>  <script>
    function sendDemo(e){
      e.preventDefault();
      const name = document.getElementById('name').value;
      const email = document.getElementById('email').value;
      const message = document.getElementById('message').value;
      // This demo does not send to a server. Show a friendly message instead.
      alert('Dhanyavaad, ' + name + '! Aapka sandesh prapt hua. (Demo)');
      // Clear form
      e.target.reset();
    }
  </script></body>
</html>
