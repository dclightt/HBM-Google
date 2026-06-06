<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Home Builder Marketers · Google Just Killed the Ten Blue Links</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#191925;
    --layer:#20202c;
    --layer2:#292936;
    --white:#FFFFFF;
    --aqua:#DAFFFF;
    --gray:#BBBBBB;
    --teal:#03B6B6;
    --teal-hi:#19D6D6;
    --navy:#191925;
    --hairline:rgba(255,255,255,0.13);
    --hairline2:rgba(255,255,255,0.07);
  }
  *{box-sizing:border-box;margin:0;padding:0}
  html{scroll-behavior:smooth}
  body{
    background:var(--bg);color:var(--white);
    font-family:Arial,"Helvetica Neue",Helvetica,sans-serif;
    font-weight:400;font-size:18px;line-height:1.65;letter-spacing:-0.01em;
    overflow-x:hidden;-webkit-font-smoothing:antialiased;position:relative;
  }
  body::before{
    content:"";position:fixed;inset:0;pointer-events:none;opacity:0.05;
    mix-blend-mode:screen;z-index:1;
    background-image:url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='160' height='160'><filter id='n'><feTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='2' stitchTiles='stitch'/><feColorMatrix values='0 0 0 0 1 0 0 0 0 1 0 0 0 0 1 0 0 0 1 0'/></filter><rect width='100%25' height='100%25' filter='url(%23n)'/></svg>");
  }
  ::selection{background:var(--teal);color:var(--navy)}
  .wrap{position:relative;z-index:2;max-width:1240px;margin:0 auto;padding:0 32px}

  /* Display + label type helpers */
  .display{font-family:"Bebas Neue",Impact,"Arial Narrow",sans-serif;font-weight:400;letter-spacing:0.005em;}
  .label{font-family:Arial,sans-serif;font-weight:700;text-transform:uppercase;letter-spacing:0.2em;}

  /* NAV */
  nav.top{display:flex;justify-content:space-between;align-items:center;padding:22px 0;border-bottom:1px solid var(--hairline);gap:24px}
  .nav-logo{height:46px;width:auto;display:block}
  .nav-links{display:flex;align-items:center;gap:30px}
  .nav-links a{
    font-family:Arial,sans-serif;font-weight:700;font-size:12px;text-transform:uppercase;
    letter-spacing:0.14em;color:var(--gray);text-decoration:none;transition:color 0.2s ease;
  }
  .nav-links a:hover{color:var(--teal)}
  .nav-book{
    background:var(--teal);color:var(--navy) !important;padding:12px 22px;
    letter-spacing:0.12em !important;transition:background 0.2s ease,color 0.2s ease;
  }
  .nav-book:hover{background:var(--aqua);color:var(--navy) !important}

  /* HERO */
  .hero{padding:78px 0 96px;position:relative}
  .eyebrow{
    display:inline-flex;align-items:center;gap:14px;font-family:Arial,sans-serif;font-weight:700;
    font-size:12px;text-transform:uppercase;letter-spacing:0.22em;color:var(--teal);margin-bottom:34px;
  }
  .eyebrow .pulse{width:8px;height:8px;border-radius:50%;background:var(--teal);
    box-shadow:0 0 0 0 rgba(3,182,182,0.55);animation:pulse 2.4s infinite;}
  @keyframes pulse{0%{box-shadow:0 0 0 0 rgba(3,182,182,0.55)}70%{box-shadow:0 0 0 14px rgba(3,182,182,0)}100%{box-shadow:0 0 0 0 rgba(3,182,182,0)}}

  h1.headline{
    font-family:"Bebas Neue",Impact,"Arial Narrow",sans-serif;font-weight:400;
    font-size:clamp(58px,9.5vw,140px);line-height:0.9;letter-spacing:0.005em;
    max-width:15ch;color:var(--white);text-transform:uppercase;
  }
  h1.headline em{font-style:normal;color:var(--teal)}
  h1.headline .blocky{display:inline-block;background:var(--teal);color:var(--navy);
    padding:0 0.14em 0.02em;font-style:normal;transform:rotate(-0.5deg);}

  .hero-grid{display:grid;grid-template-columns:1.6fr 1fr;gap:60px;margin-top:54px;align-items:start}
  .lede{font-family:Arial,sans-serif;font-weight:400;font-size:20px;line-height:1.6;
    letter-spacing:-0.01em;color:var(--white);}
  .lede strong{color:var(--white);font-weight:700;
    background:linear-gradient(to top,rgba(3,182,182,0.32) 45%,transparent 45%);padding:0 2px;}

  .meta-card{background:var(--layer);border:1px solid var(--hairline);padding:28px;position:relative}
  .meta-card::before{content:"";position:absolute;top:14px;right:14px;width:10px;height:10px;background:var(--teal)}
  .meta-card h4{font-family:Arial,sans-serif;font-weight:700;font-size:11px;text-transform:uppercase;
    letter-spacing:0.2em;color:var(--gray);margin-bottom:18px}
  .meta-row{display:flex;justify-content:space-between;padding:12px 0;border-bottom:1px solid var(--hairline2);font-size:15px;color:var(--white);gap:14px}
  .meta-row:last-child{border-bottom:none}
  .meta-row span:first-child{color:var(--gray)}
  .meta-row span:last-child{font-weight:700;color:var(--white);text-align:right}

  /* MARQUEE */
  .marquee{margin:58px 0;overflow:hidden;background:var(--teal);color:var(--navy)}
  .marquee-track{display:flex;gap:54px;padding:14px 0;white-space:nowrap;animation:scroll 40s linear infinite;
    font-family:"Bebas Neue",Impact,sans-serif;font-size:28px;letter-spacing:0.04em}
  .marquee-track span{display:flex;align-items:center;gap:54px}
  .marquee-track .star{color:var(--navy);font-size:16px}
  @keyframes scroll{from{transform:translateX(0)}to{transform:translateX(-50%)}}

  /* SECTIONS */
  section{padding:88px 0;position:relative}
  .section-head{display:grid;grid-template-columns:130px 1fr;gap:40px;margin-bottom:54px;align-items:start}
  .section-num{font-family:Arial,sans-serif;font-weight:700;font-size:12px;color:var(--teal);
    letter-spacing:0.16em;padding-top:10px;text-transform:uppercase}
  .section-num::before{content:"";display:inline-block;width:22px;height:2px;background:var(--teal);vertical-align:middle;margin-right:10px}
  h2{font-family:"Bebas Neue",Impact,sans-serif;font-weight:400;font-size:clamp(40px,6vw,72px);
    line-height:0.98;letter-spacing:0.01em;max-width:20ch;color:var(--white);text-transform:uppercase}
  h2 em{font-style:normal;color:var(--teal)}

  .body-grid{display:grid;grid-template-columns:130px 1fr;gap:40px}
  .body-content p{margin-bottom:1.3em;font-size:19px;color:var(--white);max-width:62ch;line-height:1.65;letter-spacing:-0.01em}
  .body-content p strong{color:var(--teal);font-weight:700}

  /* STAT STRIP */
  .stat-strip{background:var(--layer);padding:78px 0;margin:40px 0;border-top:1px solid var(--hairline);border-bottom:1px solid var(--hairline)}
  .stat-row{display:grid;grid-template-columns:repeat(3,1fr);margin-top:54px;border-top:1px solid var(--hairline);border-bottom:1px solid var(--hairline)}
  .stat{padding:34px 28px;border-right:1px solid var(--hairline)}
  .stat:last-child{border-right:none}
  .stat-num{font-family:"Bebas Neue",Impact,sans-serif;font-weight:400;font-size:84px;line-height:0.9;
    letter-spacing:0.01em;color:var(--teal);margin-bottom:12px}
  .stat-label{font-family:Arial,sans-serif;font-weight:700;font-size:11px;text-transform:uppercase;letter-spacing:0.16em;color:var(--gray);line-height:1.5}

  /* CAPABILITIES */
  .caps{display:grid;grid-template-columns:repeat(2,1fr);gap:1px;background:var(--hairline);border:1px solid var(--hairline);margin-top:40px}
  .cap{background:var(--bg);padding:42px 36px;position:relative;transition:background 0.3s ease}
  .cap:hover{background:var(--layer)}
  .cap-num{font-family:Arial,sans-serif;font-weight:700;font-size:11px;color:var(--teal);letter-spacing:0.16em;margin-bottom:22px;display:block}
  .cap h3{font-family:Arial,sans-serif;font-weight:700;font-size:23px;line-height:1.2;letter-spacing:-0.02em;margin-bottom:16px;color:var(--white)}
  .cap p{font-size:17px;color:var(--gray);line-height:1.6;letter-spacing:-0.01em}
  .cap .cap-icon{position:absolute;top:36px;right:36px;width:42px;height:42px;border:1px solid var(--teal);color:var(--teal);
    display:flex;align-items:center;justify-content:center;font-family:"Bebas Neue",sans-serif;font-size:24px}

  /* PULL */
  .pull{padding:120px 0;text-align:center;position:relative;background:var(--layer);border-top:1px solid var(--hairline);border-bottom:1px solid var(--hairline)}
  .pull-quote{font-family:"Bebas Neue",Impact,sans-serif;font-weight:400;font-size:clamp(42px,6.5vw,76px);
    line-height:1.0;letter-spacing:0.01em;max-width:24ch;margin:0 auto;color:var(--white);text-transform:uppercase}
  .pull-quote::before{content:"";display:block;width:60px;height:4px;background:var(--teal);margin:0 auto 34px}
  .pull-attr{font-family:Arial,sans-serif;font-weight:700;font-size:11px;text-transform:uppercase;letter-spacing:0.22em;color:var(--gray);margin-top:36px}

  /* VS */
  .vs{display:grid;grid-template-columns:1fr 1fr;gap:1px;background:var(--hairline);border:1px solid var(--hairline);margin-top:40px}
  .vs > div{padding:48px 42px;background:var(--bg)}
  .vs .label{font-family:Arial,sans-serif;font-weight:700;font-size:11px;text-transform:uppercase;letter-spacing:0.22em;margin-bottom:22px}
  .vs .before .label{color:var(--gray)}
  .vs .after .label{color:var(--teal)}
  .vs h3{font-family:Arial,sans-serif;font-weight:700;font-size:23px;line-height:1.35;letter-spacing:-0.01em;color:var(--white)}
  .vs .before h3{color:var(--gray);text-decoration:line-through;text-decoration-color:var(--teal);text-decoration-thickness:2px}

  /* ARROW LIST */
  .arrow-list{list-style:none;margin-top:40px;border-top:1px solid var(--hairline)}
  .arrow-list li{display:grid;grid-template-columns:54px 1fr;gap:28px;padding:30px 0;border-bottom:1px solid var(--hairline);align-items:baseline}
  .arrow-list .arrow{font-family:"Bebas Neue",sans-serif;font-size:34px;color:var(--teal);line-height:1}
  .arrow-list h4{font-family:Arial,sans-serif;font-weight:700;font-size:21px;margin-bottom:8px;letter-spacing:-0.01em;color:var(--white);line-height:1.25}
  .arrow-list p{color:var(--gray);font-size:17px;max-width:60ch;line-height:1.6;letter-spacing:-0.01em}

  /* WARNING */
  .warning{margin:80px auto;max-width:920px;background:var(--teal);color:var(--navy);padding:58px 50px;position:relative}
  .warning::before{content:"!";position:absolute;top:28px;left:30px;font-family:"Bebas Neue",sans-serif;font-size:48px;color:var(--navy)}
  .warning h3{font-family:"Bebas Neue",Impact,sans-serif;font-weight:400;font-size:40px;margin-bottom:18px;margin-left:56px;color:var(--navy);line-height:1.0;letter-spacing:0.01em;text-transform:uppercase}
  .warning p{color:var(--navy);margin-left:56px;font-size:17px;max-width:60ch;line-height:1.6;font-weight:400;letter-spacing:-0.01em}
  .warning p + p{margin-top:14px}
  .warning p strong{font-weight:700}

  /* CTA (big book a call) */
  .cta{padding:130px 0 120px;text-align:center}
  .cta h2{margin:0 auto 18px;text-align:center;max-width:20ch}
  .cta-sub{font-family:Arial,sans-serif;font-size:18px;color:var(--gray);max-width:52ch;margin:0 auto 40px;letter-spacing:-0.01em;line-height:1.55}
  .cta-btn{display:inline-block;background:var(--teal);color:var(--navy);padding:26px 60px;
    font-family:"Bebas Neue",Impact,sans-serif;font-size:26px;letter-spacing:0.06em;text-transform:uppercase;
    text-decoration:none;transition:all 0.25s ease;border:2px solid var(--teal)}
  .cta-btn:hover{background:var(--aqua);border-color:var(--aqua);color:var(--navy)}

  /* FOOTER */
  footer.closing{background:var(--layer);color:var(--white);padding:80px 0 56px;position:relative;z-index:2;border-top:1px solid var(--hairline)}
  .closing .brand-para{font-family:Arial,sans-serif;font-weight:400;font-size:18px;line-height:1.6;max-width:62ch;margin-bottom:44px;color:var(--gray);letter-spacing:-0.01em}
  .closing .brand-para strong{color:var(--white);font-weight:700}
  .closing .label{font-family:Arial,sans-serif;font-weight:700;font-size:11px;text-transform:uppercase;letter-spacing:0.22em;color:var(--teal);margin-bottom:16px}
  .closing a{color:var(--white);text-decoration:none;border-bottom:1px solid rgba(255,255,255,0.28);transition:border-color 0.2s ease,color 0.2s ease}
  .closing a:hover{border-color:var(--teal);color:var(--teal)}
  .follow-list{list-style:none;font-size:17px}
  .follow-list li{padding:9px 0;display:flex;align-items:baseline;gap:14px}
  .follow-list li::before{content:"";width:7px;height:7px;background:var(--teal);flex-shrink:0;align-self:center}
  .colophon{margin-top:56px;padding-top:28px;border-top:1px solid var(--hairline);display:flex;justify-content:space-between;flex-wrap:wrap;gap:18px;
    font-family:Arial,sans-serif;font-weight:700;font-size:10px;text-transform:uppercase;letter-spacing:0.18em;color:var(--gray)}

  /* RESPONSIVE */
  @media (max-width:980px){.nav-links a:not(.nav-book){display:none}}
  @media (max-width:880px){
    .wrap{padding:0 22px}body{font-size:17px}
    .hero{padding:46px 0 56px}
    .hero-grid{grid-template-columns:1fr;gap:40px}
    .section-head{grid-template-columns:1fr;gap:16px;margin-bottom:38px}
    .body-grid{grid-template-columns:1fr;gap:0}
    .stat-row{grid-template-columns:1fr;border-top:none}
    .stat{border-right:none;border-bottom:1px solid var(--hairline)}
    .stat:last-child{border-bottom:none}
    .caps{grid-template-columns:1fr}
    .vs{grid-template-columns:1fr}
    .arrow-list li{grid-template-columns:36px 1fr;gap:18px}
    .pull{padding:78px 0}
    .warning{padding:46px 28px}
    .warning h3,.warning p{margin-left:0}
    .warning::before{position:relative;top:auto;left:auto;display:block;margin-bottom:12px}
    section{padding:58px 0}
    .cta{padding:76px 0 66px}
    .cta-btn{padding:22px 40px;font-size:22px}
    .nav-logo{height:38px}
  }
  .reveal{opacity:0;transform:translateY(18px);animation:rev 0.9s cubic-bezier(.2,.7,.2,1) forwards}
  .d1{animation-delay:0.05s}.d2{animation-delay:0.15s}.d3{animation-delay:0.3s}.d4{animation-delay:0.45s}
  @keyframes rev{to{opacity:1;transform:translateY(0)}}
