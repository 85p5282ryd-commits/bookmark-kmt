<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>bookmark | 熊本・下通 会話が主役の大人数でも使いやすい遊べるバー</title>
  <meta name="description" content="熊本・下通のアミューズメントバー bookmark。4名から20名ほどの集まり、二次会、打ち上げ、貸切にも使いやすい、会話が主役の落ち着いた遊べるバー。平日 無制限飲み放題3,500円。" />
  
  <style>
    /* --- Variables --- */
    :root {
      --bg: #0d0d0f;
      --bg-soft: #151519;
      --card: rgba(255, 255, 255, 0.05);
      --card-hover: rgba(255, 255, 255, 0.08);
      --text: #f2f2f0;
      --muted: #b9b8b2;
      --line: rgba(255, 255, 255, 0.12);
      --accent: #d9c6a0;
      --accent-dark: #a89164;
      --shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
      --max-width: 1120px;
      --radius-xl: 28px;
      --radius-lg: 22px;
      --radius-md: 16px;
      --transition: 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);
    }

    /* --- Base --- */
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    
    body {
      margin: 0;
      font-family: "Helvetica Neue", Arial, "Hiragino Kaku Gothic ProN", "Hiragino Sans", Meiryo, sans-serif;
      background-color: var(--bg);
      background-image: 
        radial-gradient(circle at top right, rgba(217, 198, 160, 0.12), transparent 40%),
        radial-gradient(circle at bottom left, rgba(217, 198, 160, 0.08), transparent 30%);
      color: var(--text);
      line-height: 1.8;
      word-break: break-all;
    }

    a { color: inherit; text-decoration: none; transition: var(--transition); }
    ul { padding: 0; list-style: none; }

    /* --- Layout Components --- */
    .container {
      width: min(calc(100% - 40px), var(--max-width));
      margin: 0 auto;
    }

    section { padding: 80px 0; }
    @media (max-width: 768px) { section { padding: 50px 0; } }

    .grid { display: grid; gap: 20px; }
    .grid-2 { grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); }
    .grid-3 { grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); }
    .grid-4 { grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); }

    /* --- UI Parts --- */
    .card-base {
      background: var(--card);
      border: 1px solid var(--line);
      border-radius: var(--radius-lg);
      padding: 30px;
      transition: var(--transition);
    }
    .card-base:hover { background: var(--card-hover); transform: translateY(-4px); }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      min-height: 54px;
      padding: 0 32px;
      border-radius: 999px;
      font-weight: 700;
      cursor: pointer;
      border: none;
    }
    .btn-primary {
      background: linear-gradient(135deg, var(--accent) 0%, var(--accent-dark) 100%);
      color: #141414;
      box-shadow: 0 10px 20px rgba(168, 145, 100, 0.2);
    }
    .btn-secondary {
      background: rgba(255, 255, 255, 0.08);
      border: 1px solid var(--line);
      color: var(--text);
    }
    .btn:hover { opacity: 0.9; transform: scale(1.02); }

    /* --- Header --- */
    .header {
      position: sticky; top: 0; z-index: 100;
      backdrop-filter: blur(16px);
      background: rgba(13, 13, 15, 0.8);
      border-bottom: 1px solid var(--line);
    }
    .header-inner {
      display: flex; align-items: center; justify-content: space-between;
      height: 72px;
    }
    .nav { display: flex; gap: 24px; font-size: 14px; font-weight: 500; }
    @media (max-width: 900px) { .nav { display: none; } }

    /* --- Hero --- */
    .hero { padding-top: 60px; }
    .hero-content h1 {
      font-size: clamp(32px, 5vw, 56px);
      line-height: 1.2;
      margin: 20px 0;
      font-weight: 800;
    }
    .eyebrow {
      color: var(--accent);
      font-size: 14px;
      font-weight: 700;
      letter-spacing: 0.1em;
      display: block;
    }
    .pill-group { display: flex; flex-wrap: wrap; gap: 8px; margin: 24px 0; }
    .pill {
      font-size: 13px; padding: 6px 16px;
      background: rgba(217, 198, 160, 0.1);
      border: 1px solid rgba(217, 198, 160, 0.2);
      border-radius: 50px;
    }

    /* --- Specific Sections --- */
    .section-title { font-size: clamp(24px, 4vw, 36px); margin-bottom: 12px; }
    .section-desc { color: var(--muted); margin-bottom: 40px; max-width: 700px; }

    .price-box { text-align: center; border-color: var(--accent-dark); }
    .price-val { font-size: 48px; font-weight: 800; color: var(--accent); margin: 10px 0; }

    /* --- Footer & Floating --- */
    .footer { padding: 60px 0 120px; border-top: 1px solid var(--line); color: var(--muted); font-size: 14px; }
    
    .floating-cta {
      position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%);
      width: min(calc(100% - 32px), 500px);
      display: grid; grid-template-columns: 1fr 1fr; gap: 12px;
      background: rgba(20, 20, 25, 0.9); padding: 12px;
      border-radius: 20px; backdrop-filter: blur(10px);
      border: 1px solid var(--line); z-index: 200;
    }
  </style>
