<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Adi Desiging | Poster, Thumbnail & Website Design</title>
  <meta name="description" content="Adi Desiging creates posters, YouTube thumbnails and modern websites for local businesses, creators, coaching centers, cafes and shops." />
  <meta name="theme-color" content="#050816" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#050816;
      --bg2:#080b22;
      --card:rgba(255,255,255,.075);
      --card2:rgba(255,255,255,.11);
      --line:rgba(255,255,255,.14);
      --text:#eef6ff;
      --muted:#9fb0cc;
      --cyan:#17e7ff;
      --blue:#397cff;
      --pink:#ff2bd6;
      --yellow:#ffe45c;
      --green:#2bff88;
      --shadow: 0 24px 80px rgba(0,0,0,.42);
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      background:
        radial-gradient(circle at 20% 10%, rgba(57,124,255,.26), transparent 32%),
        radial-gradient(circle at 85% 20%, rgba(255,43,214,.19), transparent 30%),
        radial-gradient(circle at 50% 90%, rgba(23,231,255,.12), transparent 35%),
        linear-gradient(180deg, var(--bg), #02030b 70%);
      color:var(--text);
      font-family:Inter, system-ui, -apple-system, Segoe UI, sans-serif;
      overflow-x:hidden;
    }
    body:before{
      content:"";
      position:fixed;
      inset:0;
      pointer-events:none;
      background-image:
        linear-gradient(rgba(255,255,255,.035) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255,255,255,.035) 1px, transparent 1px);
      background-size:52px 52px;
      mask-image:linear-gradient(to bottom, black, transparent 78%);
      z-index:-2;
    }
    .orb{position:fixed; border-radius:50%; filter:blur(10px); opacity:.35; z-index:-1; animation:float 8s ease-in-out infinite alternate}
    .orb.one{width:280px;height:280px;background:var(--blue);left:-80px;top:150px}
    .orb.two{width:220px;height:220px;background:var(--pink);right:-60px;top:430px;animation-delay:1.4s}
    .orb.three{width:180px;height:180px;background:var(--cyan);left:45%;bottom:80px;animation-delay:.8s}
    @keyframes float{to{transform:translate3d(28px,-36px,0) scale(1.08)}}
    .container{width:min(1180px, calc(100% - 32px)); margin-inline:auto}
    nav{
      position:sticky;
      top:0;
      z-index:20;
      backdrop-filter:blur(20px);
      background:rgba(5,8,22,.68);
      border-bottom:1px solid var(--line);
    }
    .nav-inner{display:flex;align-items:center;justify-content:space-between;gap:18px;padding:14px 0}
    .brand{display:flex;align-items:center;gap:12px;text-decoration:none;color:var(--text)}
    .logo{
      width:44px;height:44px;border-radius:14px;
      display:grid;place-items:center;font-weight:900;
      background:linear-gradient(135deg,var(--cyan),var(--blue) 55%,var(--pink));
      color:#fff;box-shadow:0 0 30px rgba(23,231,255,.35)
    }
    .brand strong{font-family:Space Grotesk,Inter,sans-serif;font-size:1.12rem;letter-spacing:.3px}
    .brand span{display:block;color:var(--muted);font-size:.78rem;margin-top:2px}
    .links{display:flex;align-items:center;gap:20px}
    .links a{color:var(--muted);text-decoration:none;font-weight:700;font-size:.92rem}
    .links a:hover{color:#fff}
    .btn{border:0;cursor:pointer;text-decoration:none;color:#06101f;font-weight:900;border-radius:999px;padding:13px 18px;background:linear-gradient(135deg,var(--cyan),var(--yellow));box-shadow:0 12px 32px rgba(23,231,255,.24);display:inline-flex;align-items:center;gap:9px;white-space:nowrap}
    .btn.secondary{background:rgba(255,255,255,.08); color:var(--text); border:1px solid var(--line); box-shadow:none}
    .hero{padding:78px 0 42px;position:relative}
    .hero-grid{display:grid;grid-template-columns:1.04fr .96fr;gap:38px;align-items:center}
    .eyebrow{display:inline-flex;gap:8px;align-items:center;padding:9px 13px;border:1px solid rgba(23,231,255,.32);border-radius:999px;background:rgba(23,231,255,.08);color:#bdf8ff;font-weight:800;font-size:.86rem}
    h1{font-family:Space Grotesk,Inter,sans-serif;font-size:clamp(2.7rem,6vw,6.4rem);line-height:.92;margin:22px 0 18px;letter-spacing:-.06em}
    .gradient{background:linear-gradient(90deg,#fff 0%,var(--cyan) 40%,var(--pink) 78%,var(--yellow));-webkit-background-clip:text;background-clip:text;color:transparent}
    .lead{color:var(--muted);font-size:1.08rem;line-height:1.75;max-width:650px}
    .hero-actions{display:flex;gap:14px;flex-wrap:wrap;margin-top:28px}
    .stats{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:28px}
    .stat{background:var(--card);border:1px solid var(--line);border-radius:22px;padding:16px;box-shadow:var(--shadow)}
    .stat b{font-size:1.6rem;color:#fff}.stat span{display:block;color:var(--muted);font-size:.84rem;margin-top:5px}
    .scene{perspective:1100px;min-height:540px;position:relative}
    .device{
      min-height:430px;
      transform-style:preserve-3d;
      transform:rotateX(8deg) rotateY(-15deg);
      transition:.35s ease;
      background:linear-gradient(145deg,rgba(255,255,255,.12),rgba(255,255,255,.035));
      border:1px solid rgba(255,255,255,.18);
      border-radius:32px;padding:18px;box-shadow:0 32px 110px rgba(0,0,0,.55), 0 0 70px rgba(23,231,255,.16);
      position:relative;overflow:hidden;
    }
    .device:hover{transform:rotateX(3deg) rotateY(-8deg) translateY(-6px)}
    .screen{height:100%;min-height:405px;border-radius:24px;background:#060917;border:1px solid rgba(255,255,255,.13);overflow:hidden;position:relative;padding:22px}
    .screen:before{content:"";position:absolute;inset:0;background:radial-gradient(circle at 20% 10%, rgba(23,231,255,.19), transparent 35%), radial-gradient(circle at 80% 70%, rgba(255,43,214,.15), transparent 40%)}
    .mock-nav,.mock-content,.mock-row{position:relative;z-index:1}.mock-nav{display:flex;justify-content:space-between;align-items:center;margin-bottom:34px}.mock-nav div:first-child{height:18px;width:130px;background:linear-gradient(90deg,var(--cyan),var(--pink));border-radius:999px}.mock-nav div:last-child{height:14px;width:220px;background:rgba(255,255,255,.12);border-radius:999px}.mock-title{font-family:Space Grotesk;font-size:3.2rem;line-height:1;max-width:360px;margin-bottom:16px}.mock-content p{color:var(--muted);line-height:1.6}.mock-row{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin-top:30px}.mock-card{height:104px;border-radius:18px;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.12);padding:14px}.mock-card i{display:block;width:48px;height:14px;background:var(--cyan);border-radius:999px;margin-bottom:35px}.mock-card:nth-child(2) i{background:var(--pink)}.mock-card:nth-child(3) i{background:var(--yellow)}
    .float-card{position:absolute;background:rgba(255,255,255,.1);border:1px solid var(--line);backdrop-filter:blur(16px);border-radius:22px;padding:16px;box-shadow:var(--shadow);animation:cardFloat 5s ease-in-out infinite alternate}
    .float-card.one{left:-20px;bottom:30px}.float-card.two{right:-10px;top:50px;animation-delay:1s}.float-card b{display:block;font-size:1.05rem}.float-card span{color:var(--muted);font-size:.82rem}
    @keyframes cardFloat{to{transform:translateY(-18px)}}
    section{padding:76px 0}.section-head{display:flex;justify-content:space-between;align-items:end;gap:22px;margin-bottom:28px}.section-head h2{font-family:Space Grotesk;font-size:clamp(2rem,4vw,3.3rem);margin:0;letter-spacing:-.04em}.section-head p{color:var(--muted);max-width:520px;line-height:1.65}
    .services{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}.service-card,.pricing-card,.gallery-card,.calculator,.preview-box{background:linear-gradient(145deg,rgba(255,255,255,.105),rgba(255,255,255,.045));border:1px solid var(--line);border-radius:28px;box-shadow:var(--shadow);position:relative;overflow:hidden}.service-card{padding:26px;min-height:270px;transform-style:preserve-3d;transition:.25s ease}.service-card:hover{transform:translateY(-8px) rotateX(4deg);border-color:rgba(23,231,255,.42)}.service-icon{width:58px;height:58px;border-radius:18px;display:grid;place-items:center;background:rgba(23,231,255,.12);font-size:1.7rem;margin-bottom:20px}.service-card h3{font-size:1.45rem;margin:0 0 10px}.service-card p{color:var(--muted);line-height:1.65}.pill-list{display:flex;flex-wrap:wrap;gap:8px;margin-top:20px}.pill{font-size:.78rem;font-weight:800;border:1px solid rgba(255,255,255,.14);color:#cfe8ff;border-radius:999px;padding:7px 10px;background:rgba(255,255,255,.06)}
    .preview-box{padding:20px}.browser{border-radius:22px;overflow:hidden;border:1px solid rgba(255,255,255,.16);background:#060917}.browser-top{height:42px;background:rgba(255,255,255,.08);display:flex;align-items:center;gap:7px;padding:0 14px}.dot{width:11px;height:11px;border-radius:50%;background:var(--pink)}.dot:nth-child(2){background:var(--yellow)}.dot:nth-child(3){background:var(--green)}.browser-body{min-height:390px;padding:26px;background:radial-gradient(circle at 80% 10%,rgba(23,231,255,.22),transparent 30%),linear-gradient(135deg,#080d24,#02040f)}.site-hero{display:grid;grid-template-columns:1.1fr .9fr;gap:20px;align-items:center}.mini-title{font-family:Space Grotesk;font-size:2.2rem;line-height:1.05}.mini-panel{height:230px;border-radius:22px;background:linear-gradient(135deg,rgba(57,124,255,.3),rgba(255,43,214,.18));border:1px solid rgba(255,255,255,.14);display:grid;place-items:center;font-size:4rem}.mini-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:24px}.mini-grid div{height:95px;border-radius:16px;background:rgba(255,255,255,.08);border:1px solid rgba(255,255,255,.1);display:grid;place-items:center;color:var(--muted);font-weight:800;text-align:center;padding:8px}
    .gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}.gallery-card{min-height:295px;padding:18px}.art{height:190px;border-radius:22px;margin-bottom:16px;display:grid;place-items:center;position:relative;overflow:hidden;border:1px solid rgba(255,255,255,.12)}.art.poster{background:linear-gradient(135deg,#061126,#122f66)}.art.thumb{background:linear-gradient(135deg,#180914,#4f123d)}.art.web{background:linear-gradient(135deg,#061a16,#14364a)}.art .big{font-size:2.4rem;font-family:Space Grotesk;font-weight:900;text-align:center;line-height:1.05}.art .tag{position:absolute;right:12px;bottom:12px;background:#fff;color:#06101f;border-radius:999px;padding:8px 10px;font-weight:900;font-size:.78rem}.gallery-card h3{margin:0 0 7px}.gallery-card p{margin:0;color:var(--muted);line-height:1.55}
    .pricing{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}.pricing-card{padding:24px}.pricing-card.featured{border-color:rgba(23,231,255,.55);box-shadow:0 30px 100px rgba(23,231,255,.12)}.pricing-card h3{font-size:1.35rem;margin:0}.price{font-family:Space Grotesk;font-size:2.5rem;font-weight:900;margin:18px 0}.price small{font-size:1rem;color:var(--muted)}.features{list-style:none;padding:0;margin:20px 0 0}.features li{padding:10px 0;border-top:1px solid rgba(255,255,255,.09);color:#d8e8ff}.features li:before{content:"✓";color:var(--green);font-weight:900;margin-right:10px}
    .calculator{padding:26px}.calc-grid{display:grid;grid-template-columns:1fr 1fr;gap:18px}.field{display:flex;flex-direction:column;gap:8px;margin-bottom:16px}.field label{font-weight:800;color:#dceaff}.field input,.field select,.field textarea{width:100%;border:1px solid rgba(255,255,255,.16);background:rgba(0,0,0,.24);color:#fff;border-radius:16px;padding:13px 14px;font:inherit;outline:none}.field input:focus,.field select:focus,.field textarea:focus{border-color:var(--cyan);box-shadow:0 0 0 4px rgba(23,231,255,.1)}.checks{display:grid;grid-template-columns:1fr 1fr;gap:10px}.check{display:flex;align-items:center;gap:9px;padding:12px;border:1px solid rgba(255,255,255,.12);border-radius:16px;background:rgba(255,255,255,.055);color:#dceaff;font-weight:700}.result{background:linear-gradient(135deg,rgba(23,231,255,.12),rgba(255,43,214,.11));border:1px solid rgba(23,231,255,.25);border-radius:24px;padding:22px;position:sticky;top:96px}.result .total{font-family:Space Grotesk;font-size:3rem;font-weight:900;margin:10px 0;color:#fff}.breakdown{color:var(--muted);line-height:1.8;margin-top:12px}.whatsapp{width:100%;justify-content:center;margin-top:18px}.note{font-size:.86rem;color:var(--muted);line-height:1.55;margin-top:12px}
    .process{display:grid;grid-template-columns:repeat(4,1fr);gap:14px}.step{border:1px solid var(--line);border-radius:22px;padding:18px;background:rgba(255,255,255,.055)}.step b{display:grid;place-items:center;width:42px;height:42px;border-radius:14px;background:linear-gradient(135deg,var(--cyan),var(--blue));margin-bottom:14px;color:#00101c}.step h3{margin:0 0 8px}.step p{color:var(--muted);line-height:1.55;margin:0}
    footer{padding:46px 0;border-top:1px solid var(--line);background:rgba(0,0,0,.18)}.footer-grid{display:grid;grid-template-columns:1fr auto;gap:20px;align-items:center}.footer-grid p{color:var(--muted);line-height:1.6}.socials{display:flex;gap:10px;flex-wrap:wrap}
    .mobile-menu{display:none}
    @media(max-width:900px){
      .links{display:none}.mobile-menu{display:inline-flex}.hero-grid,.site-hero,.calc-grid,.footer-grid{grid-template-columns:1fr}.services,.gallery,.pricing{grid-template-columns:1fr}.process{grid-template-columns:1fr 1fr}.scene{min-height:auto}.device{transform:none}.float-card{display:none}.stats{grid-template-columns:1fr}.section-head{display:block}.checks{grid-template-columns:1fr}.browser-body{padding:18px}.mini-grid{grid-template-columns:1fr}.hero{padding-top:50px}.mock-row{grid-template-columns:1fr}.mock-title{font-size:2.4rem}.result{position:static}
    }
    @media(max-width:520px){.process{grid-template-columns:1fr}h1{font-size:3.2rem}.hero-actions .btn{width:100%;justify-content:center}}
  </style>
</head>
<body>
  <div class="orb one"></div><div class="orb two"></div><div class="orb three"></div>
  <nav>
    <div class="container nav-inner">
      <a href="#home" class="brand">
        <div class="logo">AD</div>
        <div><strong>Adi Desiging</strong><span>@adi_desiging_</span></div>
      </a>
      <div class="links">
        <a href="#services">Services</a>
        <a href="#preview">Preview</a>
        <a href="#gallery">Gallery</a>
        <a href="#pricing">Pricing</a>
        <a href="#calculator">Calculator</a>
      </div>
      <a class="btn" href="#calculator">Book Now</a>
    </div>
  </nav>

  <main id="home">
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="eyebrow">⚡ Posters • Thumbnails • Websites</span>
          <h1>Designs that make your <span class="gradient">brand look premium.</span></h1>
          <p class="lead">I create eye-catching posters, high-click YouTube thumbnails and modern WhatsApp booking websites for creators, shops, cafes, coaching centers and local businesses.</p>
          <div class="hero-actions">
            <a href="#calculator" class="btn">Calculate Price</a>
            <a href="#gallery" class="btn secondary">View Gallery</a>
          </div>
          <div class="stats">
            <div class="stat"><b>₹99+</b><span>Poster / thumbnail starting</span></div>
            <div class="stat"><b>₹1499+</b><span>Basic website starting</span></div>
            <div class="stat"><b>Fast</b><span>Preview + WhatsApp booking</span></div>
          </div>
        </div>
        <div class="scene">
          <div class="device tilt">
            <div class="screen">
              <div class="mock-nav"><div></div><div></div></div>
              <div class="mock-content">
                <div class="mock-title">Live 3D Website Design</div>
                <p>Modern layout, mobile-friendly pages, premium colors, gallery, pricing, contact and booking flow.</p>
              </div>
              <div class="mock-row">
                <div class="mock-card"><i></i>Poster</div>
                <div class="mock-card"><i></i>Thumbnail</div>
                <div class="mock-card"><i></i>Website</div>
              </div>
            </div>
          </div>
          <div class="float-card one"><b>WhatsApp Booking</b><span>Auto message generated</span></div>
          <div class="float-card two"><b>Live Calculator</b><span>Price updates instantly</span></div>
        </div>
      </div>
    </section>

    <section id="services">
      <div class="container">
        <div class="section-head">
          <h2>Services</h2>
          <p>Separate clean services for creators and businesses. Use this page as your portfolio and booking system.</p>
        </div>
        <div class="services">
          <article class="service-card tilt">
            <div class="service-icon">🎨</div>
            <h3>Poster Design</h3>
            <p>Business posters, coaching admission posts, cafe offers, sale posters, event banners and Instagram promotional designs.</p>
            <div class="pill-list"><span class="pill">Business</span><span class="pill">Event</span><span class="pill">Promotion</span></div>
          </article>
          <article class="service-card tilt">
            <div class="service-icon">▶️</div>
            <h3>Thumbnail Design</h3>
            <p>Bold and clickable YouTube thumbnails for gaming, education, tech, fitness, vlogs and creator content.</p>
            <div class="pill-list"><span class="pill">High CTR</span><span class="pill">YouTube</span><span class="pill">Creator</span></div>
          </article>
          <article class="service-card tilt">
            <div class="service-icon">🌐</div>
            <h3>Website Design</h3>
            <p>Modern websites for local businesses with pricing, gallery, contact section and WhatsApp booking button.</p>
            <div class="pill-list"><span class="pill">Responsive</span><span class="pill">Booking</span><span class="pill">Modern UI</span></div>
          </article>
        </div>
      </div>
    </section>

    <section id="preview">
      <div class="container">
        <div class="section-head">
          <h2>Live Website Preview</h2>
          <p>This section shows clients what kind of website you can build for their shop, cafe, coaching or personal brand.</p>
        </div>
        <div class="preview-box">
          <div class="browser">
            <div class="browser-top"><span class="dot"></span><span class="dot"></span><span class="dot"></span></div>
            <div class="browser-body">
              <div class="site-hero">
                <div>
                  <div class="eyebrow">Demo Client Website</div>
                  <div class="mini-title">We build websites that grow your local business.</div>
                  <p class="lead">Home, services, pricing, gallery and direct WhatsApp booking in one professional website.</p>
                  <a href="#calculator" class="btn">Get Website Quote</a>
                </div>
                <div class="mini-panel">💻</div>
              </div>
              <div class="mini-grid">
                <div>Business Website</div><div>Portfolio Website</div><div>Booking Website</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="gallery">
      <div class="container">
        <div class="section-head">
          <h2>Gallery</h2>
          <p>Post these as portfolio samples on Instagram. Replace mock designs later with your real client work.</p>
        </div>
        <div class="gallery">
          <article class="gallery-card tilt">
            <div class="art poster"><div class="big">COACHING<br>ADMISSION</div><span class="tag">Poster</span></div>
            <h3>Coaching Poster</h3><p>Admission, result, batch launch and exam campaign designs.</p>
          </article>
          <article class="gallery-card tilt">
            <div class="art thumb"><div class="big">I BUILT<br>₹1 LAKH<br>BUSINESS</div><span class="tag">Thumbnail</span></div>
            <h3>YouTube Thumbnail</h3><p>Bold title, emotion, contrast and click-focused layout.</p>
          </article>
          <article class="gallery-card tilt">
            <div class="art web"><div class="big">CAFE<br>WEBSITE<br>PREVIEW</div><span class="tag">Website</span></div>
            <h3>Business Website</h3><p>Landing page, menu, gallery, booking and contact system.</p>
          </article>
          <article class="gallery-card tilt">
            <div class="art poster"><div class="big">SALE<br>70% OFF</div><span class="tag">Poster</span></div>
            <h3>Sale Poster</h3><p>Festival offers, shop sale, product promotion and campaigns.</p>
          </article>
          <article class="gallery-card tilt">
            <div class="art thumb"><div class="big">7 DAY<br>WORKOUT<br>CHALLENGE</div><span class="tag">Thumbnail</span></div>
            <h3>Fitness Thumbnail</h3><p>Strong visual hierarchy for Shorts, videos and reels.</p>
          </article>
          <article class="gallery-card tilt">
            <div class="art web"><div class="big">ARTIST<br>PORTFOLIO</div><span class="tag">Website</span></div>
            <h3>Portfolio Website</h3><p>Showcase work, collect inquiries and convert visitors.</p>
          </article>
        </div>
      </div>
    </section>

    <section id="pricing">
      <div class="container">
        <div class="section-head">
          <h2>Price Section</h2>
          <p>Starter pricing for first clients. You can increase prices after reviews and portfolio proof.</p>
        </div>
        <div class="pricing">
          <article class="pricing-card">
            <h3>Poster Design</h3>
            <div class="price">₹99 <small>starting</small></div>
            <ul class="features">
              <li>Basic Instagram poster</li>
              <li>Business offer design</li>
              <li>HD PNG/JPG delivery</li>
              <li>Premium poster: ₹249</li>
            </ul>
          </article>
          <article class="pricing-card featured">
            <h3>Thumbnail Design</h3>
            <div class="price">₹99 <small>starting</small></div>
            <ul class="features">
              <li>YouTube thumbnail</li>
              <li>Bold text and effects</li>
              <li>Creator/gaming/education style</li>
              <li>Premium thumbnail: ₹199</li>
            </ul>
          </article>
          <article class="pricing-card">
            <h3>Website Design</h3>
            <div class="price">₹1499 <small>starting</small></div>
            <ul class="features">
              <li>One page basic website</li>
              <li>Mobile friendly layout</li>
              <li>WhatsApp booking button</li>
              <li>Booking website: ₹4999</li>
            </ul>
          </article>
        </div>
      </div>
    </section>

    <section id="calculator">
      <div class="container">
        <div class="section-head">
          <h2>Automatic Price Calculator</h2>
          <p>Select service and options. The website automatically calculates price and creates a WhatsApp booking message.</p>
        </div>
        <div class="calculator">
          <div class="calc-grid">
            <div>
              <div class="field">
                <label>Your Name</label>
                <input id="clientName" type="text" placeholder="Enter your name" />
              </div>
              <div class="field">
                <label>Service</label>
                <select id="service">
                  <option value="poster">Poster Design</option>
                  <option value="thumbnail">Thumbnail Design</option>
                  <option value="website">Website Design</option>
                </select>
              </div>
              <div class="field">
                <label>Package</label>
                <select id="package"></select>
              </div>
              <div class="field">
                <label>Quantity / Pages</label>
                <input id="qty" type="number" min="1" value="1" />
              </div>
              <div class="field">
                <label>Add-ons</label>
                <div class="checks">
                  <label class="check"><input type="checkbox" id="urgent" /> Urgent delivery +₹299</label>
                  <label class="check"><input type="checkbox" id="source" /> Source file +₹199</label>
                  <label class="check"><input type="checkbox" id="extraRevision" /> Extra revision +₹99</label>
                  <label class="check"><input type="checkbox" id="seo" /> Basic SEO setup +₹499</label>
                </div>
              </div>
              <div class="field">
                <label>Project Details</label>
                <textarea id="details" rows="4" placeholder="Example: coaching admission poster, gaming thumbnail, cafe website etc."></textarea>
              </div>
            </div>
            <div class="result">
              <span class="eyebrow">Instant Quote</span>
              <div class="total" id="total">₹99</div>
              <div class="breakdown" id="breakdown"></div>
              <button class="btn whatsapp" id="whatsappBtn">Book on WhatsApp</button>
              <p class="note">Note: Final price can change if the work is complex. Take 50% advance before starting any client project.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="process">
      <div class="container">
        <div class="section-head">
          <h2>Order Process</h2>
          <p>Simple system for clients. This makes you look professional and avoids confusion.</p>
        </div>
        <div class="process">
          <div class="step"><b>1</b><h3>Send Details</h3><p>Client shares service, content, logo, images and deadline.</p></div>
          <div class="step"><b>2</b><h3>Advance</h3><p>Start work after 50% advance payment confirmation.</p></div>
          <div class="step"><b>3</b><h3>Preview</h3><p>Send watermarked preview and take revision feedback.</p></div>
          <div class="step"><b>4</b><h3>Final Delivery</h3><p>After final payment, deliver HD file or live website link.</p></div>
        </div>
      </div>
    </section>
  </main>

  <footer>
    <div class="container footer-grid">
      <div>
        <a href="#home" class="brand"><div class="logo">AD</div><div><strong>Adi Desiging</strong><span>Poster • Thumbnail • Website</span></div></a>
        <p>Design service for creators and local businesses. DM on Instagram or book through WhatsApp.</p>
      </div>
      <div class="socials">
        <a class="btn secondary" href="https://www.instagram.com/adi_desiging_/" target="_blank" rel="noreferrer">Instagram</a>
        <a class="btn" href="#calculator">Calculate Price</a>
      </div>
    </div>
  </footer>

  <script>
    // Change this number if your WhatsApp business number is different.
    const WHATSAPP_NUMBER = "8090399288";

    const packageData = {
      poster: [
        { name: "Basic Poster", price: 99 },
        { name: "Premium Poster", price: 249 },
        { name: "3 Poster Pack", price: 499 }
      ],
      thumbnail: [
        { name: "Basic Thumbnail", price: 99 },
        { name: "Premium Thumbnail", price: 199 },
        { name: "5 Thumbnail Pack", price: 799 }
      ],
      website: [
        { name: "Basic One Page Website", price: 1499 },
        { name: "Business Website", price: 2999 },
        { name: "WhatsApp Booking Website", price: 4999 }
      ]
    };

    const serviceEl = document.getElementById("service");
    const packageEl = document.getElementById("package");
    const qtyEl = document.getElementById("qty");
    const totalEl = document.getElementById("total");
    const breakdownEl = document.getElementById("breakdown");
    const whatsappBtn = document.getElementById("whatsappBtn");

    function setPackages(){
      const service = serviceEl.value;
      packageEl.innerHTML = packageData[service].map((p, i) => `<option value="${i}">${p.name} - ₹${p.price}</option>`).join("");
      qtyEl.value = 1;
      calculate();
    }

    function money(n){ return "₹" + n.toLocaleString("en-IN"); }

    function calculate(){
      const service = serviceEl.value;
      const selected = packageData[service][Number(packageEl.value || 0)];
      const qty = Math.max(1, Number(qtyEl.value || 1));
      let total = selected.price * qty;
      const items = [`${selected.name} × ${qty}: ${money(selected.price * qty)}`];

      const urgent = document.getElementById("urgent").checked;
      const source = document.getElementById("source").checked;
      const extraRevision = document.getElementById("extraRevision").checked;
      const seo = document.getElementById("seo").checked;

      if(urgent){ total += 299; items.push("Urgent delivery: ₹299"); }
      if(source){ total += 199; items.push("Source file: ₹199"); }
      if(extraRevision){ total += 99; items.push("Extra revision: ₹99"); }
      if(seo){ total += 499; items.push("Basic SEO setup: ₹499"); }

      totalEl.textContent = money(total);
      breakdownEl.innerHTML = items.join("<br>");
      return { service, selected, qty, total, items };
    }

    function bookWhatsApp(){
      const quote = calculate();
      const name = document.getElementById("clientName").value.trim() || "Client";
      const details = document.getElementById("details").value.trim() || "No extra details added";
      const serviceName = serviceEl.options[serviceEl.selectedIndex].text;
      const message = `Hello, I want to book a design service.%0A%0AName: ${encodeURIComponent(name)}%0AService: ${encodeURIComponent(serviceName)}%0APackage: ${encodeURIComponent(quote.selected.name)}%0AQuantity/Pages: ${quote.qty}%0AEstimated Price: ${encodeURIComponent(money(quote.total))}%0ADetails: ${encodeURIComponent(details)}%0A%0APlease confirm availability and advance payment details.`;
      window.open(`https://wa.me/${WHATSAPP_NUMBER}?text=${message}`, "_blank");
    }

    [serviceEl, packageEl, qtyEl, ...document.querySelectorAll("input[type='checkbox']")].forEach(el => el.addEventListener("input", calculate));
    serviceEl.addEventListener("change", setPackages);
    whatsappBtn.addEventListener("click", bookWhatsApp);
    setPackages();

    // 3D tilt interaction
    document.querySelectorAll(".tilt").forEach(card => {
      card.addEventListener("mousemove", e => {
        const rect = card.getBoundingClientRect();
        const x = e.clientX - rect.left;
        const y = e.clientY - rect.top;
        const rx = ((y / rect.height) - .5) * -8;
        const ry = ((x / rect.width) - .5) * 8;
        card.style.transform = `rotateX(${rx}deg) rotateY(${ry}deg) translateY(-6px)`;
      });
      card.addEventListener("mouseleave", () => card.style.transform = "");
    });
  </script>
</body>
</html>