</style>
</head>
<body>

<div class="wrap">
  <nav class="top">
    <img class="nav-logo" src="data:image/webp;base64,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" alt="Home Builder Marketers" />
    <div class="nav-links">
      <a href="https://homebuildermarketers.com/services/">Services</a>
      <a href="https://homebuildermarketers.com/home-builder-marketing-case-studies/">Case Studies</a>
      <a href="https://homebuildermarketers.com/packages/">Packages</a>
      <a href="https://homebuildermarketers.com/library-of-resources/">Resources</a>
      <a href="https://homebuildermarketers.com/contact-us/">Contact</a>
      <a class="nav-book label" href="https://homebuildermarketers.com/schedule-a-consultation/">Book Now</a>
    </div>
  </nav>
</div>

<header class="hero">
  <div class="wrap">
    <div class="eyebrow reveal d1"><span class="pulse"></span> Issue No. 05 · June 2026</div>
    <h1 class="headline reveal d2">
      The ten blue links are <span class="blocky">dead.</span>
    </h1>
    <div class="hero-grid">
      <p class="lede reveal d3">
        At Google I/O on <strong>May 19</strong>, Google made the biggest change to search since it launched. AI now answers the question at the top of the page and the list of links gets pushed down below it, or skipped entirely. AI Overviews already reach <strong>2.5 billion people a month</strong>. The way a homeowner finds a builder online is not what it was a year ago, and most builders have no idea it already happened.
      </p>
      <div class="meta-card reveal d4">
        <h4>Brief</h4>
        <div class="meta-row"><span>Event</span><span>Google I/O 2026</span></div>
        <div class="meta-row"><span>Date</span><span>May 19, 2026</span></div>
        <div class="meta-row"><span>The shift</span><span>Links to AI answers</span></div>
        <div class="meta-row"><span>What it needs</span><span>GEO, not just SEO</span></div>
        <div class="meta-row"><span>Reading Time</span><span>6 min</span></div>
      </div>
    </div>
  </div>
