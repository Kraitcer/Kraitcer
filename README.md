
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="theme-color" content="#090d18">
  <meta name="description" content="Hi there, I'm Gleb Kraitcer, a full stack developer.">
  <title>Gleb Kraitcer — Full Stack Developer</title>
  <style>
    :root {
      color-scheme: dark;
      font-family: Inter, "Segoe UI", Arial, sans-serif;
      font-synthesis: none;
      text-rendering: optimizeLegibility;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
    }

    * {
      box-sizing: border-box;
    }

    body {
      min-height: 100vh;
      margin: 0;
      background: #090d18;
      color: #f7f8ff;
    }

    .landing {
      position: relative;
      isolation: isolate;
      display: flex;
      min-height: 100vh;
      min-height: 100svh;
      flex-direction: column;
      justify-content: space-between;
      overflow: hidden;
      padding: clamp(2rem, 6vw, 5.5rem) clamp(1.25rem, 7vw, 7rem) clamp(1.25rem, 3.5vw, 3rem);
      background-image: url("images/landingOverview.webp");
      background-position: center center;
      background-size: cover;
    }

    .landing::before {
      position: absolute;
      z-index: -1;
      background:
        linear-gradient(180deg, rgb(5 8 17 / 69%) 0%, rgb(5 8 17 / 17%) 44%, rgb(5 8 17 / 18%) 62%, rgb(5 8 17 / 76%) 100%),
        linear-gradient(90deg, rgb(5 8 17 / 29%) 0%, transparent 76%);
      content: "";
      inset: 0;
    }

    .intro {
      max-width: 1050px;
      text-wrap: balance;
    }

    .intro h1 {
      margin: 0;
      font-size: clamp(2.2rem, 5.3vw, 5.5rem);
      font-weight: 750;
      letter-spacing: -0.055em;
      line-height: 1.08;
    }

    .intro h1 span {
      display: block;
      margin-top: 0.13em;
      background: linear-gradient(95deg, #48d8ff 4%, #73a7ff 50%, #c376ff 96%);
      background-clip: text;
      color: transparent;
      -webkit-background-clip: text;
    }

    .technologies {
      display: grid;
      grid-template-columns: repeat(4, minmax(0, 1fr));
      background: rgb(7 12 25 / 32%);
      -webkit-backdrop-filter: blur(14px);
      backdrop-filter: blur(14px);
    }

    .technology-group {
      min-width: 0;
      padding: 1rem clamp(0.65rem, 1.6vw, 1.5rem);
    }

    .technology-group + .technology-group {
      border-left: 1px solid rgb(186 204 255 / 24%);
    }

    .technology-group h2 {
      margin: 0 0 0.8rem;
      color: #aab9d6;
      font-size: 0.7rem;
      font-weight: 700;
      letter-spacing: 0.11em;
      text-transform: uppercase;
    }

    .logo-list {
      display: flex;
      min-height: 2.25rem;
      align-items: center;
      gap: clamp(0.65rem, 1.45vw, 1.3rem);
    }

    .logo-list a {
      display: inline-flex;
      flex: 0 0 auto;
      align-items: center;
      justify-content: center;
      transition: transform 160ms ease;
    }

    .logo-list a:hover {
      transform: translateY(-3px);
    }

    .logo-list img {
      display: block;
      width: clamp(1.5rem, 2.5vw, 2rem);
      height: clamp(1.5rem, 2.5vw, 2rem);
      object-fit: contain;
    }

    .logo-list .wordmark {
      width: clamp(2.5rem, 4vw, 3.4rem);
    }

    @media (max-width: 760px) {
      .landing {
        padding: 2rem 1rem 1rem;
        background-position: center center;
      }

      .intro {
        max-width: 560px;
      }

      .intro h1 {
        max-width: 12ch;
        font-size: clamp(2.3rem, 9vw, 4rem);
      }

      .technologies {
        grid-template-columns: repeat(2, minmax(0, 1fr));
      }

      .technology-group {
        padding: 0.8rem;
      }

      .technology-group + .technology-group {
        border-left: 0;
      }

      .technology-group:nth-child(even) {
        border-left: 1px solid rgb(186 204 255 / 24%);
      }

      .technology-group:nth-child(n + 3) {
        border-top: 1px solid rgb(186 204 255 / 24%);
      }
    }

    @media (max-width: 380px) {
      .technology-group {
        padding: 0.65rem;
      }

      .logo-list {
        gap: 0.55rem;
      }

      .logo-list .wordmark {
        width: 2rem;
      }
    }

    @media (prefers-reduced-motion: reduce) {
      *,
      *::before,
      *::after {
        scroll-behavior: auto !important;
        transition-duration: 0.01ms !important;
      }
    }
  </style>
</head>
<body>
  <main class="landing">
    <header class="intro">
      <h1>Hi there ✌️. My name is Gleb Kraitcer<span>I am a full stack developer</span></h1>
    </header>

    <section class="technologies" aria-label="Technologies I work with">
      <div class="technology-group">
        <h2>Languages</h2>
        <div class="logo-list">
          <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" aria-label="JavaScript"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript"></a>
          <a href="https://www.typescriptlang.org/" aria-label="TypeScript"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="TypeScript"></a>
        </div>
      </div>
      <div class="technology-group">
        <h2>Databases</h2>
        <div class="logo-list">
          <a href="https://www.mongodb.com/" aria-label="MongoDB"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original.svg" alt="MongoDB"></a>
          <a href="https://www.mysql.com/" aria-label="MySQL"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original.svg" alt="MySQL"></a>
        </div>
      </div>
      <div class="technology-group">
        <h2>Frontend</h2>
        <div class="logo-list">
          <a href="https://react.dev/" aria-label="React"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" alt="React"></a>
          <a href="https://redux.js.org/" aria-label="Redux"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redux/redux-original.svg" alt="Redux"></a>
          <a href="https://sass-lang.com/" aria-label="Sass"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/sass/sass-original.svg" alt="Sass"></a>
        </div>
      </div>
      <div class="technology-group">
        <h2>Backend &amp; Tools</h2>
        <div class="logo-list">
          <a href="https://nodejs.org/" aria-label="Node.js"><img class="wordmark" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original-wordmark.svg" alt="Node.js"></a>
          <a href="https://expressjs.com/" aria-label="Express"><img class="wordmark" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/express/express-original-wordmark.svg" alt="Express"></a>
          <a href="https://git-scm.com/" aria-label="Git"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git"></a>
        </div>
      </div>
    </section>
  </main>
</body>