</head>
<body>

  <header class="header">
    <div class="container header-inner">
      <a href="#" class="logo" style="font-size: 24px; font-weight: 800;">bookmark</a>
      <nav class="nav">
        <a href="#about">特徴</a>
        <a href="#pricing">料金</a>
        <a href="#group">貸切</a>
        <a href="#access">アクセス</a>
      </nav>
      <a href="#reserve" class="btn btn-primary" style="min-height: 40px; padding: 0 20px; font-size: 13px;">予約する</a>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container grid grid-2">
        <div class="hero-content">
          <span class="eyebrow">KUMAMOTO SHIMOTORI</span>
          <h1>大人数でも使いやすい。<br>でも、うるさすぎない。</h1>
          <p class="section-desc">
            bookmarkは、会話を主役にしたアミューズメントバーです。ダーツや卓球を楽しみながら、落ち着いた時間をお過ごしいただけます。
          </p>
          <div class="pill-group">
            <span class="pill">平日 無制限 3,500円</span>
            <span class="pill">4名〜20名対応</span>
            <span class="pill">カラオケなし</span>
          </div>
          <div style="display: flex; gap: 12px;">
            <a href="#reserve" class="btn btn-primary">予約・問い合わせ</a>
            <a href="#pricing" class="btn btn-secondary">料金を見る</a>
          </div>
        </div>
        <div class="card-base" style="background: linear-gradient(135deg, rgba(255,255,255,0.08), transparent);">
          <h2 style="font-size: 20px; margin-bottom: 20px;">安心の定額システム</h2>
          <div style="margin-bottom: 24px;">
            <p style="font-size: 13px; color: var(--accent); margin: 0;">平日</p>
            <p style="font-size: 28px; font-weight: 800; margin: 5px 0;">無制限飲み放題 ¥3,500</p>
          </div>
          <div>
            <p style="font-size: 13px; color: var(--accent); margin: 0;">金・土・祝前日</p>
            <p style="font-size: 28px; font-weight: 800; margin: 5px 0;">150分飲み放題 ¥3,500</p>
          </div>
        </div>
      </div>
    </section>

    <section id="about">
      <div class="container">
        <span class="eyebrow">ABOUT</span>
        <h2 class="section-title">bookmarkが選ばれる理由</h2>
        <div class="grid grid-3">
          <article class="card-base">
            <h3>会話が主役</h3>
            <p class="muted">あえてカラオケを設置せず、自然な会話が弾む音量にこだわっています。</p>
          </article>
          <article class="card-base">
            <h3>大人数に最適</h3>
            <p class="muted">4〜20名のグループに最適なレイアウト。二次会や打ち上げに重宝されます。</p>
          </article>
          <article class="card-base">
            <h3>明朗会計</h3>
            <p class="muted">「結局いくら？」という不安を解消。追加料金なしの分かりやすいプランです。</p>
          </article>
        </div>
      </div>
    </section>

    <section id="pricing" style="background: var(--bg-soft);">
      <div class="container">
        <span class="eyebrow">PRICING</span>
        <h2 class="section-title">シンプルな料金体系</h2>
        <div class="grid grid-2">
          <div class="card-base price-box">
            <h3>平日 (月〜木)</h3>
            <p class="price-val">¥3,500</p>
            <p>時間無制限・飲み放題</p>
          </div>
          <div class="card-base price-box">
            <h3>週末 (金土祝前)</h3>
            <p class="price-val">¥3,500</p>
            <p>150分・飲み放題</p>
          </div>
        </div>
      </div>
    </section>

    <section id="access">
      <div class="container grid grid-2">
        <div>
          <span class="eyebrow">ACCESS</span>
          <h2 class="section-title">アクセス</h2>
          <p>〒860-0807<br>熊本県熊本市中央区下通1-2-11 TM34ビル4階</p>
          <p>電話: <a href="tel:0962289880" style="color: var(--accent); font-weight: 700;">096-228-9880</a></p>
          <p>Instagram: <a href="https://www.instagram.com/bookmark_kmt/" target="_blank">@bookmark_kmt</a></p>
        </div>
        <div id="reserve" class="card-base">
          <h3 style="margin-top: 0;">ご予約・お問い合わせ</h3>
          <p class="muted">貸切の相談や人数の変更など、柔軟に対応いたします。まずはお気軽にご連絡ください。</p>
          <a href="tel:0962289880" class="btn btn-primary" style="width: 100%;">電話で問い合わせ</a>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">
      <p>&copy; 2024 bookmark - Amusement Bar in Kumamoto</p>
    </div>
  </footer>

  <div class="floating-cta">
    <a href="tel:0962289880" class="btn btn-secondary" style="min-height: 44px;">電話する</a>
    <a href="https://www.instagram.com/bookmark_kmt/" class="btn btn-primary" style="min-height: 44px;">Instagram</a>
  </div>

</body>
</html>