</header>

<div class="marquee">
  <div class="marquee-track">
    <span>
      AI Overviews <span class="star">&#10022;</span>
      AI Mode <span class="star">&#10022;</span>
      Search Agents <span class="star">&#10022;</span>
      Generative Engine Optimization <span class="star">&#10022;</span>
      Zero Click Search <span class="star">&#10022;</span>
      Being The Recommendation <span class="star">&#10022;</span>
      AI Overviews <span class="star">&#10022;</span>
      AI Mode <span class="star">&#10022;</span>
      Search Agents <span class="star">&#10022;</span>
      Generative Engine Optimization <span class="star">&#10022;</span>
      Zero Click Search <span class="star">&#10022;</span>
      Being The Recommendation <span class="star">&#10022;</span>
    </span>
  </div>
</div>

<section>
  <div class="wrap">
    <div class="section-head">
      <div class="section-num">01 / The Drop</div>
      <h2>What Google <em>actually</em> announced.</h2>
    </div>
    <div class="body-grid">
      <div></div>
      <div class="body-content">
        <p>On May 19th at Google I/O, Sundar Pichai walked on stage and confirmed what the search world had been bracing for. <strong>AI Overviews now reach 2.5 billion people a month.</strong> AI Mode, the full conversational version of search, crossed a billion users in its first year. And the two are merging into one AI first search experience that rolls out worldwide.</p>
        <p>Google also introduced search agents that go research the web for you in the background, no clicks needed. The reporting out of the keynote put it bluntly. Links are becoming an afterthought.</p>
        <p>Google did not delete the blue links overnight. What it did is quieter and more permanent. It is absorbing classic search into AI, one piece at a time, until the answer shows up before anyone scrolls. For a builder, that answer is now the first impression. Not your website. Not your reviews page. The answer.</p>
      </div>
    </div>
  </div>
