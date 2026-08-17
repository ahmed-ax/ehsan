
<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover" />
  <meta name="theme-color" content="#2b2825" />
  <meta name="description" content="جمعية الإحسان للخدمات الاجتماعية — تجربة رقمية رسمية تضع الأثر والثقة وسهولة التبرع في الواجهة." />
  <title>جمعية الإحسان للخدمات الاجتماعية</title>
  <style>
    :root{
      --brand:#ff7c19;
      --brand-deep:#cd3e01;
      --brand-ink:#7a2600;
      --brand-soft:#fff3e9;
      --brand-wash:#fff9f4;
      --ink:#25211e;
      --ink-2:#4d4741;
      --muted:#7d756d;
      --line:#e7ded5;
      --line-dark:rgba(255,255,255,.12);
      --paper:#fff;
      --paper-2:#f8f5f1;
      --paper-3:#efe9e2;
      --night:#2b2825;
      --night-2:#34302c;
      --shadow-sm:0 10px 26px rgba(50,38,28,.07);
      --shadow:0 28px 72px rgba(50,38,28,.13);
      --shadow-brand:0 18px 36px rgba(205,62,1,.18);
      --radius-sm:10px;
      --radius:18px;
      --radius-lg:28px;
      --container:min(1240px, calc(100% - 48px));
    }

    *{box-sizing:border-box}
    html{scroll-behavior:smooth;scroll-padding-top:96px}
    body{
      margin:0;
      background:var(--paper);
      color:var(--ink);
      font-family:"Noto Sans Arabic","Segoe UI",Tahoma,Arial,sans-serif;
      line-height:1.8;
      text-rendering:optimizeLegibility;
      -webkit-font-smoothing:antialiased;
    }
    body.menu-open,body.modal-open{overflow:hidden}
    img{display:block;max-width:100%}
    a{color:inherit;text-decoration:none}
    button,input,select{font:inherit}
    button{color:inherit}
    .container{width:var(--container);margin-inline:auto}
    .section{padding:112px 0}
    .sr-only{position:absolute!important;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border:0}
    .kicker{display:inline-flex;align-items:center;gap:10px;color:var(--brand-deep);font-size:12px;font-weight:900;letter-spacing:.02em;margin-bottom:16px}
    .kicker:before{content:"";width:32px;height:2px;background:var(--brand)}
    .kicker.on-dark{color:#ffbd8d}.kicker.on-dark:before{background:#ff9a50}
    h1,h2,h3,p{margin-top:0}
    h1{font-size:clamp(42px,5.3vw,76px);line-height:1.14;letter-spacing:-.045em;margin-bottom:24px}
    h2{font-size:clamp(32px,3.7vw,52px);line-height:1.25;letter-spacing:-.035em;margin-bottom:18px}
    h3{font-size:22px;line-height:1.45;margin-bottom:10px}
    .lead{font-size:18px;color:var(--ink-2);max-width:720px}
    .muted{color:var(--muted)}
    .btn{min-height:52px;border-radius:9px;padding:0 22px;border:1px solid transparent;display:inline-flex;align-items:center;justify-content:center;gap:9px;font-weight:900;font-size:14px;cursor:pointer;transition:transform .2s ease,box-shadow .2s ease,background .2s ease,border-color .2s ease;color:inherit;background:transparent}
    .btn:hover{transform:translateY(-2px)}
    .btn-primary{background:var(--brand-deep);color:#fff;box-shadow:var(--shadow-brand)}
    .btn-primary:hover{background:#b93803}
    .btn-outline{background:#fff;border-color:var(--line);color:var(--ink)}
    .btn-outline:hover{border-color:#d4c5b8;box-shadow:var(--shadow-sm)}
    .btn-white{background:#fff;color:var(--night);box-shadow:0 12px 30px rgba(0,0,0,.16)}
    .btn-link{min-height:auto;padding:0;color:var(--brand-deep);border:0;border-radius:0}
    .btn-link:hover{transform:none;gap:13px}
    .arrow{width:19px;height:19px;transition:transform .2s ease}
    .btn:hover .arrow,.text-link:hover .arrow{transform:translateX(-4px)}
    .icon{width:21px;height:21px;display:block}

    .topbar{background:var(--night);color:#e8e2dc;border-bottom:1px solid rgba(255,255,255,.08);font-size:11px}
    .topbar-inner{min-height:39px;display:flex;justify-content:space-between;align-items:center;gap:20px}
    .topbar-group{display:flex;align-items:center;gap:22px;flex-wrap:wrap}
    .topbar a{transition:color .2s ease}.topbar a:hover{color:#fff}
    .top-badge{display:inline-flex;align-items:center;gap:7px;color:#f2c4a3}
    .top-badge:before{content:"";width:5px;height:5px;border-radius:50%;background:var(--brand)}

    .site-header{position:sticky;top:0;z-index:70;background:rgba(255,255,255,.94);backdrop-filter:blur(18px);border-bottom:1px solid rgba(231,222,213,.8)}
    .nav{height:88px;display:grid;grid-template-columns:auto 1fr auto;align-items:center;gap:32px}
    .brand{display:flex;align-items:center;gap:12px;min-width:245px}
    .brand img{width:50px;height:50px;object-fit:contain}
    .brand-text{line-height:1.3}.brand-text b{display:block;font-size:17px}.brand-text span{display:block;font-size:10px;color:var(--muted);margin-top:3px}
    .nav-links{display:flex;align-items:center;justify-content:center;gap:2px}
    .nav-links a{padding:31px 13px;font-size:13px;font-weight:800;position:relative;color:#403a35}
    .nav-links a:after{content:"";position:absolute;right:13px;left:100%;bottom:20px;height:2px;background:var(--brand);transition:left .22s ease}
    .nav-links a:hover:after,.nav-links a.active:after{left:13px}
    .nav-actions{display:flex;align-items:center;gap:9px;justify-self:end}
    .icon-btn{width:44px;height:44px;border-radius:9px;border:1px solid var(--line);background:#fff;display:grid;place-items:center;cursor:pointer;transition:.2s ease}
    .icon-btn:hover{border-color:#d2c5ba;box-shadow:var(--shadow-sm)}
    .menu-btn{display:none}
    .mobile-drawer{display:none}
    .nav-progress{position:absolute;right:0;bottom:-1px;height:2px;width:0;background:var(--brand-deep);z-index:2}

    .hero{position:relative;overflow:hidden;background:linear-gradient(180deg,#fff 0%,#fffaf6 74%,#f7f3ef 100%)}
    .hero:before{content:"";position:absolute;inset:0;background-image:linear-gradient(rgba(66,52,41,.035) 1px,transparent 1px),linear-gradient(90deg,rgba(66,52,41,.035) 1px,transparent 1px);background-size:56px 56px;mask-image:linear-gradient(to bottom,rgba(0,0,0,.55),transparent 78%);pointer-events:none}
    .hero-grid{min-height:720px;display:grid;grid-template-columns:.92fr 1.08fr;align-items:center;gap:76px;padding:72px 0 106px;position:relative;z-index:1}
    .hero-copy{max-width:630px}
    .hero-copy h1 span{color:var(--brand-deep)}
    .hero-copy .lead{font-size:18px;line-height:2;margin-bottom:32px}
    .hero-actions{display:flex;align-items:center;gap:12px;flex-wrap:wrap;margin-bottom:34px}
    .hero-trust{display:flex;align-items:center;gap:24px;flex-wrap:wrap;color:var(--muted);font-size:12px}
    .trust-line{display:flex;align-items:center;gap:8px}
    .trust-mark{width:22px;height:22px;border-radius:50%;display:grid;place-items:center;background:var(--brand-soft);color:var(--brand-deep)}
    .hero-visual{position:relative;min-height:560px}
    .hero-photo{position:absolute;inset:0 72px 38px 0;border-radius:3px;overflow:hidden;box-shadow:var(--shadow)}
    .hero-photo img{width:100%;height:100%;object-fit:cover}
    .hero-photo:after{content:"";position:absolute;inset:0;background:linear-gradient(180deg,transparent 48%,rgba(26,22,19,.42))}
    .hero-frame-line{position:absolute;inset:34px 22px 0 108px;border:1px solid rgba(205,62,1,.42);pointer-events:none}
    .hero-card{position:absolute;right:0;top:46px;width:178px;background:var(--night);color:#fff;padding:22px 20px;box-shadow:0 22px 48px rgba(29,24,20,.2)}
    .hero-card strong{display:block;font-size:37px;line-height:1.05;color:#ffab69;margin-bottom:8px}.hero-card span{font-size:11px;color:#d3cbc4}
    .hero-caption{position:absolute;left:0;bottom:0;width:min(330px,60%);background:#fff;border-top:3px solid var(--brand);padding:22px 24px;box-shadow:var(--shadow-sm)}
    .hero-caption b{display:block;font-size:16px;margin-bottom:4px}.hero-caption p{margin:0;font-size:11px;color:var(--muted);line-height:1.8}
    .hero-seal{position:absolute;left:42px;top:38px;width:92px;height:92px;border-radius:50%;background:var(--brand-deep);color:white;display:grid;place-items:center;text-align:center;box-shadow:0 18px 38px rgba(205,62,1,.24);font-size:10px;line-height:1.45;transform:rotate(-7deg)}
    .hero-seal b{display:block;font-size:20px}

    .donate-dock-wrap{position:relative;z-index:5;margin-top:-44px}
    .donate-dock{background:#fff;border:1px solid #eadfd5;box-shadow:0 24px 60px rgba(55,42,31,.13);padding:18px;display:grid;grid-template-columns:1.05fr 1.15fr 1fr auto;gap:14px;align-items:end;border-radius:14px}
    .dock-intro{padding:3px 8px 3px 4px}.dock-intro b{display:block;font-size:18px;margin-bottom:2px}.dock-intro span{font-size:11px;color:var(--muted)}
    .field label{display:block;font-size:10px;font-weight:900;color:var(--muted);margin-bottom:7px}
    .field select,.field input{width:100%;height:50px;border:1px solid var(--line);background:#fff;border-radius:8px;padding:0 13px;color:var(--ink);outline:none;transition:.2s ease}
    .field select:focus,.field input:focus{border-color:var(--brand);box-shadow:0 0 0 3px rgba(255,124,25,.1)}
    .amount-wrap{display:flex;align-items:center;gap:8px}.amount-wrap .field{flex:1}
    .amount-chip{height:50px;border:1px solid var(--line);background:var(--paper-2);border-radius:8px;padding:0 12px;display:grid;place-items:center;font-size:11px;font-weight:900;color:var(--muted)}

    .section-head{display:flex;align-items:end;justify-content:space-between;gap:36px;margin-bottom:46px}
    .section-head>div:first-child{max-width:760px}.section-head p{margin:0;color:var(--muted);max-width:520px}
    .section-head.compact{align-items:center}

    .intro-grid{display:grid;grid-template-columns:1.02fr .98fr;gap:78px;align-items:center}
    .intro-visual{position:relative;min-height:520px;padding:22px 0 0 24px}
    .intro-visual:before{content:"";position:absolute;right:-24px;top:0;width:72%;height:74%;border:1px solid rgba(205,62,1,.45);z-index:-1}
    .intro-visual img{width:100%;height:500px;object-fit:cover;box-shadow:var(--shadow-sm)}
    .intro-note{position:absolute;right:-12px;bottom:32px;background:#fff;padding:20px 22px;border-right:4px solid var(--brand-deep);box-shadow:var(--shadow-sm);max-width:260px;font-size:12px;color:var(--ink-2)}
    .intro-copy p{font-size:17px;color:var(--ink-2)}
    .timeline{margin:30px 0 34px;border-top:1px solid var(--line);border-bottom:1px solid var(--line);display:grid;grid-template-columns:1fr 1fr}
    .timeline-item{padding:22px 0;position:relative}.timeline-item+ .timeline-item{border-right:1px solid var(--line);padding-right:24px;margin-right:24px}
    .timeline-item strong{display:block;font-size:28px;color:var(--brand-deep);line-height:1.2;margin-bottom:5px}.timeline-item span{font-size:11px;color:var(--muted)}
    .signature-row{display:flex;align-items:center;gap:16px;flex-wrap:wrap}

    .programs{background:var(--night);color:#fff;position:relative;overflow:hidden}
    .programs:before{content:"";position:absolute;left:-190px;top:-190px;width:540px;height:540px;border:1px solid rgba(255,255,255,.05);border-radius:50%;box-shadow:0 0 0 70px rgba(255,255,255,.025),0 0 0 140px rgba(255,255,255,.018)}
    .programs h2{color:#fff}.programs .section-head p{color:#c5beb7}
    .program-grid{display:grid;grid-template-columns:repeat(3,1fr);border:1px solid rgba(255,255,255,.12);position:relative;z-index:1}
    .program-card{padding:42px 36px;min-height:330px;border-left:1px solid rgba(255,255,255,.12);display:flex;flex-direction:column;position:relative;overflow:hidden;transition:background .2s ease}
    .program-card:last-child{border-left:0}.program-card:hover{background:rgba(255,255,255,.035)}
    .program-no{font-size:11px;color:#ffb57b;font-weight:900;margin-bottom:42px}.program-icon{width:56px;height:56px;border:1px solid rgba(255,124,25,.45);display:grid;place-items:center;color:#ff9c51;margin-bottom:26px}
    .program-card h3{font-size:24px}.program-card p{font-size:13px;color:#bdb6af;margin-bottom:26px}.program-card .text-link{margin-top:auto;color:#ffc89d;font-size:12px;font-weight:900;display:inline-flex;align-items:center;gap:8px}
    .program-card:after{content:"";position:absolute;width:130px;height:130px;left:-88px;bottom:-88px;border:1px solid rgba(255,124,25,.24);transform:rotate(45deg)}

    .donations{background:#fff}
    .donation-feature{display:grid;grid-template-columns:1.06fr .94fr;border:1px solid var(--line);margin-bottom:20px;min-height:360px;overflow:hidden;background:var(--brand-wash)}
    .donation-feature-copy{padding:44px;display:flex;flex-direction:column;justify-content:center}
    .donation-feature-tag{display:inline-flex;align-items:center;align-self:flex-start;background:#fff;border:1px solid var(--line);padding:6px 10px;border-radius:999px;font-size:10px;color:var(--brand-deep);font-weight:900;margin-bottom:20px}
    .donation-feature h3{font-size:32px;margin-bottom:10px}.donation-feature p{color:var(--muted);max-width:600px}.feature-amount{display:flex;align-items:end;gap:8px;margin:12px 0 22px}.feature-amount strong{font-size:42px;color:var(--brand-deep);line-height:1}.feature-amount span{font-size:12px;color:var(--muted)}
    .donation-feature-visual{background:var(--night);color:#fff;position:relative;display:flex;align-items:flex-end;padding:34px;overflow:hidden}
    .donation-feature-visual:before{content:"";position:absolute;inset:0;background:radial-gradient(circle at 28% 25%,rgba(255,124,25,.24),transparent 32%),linear-gradient(135deg,transparent,rgba(255,255,255,.03))}
    .visual-quote{position:relative;z-index:1;max-width:300px}.visual-quote b{display:block;font-size:25px;line-height:1.6;margin-bottom:10px}.visual-quote span{font-size:11px;color:#c9c1ba}
    .donation-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
    .donation-card{border:1px solid var(--line);background:#fff;padding:26px;min-height:284px;display:flex;flex-direction:column;transition:.22s ease;position:relative;overflow:hidden}
    .donation-card:hover{transform:translateY(-5px);box-shadow:var(--shadow-sm);border-color:#dacbbd}.donation-card:before{content:"";position:absolute;right:0;top:0;width:3px;height:0;background:var(--brand);transition:height .22s ease}.donation-card:hover:before{height:100%}
    .card-top{display:flex;align-items:center;justify-content:space-between;margin-bottom:24px}.card-icon{width:48px;height:48px;border-radius:50%;background:var(--brand-soft);display:grid;place-items:center;color:var(--brand-deep)}.pill{font-size:10px;color:var(--muted);border:1px solid var(--line);border-radius:999px;padding:5px 9px;background:var(--paper)}
    .donation-card h3{font-size:21px}.donation-card p{font-size:12px;color:var(--muted);margin-bottom:24px}.card-bottom{margin-top:auto;border-top:1px solid var(--line);padding-top:18px;display:flex;align-items:end;justify-content:space-between;gap:14px}.card-price strong{font-size:26px;color:var(--brand-deep);line-height:1}.card-price span{font-size:10px;color:var(--muted);margin-right:4px}.text-link{font-size:11px;color:var(--brand-deep);font-weight:900;display:inline-flex;align-items:center;gap:6px}
    .donation-actions{margin-top:34px;display:flex;justify-content:center}

    .impact{background:var(--paper-2);border-top:1px solid var(--line);border-bottom:1px solid var(--line)}
    .impact-layout{display:grid;grid-template-columns:.72fr 1.28fr;gap:56px;align-items:start}
    .impact-intro{position:sticky;top:130px}.impact-intro p{color:var(--muted);font-size:14px}.impact-year{display:inline-flex;align-items:center;gap:10px;margin-top:16px;font-size:11px;color:var(--brand-deep);font-weight:900}.impact-year:before{content:"";width:7px;height:7px;border-radius:50%;background:var(--brand)}
    .stats-grid{display:grid;grid-template-columns:1fr 1fr;border-top:1px solid var(--line);border-right:1px solid var(--line);background:#fff}
    .stat{padding:34px 30px;border-left:1px solid var(--line);border-bottom:1px solid var(--line);min-height:170px;display:flex;flex-direction:column;justify-content:space-between;position:relative;overflow:hidden}.stat:after{content:"";position:absolute;left:18px;bottom:16px;width:34px;height:34px;border-left:1px solid rgba(205,62,1,.17);border-bottom:1px solid rgba(205,62,1,.17)}
    .stat strong{font-size:36px;color:var(--brand-deep);line-height:1.15;font-variant-numeric:tabular-nums}.stat span{font-size:12px;color:var(--muted)}.stat.cost strong{font-size:28px}

    .journeys{background:#fff}
    .journey-grid{display:grid;grid-template-columns:repeat(4,1fr);gap:14px}
    .journey{background:var(--paper-2);border:1px solid var(--line);padding:26px;min-height:245px;display:flex;flex-direction:column;transition:.2s ease}
    .journey:hover{background:#fff;box-shadow:var(--shadow-sm);transform:translateY(-3px)}.journey-icon{width:46px;height:46px;display:grid;place-items:center;border:1px solid #d9cbc0;background:#fff;color:var(--brand-deep);margin-bottom:24px}.journey h3{font-size:18px}.journey p{font-size:11px;color:var(--muted)}.journey .text-link{margin-top:auto}

    .media{background:linear-gradient(180deg,#fff 0%,#fbf9f6 100%)}
    .media-grid{display:grid;grid-template-columns:1.15fr .85fr .85fr;gap:18px}
    .news{border:1px solid var(--line);background:#fff;overflow:hidden;display:flex;flex-direction:column;min-height:100%}.news-img{height:220px;overflow:hidden;background:var(--paper-3)}.news.featured .news-img{height:325px}.news-img img{width:100%;height:100%;object-fit:cover;transition:transform .35s ease}.news:hover .news-img img{transform:scale(1.03)}.news-body{padding:22px;display:flex;flex-direction:column;flex:1}.news-meta{font-size:10px;color:var(--brand-deep);font-weight:900;margin-bottom:10px}.news h3{font-size:18px}.news.featured h3{font-size:24px}.news p{font-size:12px;color:var(--muted)}.news .text-link{margin-top:auto}

    .governance{background:#fff;padding-top:0}
    .gov-shell{display:grid;grid-template-columns:1fr .78fr;min-height:470px;border:1px solid #e9ddd2;overflow:hidden;background:linear-gradient(135deg,#fffaf5,#fff)}
    .gov-copy{padding:58px}.gov-copy p{color:var(--ink-2);max-width:640px}.gov-search{margin:26px 0 22px;display:flex;border:1px solid var(--line);background:#fff;max-width:600px;border-radius:9px;overflow:hidden}.gov-search input{border:0;outline:none;flex:1;min-width:0;padding:0 16px;height:52px;background:transparent}.gov-search button{width:54px;border:0;border-right:1px solid var(--line);background:#fff;display:grid;place-items:center;cursor:pointer;color:var(--brand-deep)}
    .gov-links{display:grid;grid-template-columns:1fr 1fr;gap:10px}.gov-link{background:#fff;border:1px solid var(--line);padding:13px 14px;font-size:11px;font-weight:900;display:flex;justify-content:space-between;align-items:center;transition:.2s ease}.gov-link:hover{border-color:#d4c5b8;transform:translateY(-1px)}
    .gov-visual{background:var(--night);color:#fff;padding:46px;position:relative;overflow:hidden;display:flex;flex-direction:column;justify-content:space-between}.gov-visual:before,.gov-visual:after{content:"";position:absolute;width:230px;height:230px;border:1px solid rgba(255,124,25,.32);transform:rotate(45deg)}.gov-visual:before{left:-120px;top:-120px}.gov-visual:after{right:-140px;bottom:-120px}.gov-year{position:relative;z-index:1}.gov-year strong{display:block;font-size:78px;line-height:1;color:#ff9c51}.gov-year span{font-size:11px;color:#c4bdb6}.gov-quote{position:relative;z-index:1;font-size:20px;line-height:1.8;max-width:320px}.gov-badge{position:relative;z-index:1;border-top:1px solid rgba(255,255,255,.14);padding-top:18px;font-size:10px;color:#a9a19a}

    .closing{background:var(--brand-deep);color:#fff;padding:46px 0}
    .closing-inner{display:flex;align-items:center;justify-content:space-between;gap:36px}.closing h2{font-size:30px;margin:0;color:#fff}.closing p{margin:6px 0 0;color:#f4c8b2;font-size:12px}.closing-actions{display:flex;gap:10px;flex-wrap:wrap}

    .footer{background:#211f1d;color:#fff;padding:62px 0 26px}
    .footer-grid{display:grid;grid-template-columns:1.25fr .7fr .7fr .95fr;gap:48px;padding-bottom:44px;border-bottom:1px solid rgba(255,255,255,.11)}
    .footer-brand{display:flex;align-items:center;gap:12px;margin-bottom:20px}.footer-brand img{width:54px;height:54px}.footer-brand b{font-size:17px}.footer p{font-size:12px;color:#bdb6af}.footer-license{color:#f1b88e!important}.footer h4{font-size:13px;margin:0 0 17px}.footer-links,.footer-contact{display:grid;gap:9px;font-size:12px;color:#c6bfb8}.footer-links a:hover,.footer-contact a:hover{color:#fff}.socials{display:flex;gap:8px;margin-top:20px}.social{width:36px;height:36px;border:1px solid rgba(255,255,255,.14);display:grid;place-items:center;font-size:10px;color:#d4ccc5}.footer-bottom{display:flex;align-items:center;justify-content:space-between;gap:20px;padding-top:22px;color:#8f8882;font-size:10px}

    .mobile-donate{display:none}
    .search-modal{position:fixed;inset:0;z-index:100;background:rgba(28,24,21,.72);backdrop-filter:blur(9px);padding:22px;opacity:0;visibility:hidden;transition:.2s ease}.search-modal.open{opacity:1;visibility:visible}.search-panel{width:min(760px,100%);margin:11vh auto 0;background:#fff;box-shadow:0 30px 90px rgba(0,0,0,.26);padding:28px;border-radius:14px}.search-top{display:flex;align-items:center;justify-content:space-between;margin-bottom:18px}.search-top b{font-size:18px}.search-box{display:flex;border:1px solid var(--line);height:58px}.search-box input{flex:1;min-width:0;border:0;outline:none;padding:0 16px}.search-box button{width:58px;border:0;border-right:1px solid var(--line);background:#fff;color:var(--brand-deep);display:grid;place-items:center}.search-hints{display:flex;gap:8px;flex-wrap:wrap;margin-top:16px}.search-hints span{font-size:10px;background:var(--paper-2);border:1px solid var(--line);padding:6px 9px;border-radius:999px;color:var(--muted)}
    .toast{position:fixed;left:24px;bottom:24px;z-index:120;background:var(--night);color:#fff;padding:14px 16px;box-shadow:var(--shadow);border-right:3px solid var(--brand);min-width:270px;max-width:420px;transform:translateY(20px);opacity:0;pointer-events:none;transition:.25s ease;font-size:12px}.toast.show{transform:translateY(0);opacity:1}.toast b{display:block;margin-bottom:3px;color:#ffb277}

    @media (max-width:1100px){
      .nav-links{display:none}.menu-btn{display:grid}.brand{min-width:auto}.hero-grid{gap:40px;grid-template-columns:.92fr 1.08fr}.hero-photo{inset:0 48px 38px 0}.hero-card{right:-5px}.donate-dock{grid-template-columns:1fr 1fr}.dock-intro{grid-column:1/-1}.intro-grid{gap:46px}.media-grid{grid-template-columns:1fr 1fr}.news.featured{grid-column:1/-1;display:grid;grid-template-columns:1.1fr .9fr}.news.featured .news-img{height:100%;min-height:320px}.journey-grid{grid-template-columns:1fr 1fr}.footer-grid{grid-template-columns:1.15fr .85fr .85fr}.footer-grid>div:last-child{grid-column:1/-1}
      .mobile-drawer{position:fixed;inset:128px 0 auto 0;z-index:69;background:#fff;border-bottom:1px solid var(--line);box-shadow:0 24px 60px rgba(0,0,0,.12);padding:18px 24px 24px;display:grid;gap:1px;opacity:0;visibility:hidden;transform:translateY(-8px);transition:.2s ease}.mobile-drawer.open{opacity:1;visibility:visible;transform:none}.mobile-drawer a{padding:13px 4px;border-bottom:1px solid var(--line);font-size:13px;font-weight:900}.mobile-drawer .drawer-action{margin-top:12px;border:0;background:var(--brand-deep);color:#fff;text-align:center;border-radius:8px}
    }
    @media (max-width:780px){
      :root{--container:min(100% - 28px,1240px)}
      html{scroll-padding-top:76px}.topbar{display:none}.nav{height:74px;gap:12px}.site-header{top:0}.mobile-drawer{inset:74px 0 auto 0}.brand img{width:42px;height:42px}.brand-text b{font-size:14px}.brand-text span{display:none}.nav-actions .btn-primary{display:none}.nav-actions{gap:6px}.icon-btn{width:40px;height:40px}
      h1{font-size:clamp(38px,11.5vw,58px)}h2{font-size:34px}.section{padding:78px 0}
      .hero-grid{grid-template-columns:1fr;padding:48px 0 84px;min-height:auto;gap:42px}.hero-copy{max-width:none}.hero-copy .lead{font-size:15px}.hero-visual{min-height:430px}.hero-photo{inset:0 0 26px 0}.hero-frame-line{display:none}.hero-card{right:10px;top:20px;width:140px;padding:17px}.hero-card strong{font-size:28px}.hero-caption{left:10px;bottom:0;width:260px}.hero-seal{display:none}.hero-trust{gap:12px}.trust-line{font-size:10px}
      .donate-dock-wrap{margin-top:-32px}.donate-dock{grid-template-columns:1fr;padding:16px}.dock-intro{grid-column:auto}.donate-dock .btn{width:100%}
      .section-head{align-items:start;flex-direction:column;margin-bottom:32px}.section-head.compact{align-items:start}.section-head .btn-link{padding:0}
      .intro-grid{grid-template-columns:1fr;gap:38px}.intro-visual{order:-1;min-height:390px;padding:16px 0 0 16px}.intro-visual img{height:380px}.intro-note{right:12px;bottom:18px}.timeline{grid-template-columns:1fr 1fr}
      .program-grid{grid-template-columns:1fr}.program-card{border-left:0;border-bottom:1px solid rgba(255,255,255,.12);min-height:280px}.program-card:last-child{border-bottom:0}
      .donation-feature{grid-template-columns:1fr}.donation-feature-copy{padding:30px 24px}.donation-feature-visual{min-height:260px}.donation-grid{grid-template-columns:1fr}.donation-card{min-height:250px}
      .impact-layout{grid-template-columns:1fr;gap:30px}.impact-intro{position:static}.stats-grid{grid-template-columns:1fr 1fr}.stat{min-height:150px;padding:24px 18px}.stat strong{font-size:30px}.stat.cost strong{font-size:22px}
      .journey-grid{grid-template-columns:1fr}.journey{min-height:210px}
      .media-grid{grid-template-columns:1fr}.news.featured{grid-column:auto;display:flex}.news.featured .news-img{height:240px;min-height:0}.news-img{height:220px}.news.featured h3{font-size:21px}
      .gov-shell{grid-template-columns:1fr}.gov-copy{padding:32px 24px}.gov-links{grid-template-columns:1fr}.gov-visual{min-height:330px;padding:34px 24px}
      .closing-inner{align-items:start;flex-direction:column}.closing h2{font-size:25px}.closing-actions{width:100%}.closing-actions .btn{flex:1}
      .footer-grid{grid-template-columns:1fr 1fr;gap:30px}.footer-grid>div:first-child,.footer-grid>div:last-child{grid-column:1/-1}.footer-bottom{align-items:start;flex-direction:column}
      .mobile-donate{display:flex;position:fixed;right:12px;left:12px;bottom:12px;z-index:65;background:rgba(255,255,255,.95);backdrop-filter:blur(12px);box-shadow:0 18px 50px rgba(37,33,30,.18);border:1px solid var(--line);padding:8px;border-radius:12px;gap:8px}.mobile-donate .btn{flex:1;min-height:46px}.mobile-donate .icon-btn{width:46px;height:46px}
      .toast{left:14px;right:14px;bottom:76px;min-width:0}
    }
    @media (max-width:480px){
      .brand-text b{font-size:12px}.hero-caption{width:220px;padding:16px}.hero-caption b{font-size:14px}.hero-card{width:118px}.timeline{grid-template-columns:1fr}.timeline-item+ .timeline-item{border-right:0;border-top:1px solid var(--line);padding-right:0;margin-right:0}.stats-grid{grid-template-columns:1fr}.footer-grid{grid-template-columns:1fr}.footer-grid>div{grid-column:auto!important}.closing-actions .btn{flex:1 1 100%}
    }
    @media (prefers-reduced-motion:reduce){*,*:before,*:after{scroll-behavior:auto!important;transition:none!important;animation:none!important}}
  </style>
</head>
<body>
  <div class="topbar">
    <div class="container topbar-inner">
      <div class="topbar-group">
        <span class="top-badge">جمعية أهلية غير ربحية · ترخيص 1504</span>
        <span class="top-badge">ترخيص جمع التبرعات 6253</span>
      </div>
      <div class="topbar-group">
        <a href="tel:920022100">920022100</a>
        <a href="mailto:info@ehsan.org.sa">info@ehsan.org.sa</a>
        <a href="#" aria-label="English">EN</a>
      </div>
    </div>
  </div>

  <header class="site-header" id="siteHeader">
    <div class="container nav">
      <a class="brand" href="#home" aria-label="جمعية الإحسان للخدمات الاجتماعية">
        <img src="assets/logo-mark.webp" alt="شعار جمعية الإحسان" />
        <div class="brand-text"><b>جمعية الإحسان</b><span>للخدمات الاجتماعية</span></div>
      </a>
      <nav class="nav-links" aria-label="القائمة الرئيسية">
        <a class="active" href="#home">الرئيسية</a>
        <a href="#about">عن الجمعية</a>
        <a href="#programs">مجالاتنا</a>
        <a href="#donations">التبرعات</a>
        <a href="#media">المركز الإعلامي</a>
        <a href="#governance">الحوكمة</a>
        <a href="#services">الخدمات الإلكترونية</a>
      </nav>
      <div class="nav-actions">
        <button class="icon-btn" id="searchOpen" aria-label="فتح البحث">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><circle cx="11" cy="11" r="7"/><path d="m20 20-4-4"/></svg>
        </button>
        <a class="btn btn-primary" href="#donations">تبرع الآن</a>
        <button class="icon-btn menu-btn" id="menuBtn" aria-label="فتح القائمة" aria-expanded="false">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M4 7h16M4 12h16M4 17h16"/></svg>
        </button>
      </div>
    </div>
    <div class="nav-progress" id="navProgress"></div>
    <nav class="mobile-drawer" id="mobileDrawer" aria-label="القائمة للجوال">
      <a href="#home">الرئيسية</a><a href="#about">عن الجمعية</a><a href="#programs">مجالاتنا</a><a href="#donations">التبرعات</a><a href="#media">المركز الإعلامي</a><a href="#governance">الحوكمة</a><a href="#services">الخدمات الإلكترونية</a><a class="drawer-action" href="#donations">تبرع الآن</a>
    </nav>
  </header>

  <main id="home">
    <section class="hero">
      <div class="container hero-grid">
        <div class="hero-copy">
          <span class="kicker">منذ 1424هـ في خدمة المجتمع</span>
          <h1>نحو أثرٍ <span>أعمق</span><br>وحياةٍ أكثر كرامة.</h1>
          <p class="lead">جمعية الإحسان للخدمات الاجتماعية تبني أثرًا مستدامًا عبر التنمية والرعاية والمبادرات المجتمعية، ضمن عمل مؤسسي يقوم على الثقة والحوكمة.</p>
          <div class="hero-actions">
            <a class="btn btn-primary" href="#donations">تبرع الآن
              <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
            </a>
            <a class="btn btn-outline" href="#about">تعرف على الجمعية</a>
          </div>
          <div class="hero-trust">
            <span class="trust-line"><i class="trust-mark">✓</i>مسجلة بالمركز الوطني لتنمية القطاع غير الربحي</span>
            <span class="trust-line"><i class="trust-mark">✓</i>تقارير وحوكمة وشفافية</span>
          </div>
        </div>

        <div class="hero-visual" aria-label="صورة من برامج جمعية الإحسان">
          <div class="hero-frame-line"></div>
          <div class="hero-photo"><img src="assets/camp.webp" alt="برنامج تنموي من برامج جمعية الإحسان" /></div>
          <div class="hero-card"><strong>1504</strong><span>رقم ترخيص جمعية الإحسان</span></div>
          <div class="hero-caption"><b>نستثمر في الإنسان</b><p>برامج تنموية ورعوية ومجتمعية تُصمم للأثر المستدام.</p></div>
          <div class="hero-seal"><div><b>أثر</b>يمتد للمجتمع</div></div>
        </div>
      </div>
    </section>

    <div class="container donate-dock-wrap">
      <form class="donate-dock" id="quickDonate">
        <div class="dock-intro"><b>تبرع سريع</b><span>اختر الفرصة والمبلغ، ثم انتقل مباشرة إلى خطوة الدفع.</span></div>
        <div class="field">
          <label for="project">فرصة التبرع</label>
          <select id="project"><option>كفارة اليمين</option><option>الصدقة حياة</option><option>زكاة المال</option><option>كفارة الصيام</option><option>الصندوق الوقفي</option><option>إطعام مسكين</option></select>
        </div>
        <div class="amount-wrap">
          <div class="field"><label for="amount">المبلغ</label><input id="amount" type="number" value="100" min="1" inputmode="numeric" /></div>
          <span class="amount-chip">ريال</span>
        </div>
        <button class="btn btn-primary" type="submit">متابعة التبرع</button>
      </form>
    </div>

    <section class="section" id="about">
      <div class="container intro-grid">
        <div class="intro-copy">
          <span class="kicker">عن جمعية الإحسان</span>
          <h2>مسيرة مؤسسية تبدأ من الإنسان وتصل إلى المجتمع.</h2>
          <p>تأسست جمعية الإحسان للخدمات الاجتماعية في مدينة بريدة بتاريخ 3 / 6 / 1441هـ، امتدادًا لمركز الإحسان الخيري الذي تأسس عام 1424هـ، وتعمل على تقديم برامج التنمية والخدمات المجتمعية والرعاية للمحتاجين في منطقة القصيم.</p>
          <div class="timeline">
            <div class="timeline-item"><strong>1424هـ</strong><span>بداية المسيرة عبر مركز الإحسان الخيري</span></div>
            <div class="timeline-item"><strong>القصيم</strong><span>نطاق العمل والخدمات المجتمعية</span></div>
          </div>
          <div class="signature-row">
            <a class="btn btn-link" href="#">اكتشف قصة الإحسان
              <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
            </a>
            <span class="muted" style="font-size:11px">تنمية · رعاية · خدمة مجتمع</span>
          </div>
        </div>
        <div class="intro-visual">
          <img src="assets/visit.webp" alt="لقاء مؤسسي في جمعية الإحسان" />
          <div class="intro-note">نموذج عمل يوازن بين <b>الاحتياج الآني</b> و<b>الأثر طويل المدى</b>.</div>
        </div>
      </div>
    </section>

    <section class="section programs" id="programs">
      <div class="container">
        <div class="section-head">
          <div><span class="kicker on-dark">مجالات عملنا</span><h2>ثلاثة مسارات. هدف واحد.</h2></div>
          <p>خدمات مترابطة تبدأ من تمكين الفرد، وتمتد إلى رعاية الأسرة وخدمة المجتمع ببرامج ومبادرات أكثر استدامة.</p>
        </div>
        <div class="program-grid">
          <article class="program-card">
            <div class="program-no">01 / التنمية</div>
            <div class="program-icon"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7"><path d="M4 20h16M6 20V10l6-6 6 6v10M9 20v-6h6v6"/></svg></div>
            <h3>الخدمات التنموية</h3><p>تطوير القدرات والمهارات، وتمكين الأفراد وتعزيز مشاركتهم الفاعلة واستقلالهم.</p>
            <a class="text-link" href="#">استكشف البرامج <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a>
          </article>
          <article class="program-card">
            <div class="program-no">02 / الرعاية</div>
            <div class="program-icon"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7"><path d="M20.8 4.6a5.4 5.4 0 0 0-7.6 0L12 5.8l-1.2-1.2a5.4 5.4 0 0 0-7.6 7.6L12 21l8.8-8.8a5.4 5.4 0 0 0 0-7.6Z"/></svg></div>
            <h3>الخدمات الرعوية</h3><p>رعاية متكاملة للأسر المكفولة وتلبية الاحتياجات الأساسية بما يعزز الاستقرار والعيش الكريم.</p>
            <a class="text-link" href="#">تعرف على الخدمات <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a>
          </article>
          <article class="program-card">
            <div class="program-no">03 / المجتمع</div>
            <div class="program-icon"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7"><circle cx="8" cy="8" r="3"/><circle cx="16" cy="8" r="3"/><path d="M2.5 20c.5-4 2.5-6 5.5-6s5 2 5.5 6M10.5 20c.5-4 2.5-6 5.5-6s5 2 5.5 6"/></svg></div>
            <h3>الخدمات المجتمعية</h3><p>مبادرات موسمية ومجتمعية وتطوعية تنفذ بالشراكة والتكامل وتستجيب لاحتياجات المجتمع.</p>
            <a class="text-link" href="#">شاهد المبادرات <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a>
          </article>
        </div>
      </div>
    </section>

    <section class="section donations" id="donations">
      <div class="container">
        <div class="section-head compact">
          <div><span class="kicker">فرص التبرع</span><h2>عطاء أوضح. خطوة أسرع.</h2></div>
          <a class="btn btn-link" href="#">عرض جميع المشاريع
            <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg>
          </a>
        </div>

        <article class="donation-feature">
          <div class="donation-feature-copy">
            <span class="donation-feature-tag">فرصة مختارة</span>
            <h3>الصدقة حياة</h3>
            <p>مساحة مرنة للعطاء تتيح لك تحديد قيمة مساهمتك بما يناسبك، لتصل صدقتك عبر قنوات الجمعية وبرامجها.</p>
            <div class="feature-amount"><strong>100</strong><span>ريال · مبلغ مقترح</span></div>
            <div><button class="btn btn-primary donate-demo" data-project="الصدقة حياة" data-amount="100">ساهم الآن</button></div>
          </div>
          <div class="donation-feature-visual">
            <div class="visual-quote"><b>كل مساهمة تبدأ صغيرة، وقد تصنع فرقًا كبيرًا.</b><span>تبرع إلكتروني واضح، موثوق، وقابل للتخصيص.</span></div>
          </div>
        </article>

        <div class="donation-grid">
          <article class="donation-card"><div class="card-top"><div class="card-icon">♡</div><span class="pill">كفارات</span></div><h3>كفارة اليمين</h3><p>ساهم في أداء الكفارة عبر الجمعية وفق المشروع المتاح.</p><div class="card-bottom"><div class="card-price"><strong>100</strong><span>ريال</span></div><button class="btn btn-link donate-demo" data-project="كفارة اليمين" data-amount="100">ساهم الآن <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div></article>
          <article class="donation-card"><div class="card-top"><div class="card-icon">◈</div><span class="pill">زكاة</span></div><h3>زكاة المال</h3><p>خيارات مرنة لإخراج زكاة المال عبر قنوات الجمعية.</p><div class="card-bottom"><div class="card-price"><strong>25+</strong><span>ريال</span></div><button class="btn btn-link donate-demo" data-project="زكاة المال" data-amount="25">ساهم الآن <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div></article>
          <article class="donation-card"><div class="card-top"><div class="card-icon">⌁</div><span class="pill">كفارات</span></div><h3>كفارة الصيام</h3><p>حدد مدة الكفارة بعدد الأيام واستكمل مساهمتك مباشرة.</p><div class="card-bottom"><div class="card-price"><strong>10</strong><span>ريال / يوم</span></div><button class="btn btn-link donate-demo" data-project="كفارة الصيام" data-amount="10">ساهم الآن <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div></article>
          <article class="donation-card"><div class="card-top"><div class="card-icon">□</div><span class="pill">وقف</span></div><h3>الصندوق الوقفي</h3><p>مساهمة وقفية مستدامة بوحدات مرنة بحسب المشروع.</p><div class="card-bottom"><div class="card-price"><strong>10</strong><span>ريال / وحدة</span></div><button class="btn btn-link donate-demo" data-project="الصندوق الوقفي" data-amount="10">ساهم الآن <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div></article>
          <article class="donation-card"><div class="card-top"><div class="card-icon">○</div><span class="pill">إطعام</span></div><h3>إطعام مسكين</h3><p>اختر عدد المستفيدين وساهم في مشروع الإطعام.</p><div class="card-bottom"><div class="card-price"><strong>10</strong><span>ريال</span></div><button class="btn btn-link donate-demo" data-project="إطعام مسكين" data-amount="10">ساهم الآن <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div></article>
          <article class="donation-card"><div class="card-top"><div class="card-icon">◇</div><span class="pill">صدقة</span></div><h3>تبرع مفتوح</h3><p>حدد المبلغ الذي يناسبك ليتم توجيهه إلى مسارات الجمعية.</p><div class="card-bottom"><div class="card-price"><strong>حدد</strong><span>المبلغ</span></div><button class="btn btn-link donate-demo" data-project="تبرع مفتوح" data-amount="100">ساهم الآن <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></button></div></article>
        </div>
      </div>
    </section>

    <section class="section impact" id="impact">
      <div class="container impact-layout">
        <div class="impact-intro">
          <span class="kicker">الأثر بالأرقام</span>
          <h2>حين يتحول العطاء إلى نتائج قابلة للقياس.</h2>
          <p>إحصائيات الجمعية المنشورة لعام 2025، مصممة هنا لتكون أوضح وأسهل قراءة على جميع الأجهزة.</p>
          <span class="impact-year">إحصائيات 2025</span>
        </div>
        <div class="stats-grid">
          <div class="stat"><strong data-count="25193">25,193</strong><span>الأسر المستفيدة</span></div>
          <div class="stat"><strong data-count="591">591</strong><span>الأسر المكفولة</span></div>
          <div class="stat"><strong data-count="71">71</strong><span>الجمعيات المشاركة</span></div>
          <div class="stat"><strong data-count="21730">21,730</strong><span>الساعات التطوعية</span></div>
          <div class="stat"><strong data-count="1649">1,649</strong><span>المتطوعون</span></div>
          <div class="stat"><strong data-count="100">100</strong><span>المشاريع المنفذة</span></div>
          <div class="stat"><strong data-count="391">391</strong><span>مستفيدو البرامج التنموية</span></div>
          <div class="stat cost"><strong>15,940,775.83</strong><span>ريال · تكلفة البرامج المقدمة</span></div>
        </div>
      </div>
    </section>

    <section class="section journeys" id="services">
      <div class="container">
        <div class="section-head">
          <div><span class="kicker">الخدمات الإلكترونية</span><h2>ابدأ من احتياجك مباشرة.</h2></div>
          <p>مسارات مختصرة وواضحة للمتبرع والمستفيد والمتطوع والباحث عن فرصة.</p>
        </div>
        <div class="journey-grid">
          <article class="journey"><div class="journey-icon">♡</div><h3>للمستفيد</h3><p>التسجيل والخدمات والضوابط المرتبطة بالمستفيدين.</p><a class="text-link" href="#">ابدأ الخدمة <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></article>
          <article class="journey"><div class="journey-icon">✦</div><h3>للمتطوع</h3><p>انضم إلى الفرص والبرامج التطوعية وشارك في صناعة الأثر.</p><a class="text-link" href="#">تسجيل متطوع <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></article>
          <article class="journey"><div class="journey-icon">□</div><h3>للباحث عن عمل</h3><p>استعرض الوظائف والفرص المتاحة وقدم طلبك إلكترونيًا.</p><a class="text-link" href="#">عرض الفرص <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></article>
          <article class="journey"><div class="journey-icon">✓</div><h3>قياسات الرضا</h3><p>شارك تجربتك وساهم في تحسين جودة الخدمات والبرامج.</p><a class="text-link" href="#">شارك رأيك <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></article>
        </div>
      </div>
    </section>

    <section class="section media" id="media">
      <div class="container">
        <div class="section-head compact">
          <div><span class="kicker">المركز الإعلامي</span><h2>من الميدان، إلى المجتمع.</h2></div>
          <a class="btn btn-link" href="#">عرض المركز الإعلامي <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a>
        </div>
        <div class="media-grid">
          <article class="news featured"><div class="news-img"><img src="assets/school.webp" alt="صرف المستلزمات المدرسية للأسر المكفولة" /></div><div class="news-body"><div class="news-meta">17 أغسطس 2026</div><h3>جمعية الإحسان تختتم صرف المستلزمات المدرسية للأسر المكفولة للعام الدراسي الجديد</h3><p>استفاد من المشروع 245 أسرة و583 فردًا، بتكلفة إجمالية بلغت 189,400 ريال.</p><a class="text-link" href="#">قراءة الخبر <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></div></article>
          <article class="news"><div class="news-img"><img src="assets/visit.webp" alt="زيارة وفد مؤسسة الملك خالد" /></div><div class="news-body"><div class="news-meta">05 أغسطس 2026</div><h3>استقبال وفد مؤسسة الملك خالد وشركة الريادة الاجتماعية</h3><p>زيارة ميدانية للاطلاع على تجربة الجمعية وفرص التطوير والاستدامة.</p><a class="text-link" href="#">قراءة الخبر <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></div></article>
          <article class="news"><div class="news-img"><img src="assets/camp.webp" alt="المعسكر العلمي الثالث" /></div><div class="news-body"><div class="news-meta">30 يوليو 2026</div><h3>ختام المعسكر العلمي الثالث بعد رحلة معرفية ومهارية</h3><p>برامج علمية وتطبيقية استهدفت تنمية قدرات الطلاب وصقل مهاراتهم.</p><a class="text-link" href="#">قراءة الخبر <svg class="arrow" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><path d="M5 12h14M13 6l6 6-6 6"/></svg></a></div></article>
        </div>
      </div>
    </section>

    <section class="section governance" id="governance">
      <div class="container gov-shell">
        <div class="gov-copy">
          <span class="kicker">الحوكمة والشفافية</span>
          <h2>كل وثيقة رسمية، في مكان واحد.</h2>
          <p>مركز منظم للوائح والسياسات والقوائم المالية والتقارير السنوية ومحاضر الاجتماعات، مع بحث وفلترة تسهّل الوصول إلى المعلومة.</p>
          <form class="gov-search" id="govSearch"><input type="search" placeholder="ابحث عن تقرير، سياسة، لائحة..." aria-label="البحث في الحوكمة" /><button aria-label="بحث"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><circle cx="11" cy="11" r="7"/><path d="m20 20-4-4"/></svg></button></form>
          <div class="gov-links">
            <a class="gov-link" href="#"><span>اللوائح والسياسات</span><b>←</b></a>
            <a class="gov-link" href="#"><span>القوائم المالية</span><b>←</b></a>
            <a class="gov-link" href="#"><span>التقارير السنوية</span><b>←</b></a>
            <a class="gov-link" href="#"><span>مجلس الإدارة</span><b>←</b></a>
          </div>
        </div>
        <div class="gov-visual">
          <div class="gov-year"><strong>2025</strong><span>أحدث تقرير سنوي ظاهر حاليًا</span></div>
          <div class="gov-quote">«الثقة تبدأ من وضوح المعلومات وسهولة الوصول إليها.»</div>
          <div class="gov-badge">حوكمة · تقارير · سياسات · قوائم مالية · محاضر</div>
        </div>
      </div>
    </section>

    <section class="closing">
      <div class="container closing-inner">
        <div><h2>كن جزءًا من أثر الإحسان.</h2><p>تبرع، تطوع، أو تعرف أكثر على برامج الجمعية وخدماتها.</p></div>
        <div class="closing-actions"><a class="btn btn-white" href="#donations">تبرع الآن</a><a class="btn btn-outline" href="#services" style="border-color:rgba(255,255,255,.35);color:#fff;background:transparent">استكشف الخدمات</a></div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">
      <div class="footer-grid">
        <div>
          <div class="footer-brand"><img src="assets/logo-mark.webp" alt="شعار جمعية الإحسان" /><b>جمعية الإحسان للخدمات الاجتماعية</b></div>
          <p>جمعية أهلية مسجلة بالمركز الوطني لتنمية القطاع غير الربحي برقم 1504، وهي امتداد لمركز الإحسان الخيري ببريدة الذي تأسس عام 1424هـ.</p>
          <p class="footer-license">ترخيص الجمعية 1504 · ترخيص جمع التبرعات 6253</p>
          <div class="socials"><a class="social" href="#" aria-label="X">X</a><a class="social" href="#" aria-label="Instagram">IG</a><a class="social" href="#" aria-label="YouTube">YT</a></div>
        </div>
        <div><h4>الجمعية</h4><div class="footer-links"><a href="#about">عن الجمعية</a><a href="#programs">مجالات العمل</a><a href="#media">المركز الإعلامي</a><a href="#governance">الحوكمة</a><a href="#donations">التبرعات</a></div></div>
        <div><h4>الخدمات</h4><div class="footer-links"><a href="#services">تسجيل مستفيد</a><a href="#services">تسجيل متطوع</a><a href="#services">طلب توظيف</a><a href="#services">قياسات الرضا</a><a href="#">حاسبة الزكاة</a></div></div>
        <div><h4>تواصل معنا</h4><div class="footer-contact"><span>القصيم – بريدة – برج الإحسان</span><a href="tel:920022100">920022100</a><a href="mailto:info@ehsan.org.sa">info@ehsan.org.sa</a><span>ص.ب 24000 بريدة 51311</span></div></div>
      </div>
      <div class="footer-bottom"><span>© 2026 جمعية الإحسان للخدمات الاجتماعية</span><span>سياسة الخصوصية · سياسة الاستخدام · اتصل بنا</span></div>
    </div>
  </footer>

  <div class="mobile-donate" aria-label="إجراءات سريعة"><a class="btn btn-primary" href="#donations">تبرع الآن</a><button class="icon-btn" id="mobileSearch" aria-label="البحث"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><circle cx="11" cy="11" r="7"/><path d="m20 20-4-4"/></svg></button></div>

  <div class="search-modal" id="searchModal" role="dialog" aria-modal="true" aria-labelledby="searchTitle">
    <div class="search-panel">
      <div class="search-top"><b id="searchTitle">البحث في موقع الإحسان</b><button class="icon-btn" id="searchClose" aria-label="إغلاق">×</button></div>
      <form class="search-box" id="siteSearch"><input id="searchInput" type="search" placeholder="اكتب كلمة البحث..." autocomplete="off" /><button aria-label="بحث"><svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.8"><circle cx="11" cy="11" r="7"/><path d="m20 20-4-4"/></svg></button></form>
      <div class="search-hints"><span>التقارير السنوية</span><span>زكاة المال</span><span>المتطوعون</span><span>السياسات</span><span>التسجيل كمستفيد</span></div>
    </div>
  </div>

  <div class="toast" id="toast" role="status" aria-live="polite"></div>

  <script>
    const body=document.body;
    const menuBtn=document.getElementById('menuBtn');
    const drawer=document.getElementById('mobileDrawer');
    const searchModal=document.getElementById('searchModal');
    const searchOpen=document.getElementById('searchOpen');
    const mobileSearch=document.getElementById('mobileSearch');
    const searchClose=document.getElementById('searchClose');
    const searchInput=document.getElementById('searchInput');
    const toast=document.getElementById('toast');
    const progress=document.getElementById('navProgress');

    function setDrawer(open){
      drawer.classList.toggle('open',open);
      menuBtn?.setAttribute('aria-expanded',String(open));
      body.classList.toggle('menu-open',open);
    }
    menuBtn?.addEventListener('click',()=>setDrawer(!drawer.classList.contains('open')));
    drawer?.querySelectorAll('a').forEach(a=>a.addEventListener('click',()=>setDrawer(false)));

    function setSearch(open){
      searchModal.classList.toggle('open',open);
      body.classList.toggle('modal-open',open);
      if(open) setTimeout(()=>searchInput.focus(),100);
    }
    searchOpen?.addEventListener('click',()=>setSearch(true));
    mobileSearch?.addEventListener('click',()=>setSearch(true));
    searchClose?.addEventListener('click',()=>setSearch(false));
    searchModal?.addEventListener('click',e=>{if(e.target===searchModal)setSearch(false)});
    document.addEventListener('keydown',e=>{if(e.key==='Escape'){setSearch(false);setDrawer(false)}});

    function showToast(title,text){
      toast.innerHTML=`<b>${title}</b>${text}`;
      toast.classList.add('show');
      clearTimeout(window.__toastTimer);
      window.__toastTimer=setTimeout(()=>toast.classList.remove('show'),3600);
    }

    document.getElementById('quickDonate')?.addEventListener('submit',e=>{
      e.preventDefault();
      const project=document.getElementById('project').value;
      const amount=document.getElementById('amount').value || '0';
      showToast('تم تجهيز التبرع',`${project} — ${amount} ريال. في النسخة النهائية تُربط هذه الخطوة ببوابة الدفع الحالية.`);
    });

    document.querySelectorAll('.donate-demo').forEach(btn=>btn.addEventListener('click',()=>{
      showToast('فرصة التبرع',`${btn.dataset.project} — ${btn.dataset.amount} ريال. هذه واجهة تجريبية لمسار الدفع.`);
    }));

    document.getElementById('govSearch')?.addEventListener('submit',e=>{
      e.preventDefault();
      const value=e.currentTarget.querySelector('input').value.trim();
      showToast('البحث في الحوكمة',value?`بحث تجريبي عن: ${value}`:'اكتب اسم التقرير أو الوثيقة للبحث.');
    });

    document.getElementById('siteSearch')?.addEventListener('submit',e=>{
      e.preventDefault();
      const value=searchInput.value.trim();
      setSearch(false);
      showToast('بحث الموقع',value?`بحث تجريبي عن: ${value}`:'اكتب كلمة البحث أولًا.');
    });

    function updateProgress(){
      const h=document.documentElement;
      const max=h.scrollHeight-h.clientHeight;
      const pct=max>0?(h.scrollTop/max)*100:0;
      progress.style.width=`${pct}%`;
    }
    addEventListener('scroll',updateProgress,{passive:true});updateProgress();

    const counterEls=[...document.querySelectorAll('[data-count]')];
    if('IntersectionObserver' in window && !matchMedia('(prefers-reduced-motion: reduce)').matches){
      const observer=new IntersectionObserver(entries=>{
        entries.forEach(entry=>{
          if(!entry.isIntersecting)return;
          const el=entry.target;
          const target=Number(el.dataset.count);
          const start=performance.now();
          const duration=900;
          function tick(now){
            const p=Math.min(1,(now-start)/duration);
            const eased=1-Math.pow(1-p,3);
            el.textContent=Math.round(target*eased).toLocaleString('en-US');
            if(p<1)requestAnimationFrame(tick);
          }
          requestAnimationFrame(tick);observer.unobserve(el);
        });
      },{threshold:.45});
      counterEls.forEach(el=>observer.observe(el));
    }
  </script>
</body>
</html>
