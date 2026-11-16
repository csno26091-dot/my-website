# my-website
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tの自己紹介 | 大学1年生</title>
  <style>
    /* 基本設定・リセット */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: "Hiragino Kaku Gothic ProN", "Hiragino Sans", "BIZ UDPGothic", "Meiryo", sans-serif;
      line-height: 1.8;
      color: #1e293b;
      background-color: #f8fafc;
    }

    /* ヘッダー・ナビゲーション */
    header {
      background: linear-gradient(135deg, #1d4ed8 0%, #2563eb 100%);
      color: #ffffff;
      padding: 2.5rem 1.25rem 1.5rem;
      text-align: center;
    }

    .site-title {
      font-size: 1.85rem;
      font-weight: 700;
      letter-spacing: 0.05em;
      margin-bottom: 0.4rem;
    }

    .site-subtitle {
      font-size: 0.95rem;
      color: #dbeafe;
      margin-bottom: 1.75rem;
    }

    nav {
      max-width: 800px;
      margin: 0 auto;
      background-color: rgba(255, 255, 255, 0.14);
      border-radius: 9999px;
      padding: 0.5rem 1rem;
    }

    nav ul {
      list-style: none;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: 0.5rem 1.25rem;
    }

    nav a {
      color: #ffffff;
      text-decoration: none;
      font-size: 0.9rem;
      font-weight: 600;
      padding: 0.35rem 0.75rem;
      border-radius: 9999px;
      transition: background-color 0.2s ease;
      display: inline-block;
    }

    nav a:hover,
    nav a:focus {
      background-color: #ffffff;
      color: #1d4ed8;
    }

    /* メインコンテンツ */
    main {
      max-width: 800px;
      margin: 2rem auto;
      padding: 0 1.25rem;
      display: flex;
      flex-direction: column;
      gap: 1.75rem;
    }

    section {
      background-color: #ffffff;
      border: 1px solid #e2e8f0;
      border-radius: 12px;
      padding: 2rem;
      box-shadow: 0 2px 8px rgba(15, 23, 42, 0.04);
      scroll-margin-top: 1.5rem;
    }

    h2 {
      font-size: 1.35rem;
      color: #1e40af;
      border-left: 5px solid #2563eb;
      padding-left: 0.75rem;
      margin-bottom: 1.25rem;
      line-height: 1.4;
    }

    p {
      margin-bottom: 1rem;
    }

    p:last-child {
      margin-bottom: 0;
    }

    /* プロフィール強調ボックス */
    .profile-badge {
      display: inline-block;
      background-color: #eff6ff;
      color: #1d4ed8;
      border: 1px solid #bfdbfe;
      font-weight: 700;
      padding: 0.35rem 0.9rem;
      border-radius: 6px;
      margin-bottom: 1rem;
      font-size: 0.95rem;
    }

    /* バンド紹介リスト */
    .band-list {
      list-style: none;
      margin-top: 1.25rem;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
      gap: 1rem;
    }

    .band-item {
      background-color: #f0f7ff;
      border: 1px solid #dbeafe;
      border-radius: 8px;
      padding: 1rem 1.1rem;
    }

    .band-name {
      display: block;
      font-weight: 700;
      color: #1e3a8a;
      font-size: 1.05rem;
      margin-bottom: 0.35rem;
    }

    .band-desc {
      font-size: 0.9rem;
      color: #334155;
      line-height: 1.6;
    }

    /* 目標ボックス */
    .goal-box {
      background-color: #f8fafc;
      border-left: 4px solid #3b82f6;
      padding: 1.25rem;
      border-radius: 0 8px 8px 0;
      font-weight: 500;
    }

    /* 公式サイトリンクエリア */
    .link-area {
      text-align: center;
      padding-top: 0.5rem;
    }

    .official-link {
      display: inline-block;
      background-color: #2563eb;
      color: #ffffff;
      text-decoration: none;
      font-weight: 700;
      padding: 0.85rem 2rem;
      border-radius: 8px;
      transition: background-color 0.2s ease, transform 0.1s ease;
    }

    .official-link:hover,
    .official-link:focus {
      background-color: #1d4ed8;
    }

    .link-note {
      margin-top: 0.75rem;
      font-size: 0.85rem;
      color: #64748b;
    }

    /* フッター */
    footer {
      text-align: center;
      padding: 2rem 1rem;
      color: #64748b;
      font-size: 0.85rem;
      border-top: 1px solid #e2e8f0;
      background-color: #ffffff;
      margin-top: 3rem;
    }

    /* 狭い画面（スマートフォンなど）向け調整 */
    @media (max-width: 600px) {
      header {
        padding: 2rem 1rem 1.25rem;
      }

      .site-title {
        font-size: 1.5rem;
      }

      nav {
        border-radius: 12px;
        padding: 0.5rem;
      }

      nav ul {
        gap: 0.35rem;
      }

      nav a {
        font-size: 0.85rem;
        padding: 0.3rem 0.6rem;
      }

      main {
        margin: 1.25rem auto;
        padding: 0 0.9rem;
        gap: 1.25rem;
      }

      section {
        padding: 1.35rem 1.15rem;
      }

      h2 {
        font-size: 1.2rem;
      }

      .official-link {
        width: 100%;
        padding: 0.85rem 1rem;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1 class="site-title">Tの自己紹介ページ</h1>
    <p class="site-subtitle">大学1年生 / 自分の関心を知ってもらうためのプロフィール</p>
    <nav aria-label="ページ内メニュー">
      <ul>
        <li><a href="#about">自己紹介</a></li>
        <li><a href="#favorite">好きなギタリスト</a></li>
        <li><a href="#goal">今後の目標</a></li>
        <li><a href="#links">公式サイト</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section id="about">
      <h2>自己紹介</h2>
      <span class="profile-badge">ハンドルネーム：T</span>
      <p>
        はじめまして、大学1年生のTです。同級生のみんなに自分の関心を知ってもらいたくて、この自己紹介ページを作りました。
      </p>
      <p>
        毎日ギターにたしなんでおり、音楽やギターの演奏に関心があります。
      </p>
    </section>

    <section id="favorite">
      <h2>好きなギタリスト</h2>
      <p>
        <strong>Ichka Nito</strong>というギタリストが大好きです。
      </p>
      <p>
        彼はいわゆるソロギタリストで、繊細なタッチによるクリスタルのような音色が特徴です。また、ソロ活動だけではなくバンドもいくつか組んでおり、幅広いシーンで活動しています。
      </p>
      <ul class="band-list">
        <li class="band-item">
          <span class="band-name">Among the sreep</span>
          <span class="band-desc">メタルインストバンドとして活動しています。</span>
        </li>
        <li class="band-item">
          <span class="band-name">Ichikoro</span>
          <span class="band-desc">下種の極み乙女で有名な川谷絵音さんが所属するバンドです。</span>
        </li>
        <li class="band-item">
          <span class="band-name">Dios</span>
          <span class="band-desc">J-POP界隈でかなりの知名度を持つバンドです。</span>
        </li>
      </ul>
    </section>

    <section id="goal">
      <h2>今後の目標</h2>
      <div class="goal-box">
        <p>
          今後の私の目標は、Ichka Nitoのように、人の心を動かせる演奏や曲づくりができるようになることです。
        </p>
      </div>
    </section>

    <section id="links">
      <h2>公式サイトへのリンク</h2>
      <div class="link-area">
        <!-- href="#" の部分を実際の公式サイトURLに書き換えて使用してください -->
        <a href="#" class="official-link" target="_blank" rel="noopener noreferrer">
          Ichka Nito 公式サイトへ
        </a>
        <p class="link-note">※リンク先のURLを設定すると公式サイトへ移動できます。</p>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; T</p>
  </footer>

</body>
</html>