</section>

<div class="stat-strip">
  <div class="wrap">
    <div class="section-head">
      <div class="section-num">02 / Numbers</div>
      <h2>The shift in <em>three</em> numbers.</h2>
    </div>
    <div class="body-grid">
      <div></div>
      <div class="body-content">
        <p>Pulled from Google's own keynote and the latest independent search studies. No spin.</p>
      </div>
    </div>
    <div class="stat-row">
      <div class="stat">
        <div class="stat-num">2.5B</div>
        <div class="stat-label">Monthly AI Overviews users · 2026</div>
      </div>
      <div class="stat">
        <div class="stat-num">58%</div>
        <div class="stat-label">CTR drop on the top result when an AI Overview shows (Ahrefs)</div>
      </div>
      <div class="stat">
        <div class="stat-num">48%</div>
        <div class="stat-label">Of Google searches now show an AI Overview</div>
      </div>
    </div>
  </div>
</div>

<section>
  <div class="wrap">
    <div class="section-head">
      <div class="section-num">03 / What You Do Now</div>
      <h2>Four moves while everyone else <em>waits</em>.</h2>
    </div>
    <div class="caps">
      <div class="cap">
        <span class="cap-num">MOVE_01</span>
        <div class="cap-icon">A</div>
        <h3>Become the name the AI gives.</h3>
        <p>When a homeowner asks "who builds custom homes in my area" or "is it worth building versus buying," an AI answers with a short list of names. Your only job now is to be one of those names. That is the whole game. Ranking second on page one means nothing if the AI never shows page one.</p>
      </div>
      <div class="cap">
        <span class="cap-num">MOVE_02</span>
        <div class="cap-icon">W</div>
        <h3>Write what the AI can lift.</h3>
        <p>AI pulls clean, direct answers. Your site needs the real questions your buyers ask, answered in plain language, near the top of the page. Cost to build. Timeline. The process from lot to keys. Answer first, then expand. Buried answers do not get quoted.</p>
      </div>
      <div class="cap">
        <span class="cap-num">MOVE_03</span>
        <div class="cap-icon">T</div>
        <h3>Win the signals AI trusts.</h3>
        <p>AI does not just read your website. It grounds its answers in what the rest of the web says about you. Consistent listings, real reviews, mentions on local sites, a clean footprint everywhere it looks. The builders the AI trusts are the ones it sees confirmed in more than one place.</p>
      </div>
      <div class="cap">
        <span class="cap-num">MOVE_04</span>
        <div class="cap-icon">S</div>
        <h3>Watch what the AI says about you.</h3>
        <p>Ask the AI about your company and your market the way a homeowner would. See what it says. See who it names instead of you. That is your real scoreboard now, and almost no builder is checking it. The ones who do get to fix the gap before their competitors notice it exists.</p>
      </div>
    </div>
  </div>
