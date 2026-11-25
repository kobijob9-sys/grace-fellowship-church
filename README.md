<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Grace Fellowship Church — a place to grow in faith, find community, and serve with love.">
  <title>Grace Fellowship Church | Welcome Home</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Playfair+Display:wght@500;600;700&display=swap" rel="stylesheet">
  <style>
    :root{--navy:#142b35;--navy2:#1d3b46;--gold:#c69b5b;--cream:#f7f5f0;--ink:#26343a;--muted:#68777b;--white:#fff}
    *{box-sizing:border-box}html{scroll-behavior:smooth;scroll-padding-top:82px}
    body{margin:0;font-family:"DM Sans",sans-serif;color:var(--ink);background:#fff;line-height:1.65}
    a{color:inherit;text-decoration:none}.container{width:min(1120px,90%);margin:auto}
    .topbar{background:var(--navy);color:#e9e7df;font-size:.84rem;padding:9px 0}.topbar .container{display:flex;justify-content:space-between;gap:16px;flex-wrap:wrap}
    header{position:sticky;top:0;z-index:20;background:rgba(255,255,255,.96);backdrop-filter:blur(10px);box-shadow:0 2px 18px #142b3510}
    .nav{height:76px;display:flex;align-items:center;justify-content:space-between;gap:24px}
    .brand{display:flex;align-items:center;gap:12px;font-weight:700;color:var(--navy);letter-spacing:.02em}
    .brand-mark{width:42px;height:42px;border-radius:50%;display:grid;place-items:center;background:var(--navy);color:var(--gold);font-family:Georgia,serif;font-size:25px}
    .brand small{display:block;font-size:.66rem;letter-spacing:.17em;color:var(--muted);font-weight:600}
    .links{display:flex;align-items:center;gap:25px;font-size:.91rem;font-weight:600}.links a:hover{color:#a7793e}
    .btn{display:inline-flex;align-items:center;justify-content:center;padding:12px 21px;border-radius:4px;background:var(--gold);color:#172a30;font-weight:700;border:1px solid var(--gold);transition:.2s}
    .btn:hover{background:#d5b27e;transform:translateY(-1px)}.btn.outline{background:transparent;color:white;border-color:#ffffff9c}
    .menu-btn{display:none;background:none;border:0;font-size:27px;color:var(--navy);cursor:pointer}
    .hero{min-height:610px;display:flex;align-items:center;color:white;background:linear-gradient(90deg,rgba(11,30,38,.88),rgba(11,30,38,.45)),url('https://images.unsplash.com/photo-1438032005730-c779502df39b?auto=format&fit=crop&w=2000&q=85') center/cover}
    .hero-content{max-width:680px;padding:100px 0}.eyebrow{color:var(--gold);font-size:.78rem;font-weight:700;letter-spacing:.2em;text-transform:uppercase}
    h1,h2,h3{font-family:"Playfair Display",Georgia,serif;line-height:1.16}h1{font-size:clamp(2.8rem,6vw,5.3rem);margin:18px 0}
    .hero p{font-size:1.12rem;max-width:560px;color:#edf0ed;margin:0 0 30px}.hero-actions{display:flex;gap:13px;flex-wrap:wrap}
    section{padding:88px 0}.section-head{text-align:center;max-width:700px;margin:0 auto 45px}.section-head h2{font-size:clamp(2rem,4vw,3rem);color:var(--navy);margin:10px 0 14px}.section-head p{color:var(--muted);margin:0}
    .intro-grid{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
    .intro-photo{height:430px;border-radius:8px;background:url('https://images.unsplash.com/photo-1511632765486-a01980e01a18?auto=format&fit=crop&w=1100&q=85') center/cover}
    .intro-copy h2{font-size:2.7rem;color:var(--navy);margin:10px 0 18px}.intro-copy p{color:var(--muted)}
    .text-link{display:inline-block;color:#9a6d35;font-weight:700;margin-top:12px;border-bottom:1px solid var(--gold);padding-bottom:4px}
    .verse{background:var(--cream);text-align:center}.verse-card{max-width:850px;margin:auto;padding:42px 30px;border:1px solid #e7dfd1;background:#fff;border-radius:8px}
    .verse-mark{font-family:Georgia,serif;color:var(--gold);font-size:3.5rem;line-height:1}.verse blockquote{font-family:"Playfair Display",serif;font-size:clamp(1.35rem,3vw,2rem);color:var(--navy);margin:12px 0 16px}.verse cite{font-style:normal;color:#9a6d35;font-weight:700}
    .services{background:var(--navy);color:white}.services .section-head h2{color:white}.services .section-head p{color:#c5d0d0}
    .service-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:20px}.service-card{padding:30px 25px;border:1px solid #ffffff2c;border-radius:7px;background:#ffffff08}
    .service-card .symbol{font-size:1.8rem;color:var(--gold)}.service-card h3{font-size:1.45rem;margin:12px 0 7px}.service-card p{color:#c5d0d0;margin:0}.service-card strong{display:block;color:#f0d5aa;margin-top:13px;font-size:.92rem}
    .ministries-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:22px}.ministry{border:1px solid #e8e8e4;border-radius:7px;overflow:hidden;background:white}.ministry-img{height:185px;background-size:cover;background-position:center}.ministry-body{padding:22px}.ministry h3{color:var(--navy);font-size:1.35rem;margin:0 0 8px}.ministry p{color:var(--muted);font-size:.94rem;margin:0}
    .events{background:var(--cream)}.event-list{max-width:850px;margin:auto;display:grid;gap:14px}.event{display:flex;align-items:center;gap:22px;padding:22px;background:#fff;border:1px solid #e8e1d6;border-radius:6px}.date{min-width:66px;text-align:center;background:var(--navy);color:white;padding:9px 8px;border-radius:4px}.date b{display:block;font-family:"Playfair Display",serif;font-size:1.7rem;line-height:1.1}.date span{font-size:.7rem;letter-spacing:.1em}.event h3{font-size:1.25rem;color:var(--navy);margin:0 0 4px}.event p{color:var(--muted);margin:0;font-size:.9rem}
    .contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:50px}.contact-copy h2{font-size:2.7rem;color:var(--navy);margin:10px 0 16px}.contact-copy p{color:var(--muted)}.contact-item{margin:20px 0}.contact-item b{display:block;color:var(--navy)}.contact-panel{background:var(--cream);padding:32px;border-radius:7px}.contact-panel h3{font-size:1.6rem;color:var(--navy);margin-top:0}.contact-panel p{color:var(--muted)}.contact-panel a{color:#986b35;font-weight:700}
    footer{background:#0e222a;color:#d7dfdd;padding:30px 0}.footer-inner{display:flex;justify-content:space-between;gap:20px;align-items:center;flex-wrap:wrap}.footer-inner small{color:#aebcba}.footer-links{display:flex;gap:18px;font-size:.88rem}
    @media(max-width:850px){.links{gap:13px;font-size:.82rem}.links .btn{padding:10px 13px}.intro-grid{gap:30px}.service-grid,.ministries-grid{grid-template-columns:repeat(2,1fr)}}
    @media(max-width:680px){.topbar .container{justify-content:center;text-align:center}.nav{height:68px}.menu-btn{display:block}.links{display:none;position:absolute;top:68px;left:0;right:0;background:white;padding:20px 5%;box-shadow:0 12px 15px #142b3512;flex-direction:column;align-items:stretch}.links.open{display:flex}.links .btn{text-align:center}.hero{min-height:570px}.hero-content{padding:75px 0}.intro-grid,.contact-grid{grid-template-columns:1fr}.intro-photo{height:300px;order:2}.service-grid,.ministries-grid{grid-template-columns:1fr}.event{align-items:flex-start;gap:14px}.event-list{gap:10px}section{padding:68px 0}.contact-panel{padding:25px}}
  </style>
</head>
<body>
  <div class="topbar"><div class="container"><span>✦ Growing in faith. Living in love. Serving our community.</span><span>All are welcome at Grace Fellowship Church</span></div></div>
  <header>
    <div class="container nav">
      <a class="brand" href="#home"><span class="brand-mark">✝</span><span>GRACE FELLOWSHIP<small>CHURCH</small></span></a>
      <button class="menu-btn" aria-label="Open navigation" onclick="document.querySelector('.links').classList.toggle('open')">☰</button>
      <nav class="links" aria-label="Main navigation">
        <a href="#home">Home</a><a href="#about">About</a><a href="#services">Services</a><a href="#ministries">Ministries</a><a href="#events">Events</a><a href="#contact">Contact</a><a class="btn" href="#services">Plan a Visit</a>
      </nav>
    </div>
  </header>
  <main>
    <section class="hero" id="home"><div class="container"><div class="hero-content">
      <div class="eyebrow">Welcome to Grace Fellowship Church</div>
      <h1>A place to belong.<br>A faith to grow.</h1>
      <p>We are a community brought together by God's grace, growing in Christ, encouraging one another and sharing His love with the world.</p>
      <div class="hero-actions"><a class="btn" href="#services">Join Us This Sunday</a><a class="btn outline" href="#about">Discover Our Church</a></div>
    </div></div></section>
    <section id="about"><div class="container intro-grid">
      <div class="intro-photo" role="img" aria-label="People sharing fellowship together"></div>
      <div class="intro-copy"><div class="eyebrow">Who We Are</div><h2>Faith. Fellowship. Purpose.</h2>
        <p>Grace Fellowship Church is a Christ-centred community where people from every walk of life can encounter God's love, deepen their faith and find meaningful connections.</p>
        <p>Our desire is to worship wholeheartedly, grow through God's Word and serve our neighbours with compassion.</p>
        <a class="text-link" href="#contact">Come and meet us →</a>
      </div>
    </div></section>
    <section class="verse"><div class="container"><div class="section-head"><div class="eyebrow">A Moment in the Word</div><h2>Daily Bible Verse</h2><p>Take a moment to pause, reflect and be encouraged by Scripture.</p></div>
      <div class="verse-card"><div class="verse-mark">“</div><blockquote id="verse-text">The Lord is my shepherd; I shall not want.</blockquote><cite id="verse-ref">Psalm 23:1 (KJV)</cite></div>
    </div></section>
    <section class="services" id="services"><div class="container"><div class="section-head"><div class="eyebrow">Worship With Us</div><h2>Service Times</h2><p>There is a place for you here. Join us as we worship, learn and grow together.</p></div>
      <div class="service-grid">
        <article class="service-card"><div class="symbol">✦</div><h3>Sunday Worship</h3><p>Our main weekly gathering for worship, prayer and the teaching of God's Word.</p><strong>[Add time] · Sunday</strong></article>
        <article class="service-card"><div class="symbol">⌁</div><h3>Bible Study</h3><p>Explore Scripture together and discover how to live out your faith every day.</p><strong>[Add time] · [Add day]</strong></article>
        <article class="service-card"><div class="symbol">♡</div><h3>Prayer Meeting</h3><p>A time to seek God together, give thanks and stand with one another in prayer.</p><strong>[Add time] · [Add day]</strong></article>
      </div>
    </div></section>
    <section id="ministries"><div class="container"><div class="section-head"><div class="eyebrow">Find Your Place</div><h2>Our Ministries</h2><p>Discover opportunities to connect, serve and grow in every season of life.</p></div>
      <div class="ministries-grid">
        <article class="ministry"><div class="ministry-img" style="background-image:url('https://images.unsplash.com/photo-1529156069898-49953e39b3ac?auto=format&fit=crop&w=900&q=80')"></div><div class="ministry-body"><h3>Youth Ministry</h3><p>Building a generation grounded in faith, purpose and godly friendships.</p></div></article>
        <article class="ministry"><div class="ministry-img" style="background-image:url('https://images.unsplash.com/photo-1511895426328-dc8714191300?auto=format&fit=crop&w=900&q=80')"></div><div class="ministry-body"><h3>Children's Ministry</h3><p>Helping children discover God's love in a safe, joyful and caring environment.</p></div></article>
        <article class="ministry"><div class="ministry-img" style="background-image:url('https://images.unsplash.com/photo-1516280440614-37939bbacd81?auto=format&fit=crop&w=900&q=80')"></div><div class="ministry-body"><h3>Worship Ministry</h3><p>Using music and creativity to lead the church in heartfelt worship.</p></div></article>
      </div>
    </div></section>
    <section class="events" id="events"><div class="container"><div class="section-head"><div class="eyebrow">Life Together</div><h2>Upcoming Events</h2><p>Make room for fellowship, encouragement and moments that strengthen our faith.</p></div>
      <div class="event-list">
        <article class="event"><div class="date"><b>01</b><span>EVENT</span></div><div><h3>Community Fellowship</h3><p>[Add event date, time and venue]</p></div></article>
        <article class="event"><div class="date"><b>02</b><span>EVENT</span></div><div><h3>Prayer & Worship Night</h3><p>[Add event date, time and venue]</p></div></article>
        <article class="event"><div class="date"><b>03</b><span>EVENT</span></div><div><h3>Youth Gathering</h3><p>[Add event date, time and venue]</p></div></article>
      </div>
    </div></section>
    <section id="contact"><div class="container contact-grid">
      <div class="contact-copy"><div class="eyebrow">We Would Love to Hear From You</div><h2>Let's connect.</h2><p>Whether you are visiting for the first time, looking for a church home or simply have a question, you are welcome to reach out.</p>
        <div class="contact-item"><b>Address</b><span>[Add church physical address]</span></div>
        <div class="contact-item"><b>Phone</b><span>[Add church phone number]</span></div>
        <div class="contact-item"><b>Email</b><span>[Add church email address]</span></div>
      </div>
      <div class="contact-panel"><h3>Your place is here.</h3><p>We look forward to welcoming you at Grace Fellowship Church. Come as you are; there is room for you.</p><p><b>New here?</b><br>Contact the church office for directions, service details or more information about getting involved.</p><a href="mailto:YOUR-CHURCH-EMAIL@example.com">Email the church →</a></div>
    </div></section>
  </main>
  <footer><div class="container footer-inner"><div><b>GRACE FELLOWSHIP CHURCH</b><br><small>Growing in faith. Living in love. Serving our community.</small></div><div class="footer-links"><a href="#about">About</a><a href="#services">Services</a><a href="#contact">Contact</a></div><small>© <span id="year"></span> Grace Fellowship Church. All rights reserved.</small></div></footer>
  <script>
    const verses=[
      ["The Lord is my shepherd; I shall not want.","Psalm 23:1 (KJV)"],
      ["I can do all things through Christ which strengtheneth me.","Philippians 4:13 (KJV)"],
      ["Be still, and know that I am God.","Psalm 46:10 (KJV)"],
      ["Trust in the LORD with all thine heart; and lean not unto thine own understanding.","Proverbs 3:5 (KJV)"],
      ["For we walk by faith, not by sight.","2 Corinthians 5:7 (KJV)"],
      ["The joy of the LORD is your strength.","Nehemiah 8:10 (KJV)"],
      ["Let all your things be done with charity.","1 Corinthians 16:14 (KJV)"]
    ];
    const today=new Date();const verse=verses[Math.floor((Date.UTC(today.getFullYear(),today.getMonth(),today.getDate())/86400000))%verses.length];
    document.getElementById('verse-text').textContent=verse[0];document.getElementById('verse-ref').textContent=verse[1];
    document.getElementById('year').textContent=today.getFullYear();
    document.querySelectorAll('.links a').forEach(a=>a.addEventListener('click',()=>document.querySelector('.links').classList.remove('open')));
  </script>
</body>
</html>