</section>

<section class="pull">
  <div class="wrap">
    <div class="pull-quote">
      Stop optimizing for the click. Start being the answer.
    </div>
    <div class="pull-attr">Field Note · 2026</div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <div class="section-num">04 / The Shift</div>
      <h2>The old game, <em>and</em> the new one.</h2>
    </div>
    <div class="vs">
      <div class="before">
        <div class="label">The Old Game</div>
        <h3>Rank number one on Google, earn the click, win the lead. Search engine optimization was a fight over position on a page of links.</h3>
      </div>
      <div class="after">
        <div class="label">The New Game</div>
        <h3>Be the brand the AI recommends before the homeowner scrolls. If the answer does not name you, the page of links underneath it barely matters.</h3>
      </div>
    </div>
  </div>
</section>

<section>
  <div class="wrap">
    <div class="section-head">
      <div class="section-num">05 / The Stakes</div>
      <h2>The next ninety days <em>decide</em> it.</h2>
    </div>
    <ol class="arrow-list">
      <li>
        <div class="arrow">&#8594;</div>
        <div>
          <h4>The builders who move now own the next decade of search.</h4>
          <p>This is the window where being early actually counts. The builders who build their presence into AI search over the next quarter become the default answer in their market. That position is hard to take back once someone holds it.</p>
        </div>
      </li>
      <li>
        <div class="arrow">&#8594;</div>
        <div>
          <h4>The ones who wait watch their leads dry up and never know why.</h4>
          <p>Their traffic slips month over month. Their cost per lead creeps up. They blame the season, the market, the economy. The real reason is that the AI stopped sending them anyone and they were not watching the one number that mattered.</p>
        </div>
      </li>
      <li>
        <div class="arrow">&#8594;</div>
        <div>
          <h4>Nearly sixty percent of searches now end without a single click.</h4>
          <p>People get the answer and move on. That is not a trend coming someday. That is the search results page today. Every month you treat search like it is still 2022, you fall further behind the builders who adjusted.</p>
        </div>
      </li>
    </ol>
  </div>
</section>

<section style="padding:0">
  <div class="wrap">
    <div class="warning">
      <h3>This is not a someday problem.</h3>
      <p>We talk to builders every week who are still pouring money into a website strategy built for a version of Google that no longer exists. They are optimizing to rank for a click that fewer and fewer people make. The shift already happened. The only question is whether you adjust before your competitors do or after.</p>
      <p>You do not need to panic and you do not need to burn down your website. You need to widen the play. Keep what works, and start building the presence that gets you named inside the answer. That is the work our team is doing on builder accounts right now.</p>
    </div>
  </div>
</section>

<section class="cta">
  <div class="wrap">
    <h2>If you're <em>interested</em>, book a call.</h2>
    <div class="cta-sub">Fifteen minutes. We will show you exactly where you stand in AI search right now and what to fix first so your name is the one that shows up.</div>
    <a href="https://homebuildermarketers.com/schedule-a-consultation/" class="cta-btn">Book A Call Here</a>
  </div>
</section>

<footer class="closing">
  <div class="wrap">
    <p class="brand-para">
      <strong>Home Builder Marketers</strong> helps custom home builders, remodelers, and contractors sell more homes through better marketing, better creative, and better systems. Over 150 builders served and more than 268 million dollars in revenue generated across the US and Canada.
    </p>

    <div class="label">Follow us everywhere</div>
    <ul class="follow-list">
      <li><a href="https://facebook.com/homebuildermarketers">Facebook · /homebuildermarketers</a></li>
      <li><a href="https://instagram.com/homebuildermarketers">Instagram · @homebuildermarketers</a></li>
      <li><a href="https://tiktok.com/@homebuildermarketers">TikTok · @homebuildermarketers</a></li>
      <li><a href="https://youtube.com/@HomeBuilderMarketers">YouTube · @HomeBuilderMarketers</a></li>
      <li><a href="https://linkedin.com/company/home-builder-marketers">LinkedIn · linkedin.com/company/home-builder-marketers</a></li>
    </ul>

    <div class="colophon">
      <span>&#169; 2026 Home Builder Marketers · All Rights Reserved</span>
      <span>Marketers You Can Trust</span>
    </div>
  </div>
</footer>

</body>
</html>