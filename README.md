```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Jabez Celestial | Video Editor & Creative Freelancer</title>

  <meta name="description" content="Jabez Celestial — Video editor, clip editor, thumbnail designer, and creative freelancer. Get a free sample edit to see the quality first.">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #070b14;
      color: #f5f7ff;
      line-height: 1.6;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* NAVIGATION */
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      padding: 18px 7%;
      background: rgba(7, 11, 20, 0.85);
      backdrop-filter: blur(15px);
      border-bottom: 1px solid rgba(255,255,255,0.08);

      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 25px;
      font-weight: 900;
      letter-spacing: 2px;
      color: #73b9ff;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 28px;
    }

    nav a {
      color: #b9c2d9;
      font-size: 14px;
      transition: 0.3s;
    }

    nav a:hover {
      color: #73b9ff;
    }

    /* HERO */
    .hero {
      min-height: 100vh;
      padding: 150px 7% 80px;

      display: flex;
      align-items: center;
      justify-content: center;
    }

    .hero-container {
      max-width: 1150px;
      width: 100%;

      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 60px;
      align-items: center;
    }

    .tag {
      display: inline-block;
      padding: 8px 15px;
      border-radius: 30px;
      background: rgba(115,185,255,0.1);
      border: 1px solid rgba(115,185,255,0.3);
      color: #73b9ff;
      font-size: 13px;
      margin-bottom: 22px;
    }

    h1 {
      font-size: clamp(45px, 7vw, 80px);
      line-height: 0.98;
      margin-bottom: 25px;
    }

    h1 span {
      color: #73b9ff;
    }

    .hero p {
      color: #aeb8ce;
      font-size: 18px;
      max-width: 650px;
      margin-bottom: 30px;
    }

    .buttons {
      display: flex;
      gap: 15px;
      flex-wrap: wrap;
    }

    .btn {
      padding: 14px 23px;
      border-radius: 10px;
      font-weight: 700;
      transition: 0.3s;
      display: inline-block;
    }

    .btn-primary {
      background: #73b9ff;
      color: #07101d;
    }

    .btn-primary:hover {
      transform: translateY(-3px);
      box-shadow: 0 10px 30px rgba(115,185,255,0.25);
    }

    .btn-outline {
      border: 1px solid #34415c;
      color: #e9edfa;
    }

    .btn-outline:hover {
      border-color: #73b9ff;
      color: #73b9ff;
    }

    /* VIDEO */
    .video-card {
      background: #0d1322;
      border: 1px solid #202b42;
      padding: 12px;
      border-radius: 20px;
      box-shadow: 0 25px 80px rgba(0,0,0,0.4);
    }

    .video-card video {
      width: 100%;
      display: block;
      border-radius: 13px;
      background: #000;
    }

    .video-label {
      padding: 15px 8px 5px;
      color: #9eabc4;
      font-size: 13px;
    }

    /* SECTIONS */
    section {
      padding: 100px 7%;
    }

    .section-container {
      max-width: 1100px;
      margin: auto;
    }

    .section-title {
      font-size: 40px;
      margin-bottom: 15px;
    }

    .section-subtitle {
      color: #8f9bb4;
      margin-bottom: 45px;
    }

    /* FREE SAMPLE */
    .free-sample {
      background: linear-gradient(
        135deg,
        rgba(115,185,255,0.12),
        rgba(115,185,255,0.02)
      );

      border: 1px solid rgba(115,185,255,0.25);
      border-radius: 25px;
      padding: 50px;
      text-align: center;
    }

    .free-sample h2 {
      font-size: 38px;
      margin-bottom: 15px;
    }

    .free-sample h2 span {
      color: #73b9ff;
    }

    .free-sample p {
      color: #aeb8ce;
      max-width: 700px;
      margin: 0 auto 28px;
    }

    /* SERVICES */
    .services {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 20px;
    }

    .service {
      background: #0d1322;
      border: 1px solid #202b42;
      border-radius: 18px;
      padding: 30px;
      transition: 0.3s;
    }

    .service:hover {
      transform: translateY(-7px);
      border-color: #73b9ff;
    }

    .service-icon {
      font-size: 35px;
      margin-bottom: 18px;
    }

    .service h3 {
      margin-bottom: 10px;
    }

    .service p {
      color: #8f9bb4;
      font-size: 14px;
    }

    /* ABOUT */
    .about {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
      align-items: center;
    }

    .about p {
      color: #aeb8ce;
      margin-bottom: 18px;
    }

    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .skill {
      padding: 10px 14px;
      border-radius: 8px;
      background: #111a2c;
      border: 1px solid #25334d;
      color: #b9c8df;
      font-size: 13px;
    }

    /* CONTACT */
    .contact-box {
      text-align: center;
      background: #0d1322;
      border: 1px solid #202b42;
      border-radius: 25px;
      padding: 60px 30px;
    }

    .contact-box h2 {
      font-size: 45px;
      margin-bottom: 15px;
    }

    .contact-box p {
      color: #9ca8c0;
      margin-bottom: 30px;
    }

    .contact-info {
      margin-top: 30px;
      color: #aeb8ce;
      line-height: 2;
    }

    .contact-info a {
      color: #73b9ff;
    }

    /* FOOTER */
    footer {
      text-align: center;
      padding: 35px;
      color: #65718a;
      border-top: 1px solid #182238;
      font-size: 13px;
    }

    /* MOBILE */
    @media (max-width: 850px) {

      nav ul {
        display: none;
      }

      .hero-container,
      .about {
        grid-template-columns: 1fr;
      }

      .services {
        grid-template-columns: 1fr;
      }

      .hero {
        padding-top: 130px;
      }

      .free-sample {
        padding: 35px 20px;
      }

      .contact-box h2 {
        font-size: 35px;
      }
    }
  </style>
</head>

<body>

  <!-- NAVIGATION -->
  <nav>
    <div class="logo">JABEZ.</div>

    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>


  <!-- HERO -->
  <section class="hero" id="home">

    <div class="hero-container">

      <div>

        <div class="tag">
          AVAILABLE FOR FREELANCE WORK
        </div>

        <h1>
          I turn raw footage into
          <span>content people want to watch.</span>
        </h1>

        <p>
          Hi, I'm Jabez Celestial — a video editor and creative freelancer
          specializing in short-form content, clip editing, and thumbnail design.
          I help creators and businesses turn their ideas and raw footage into
          engaging content.
        </p>

        <div class="buttons">

          <a
            href="mailto:jabezcelestial1@gmail.com?subject=Free%20Sample%20Edit%20Request"
            class="btn btn-primary">
            📩 Ready to Email Me
          </a>

          <a href="#services" class="btn btn-outline">
            View My Services
          </a>

        </div>

      </div>


      <!-- INTRO VIDEO -->
      <div class="video-card">

        <video controls preload="metadata">

          <source
            src="https://drive.google.com/uc?export=download&id=1krnjUceYq6baD6NB08m4B793hSSRxLjz"
            type="video/mp4">

          Your browser does not support the video tag.

        </video>

        <div class="video-label">
          ▶ Watch my introduction
        </div>

      </div>

    </div>

  </section>


  <!-- FREE SAMPLE -->
  <section>

    <div class="section-container">

      <div class="free-sample">

        <h2>
          Let me prove the quality <span>first.</span>
        </h2>

        <p>
          Not ready to commit yet? No problem.
          Send me your footage and I'll create a small sample edit for free.
          You can see my editing style, pacing, captions, and overall quality
          before deciding to work with me.
        </p>

        <a
          href="mailto:jabezcelestial1@gmail.com?subject=Free%20Sample%20Edit"
          class="btn btn-primary">
          🎬 Request a Free Sample
        </a>

      </div>

    </div>

  </section>


  <!-- SERVICES -->
  <section id="services">

    <div class="section-container">

      <h2 class="section-title">
        What I Can Do
      </h2>

      <p class="section-subtitle">
        Creative services designed for creators, brands, and businesses.
      </p>


      <div class="services">

        <div class="service">

          <div class="service-icon">🎬</div>

          <h3>Video Editing</h3>

          <p>
            Clean, engaging edits with strong pacing, cuts, transitions,
            captions, sound effects, and visual elements.
          </p>

        </div>


        <div class="service">

          <div class="service-icon">⚡</div>

          <h3>Short-Form Clips</h3>

          <p>
            Transform long-form videos, podcasts, interviews, and recordings
            into engaging short-form content for social media.
          </p>

        </div>


        <div class="service">

          <div class="service-icon">🖼️</div>

          <h3>Thumbnail Design</h3>

          <p>
            Attention-grabbing thumbnails designed to communicate the idea
            quickly and encourage viewers to click.
          </p>

        </div>

      </div>

    </div>

  </section>


  <!-- ABOUT -->
  <section id="about">

    <div class="section-container">

      <div class="about">

        <div>

          <div class="tag">
            ABOUT ME
          </div>

          <h2 class="section-title">
            Creative. Adaptable. Always learning.
          </h2>

          <p>
            I'm Jabez Celestial, a college student pursuing a Bachelor of
            Science in Information Systems.
          </p>

          <p>
            Alongside my studies, I'm building my skills in video editing,
            thumbnail design, content creation, and digital work.
          </p>

          <p>
            I'm focused on delivering useful, clean, and engaging work while
            continuously improving with every project.
          </p>

        </div>


        <div>

          <h3 style="margin-bottom:20px;">
            My Skills
          </h3>

          <div class="skills">

            <div class="skill">Video Editing</div>
            <div class="skill">Short-Form Content</div>
            <div class="skill">Clip Editing</div>
            <div class="skill">Thumbnail Design</div>
            <div class="skill">CapCut</div>
            <div class="skill">Canva</div>
            <div class="skill">AI Tools</div>
            <div class="skill">Creative Editing</div>
            <div class="skill">Content Research</div>
            <div class="skill">Communication</div>

          </div>

        </div>

      </div>

    </div>

  </section>


  <!-- CONTACT -->
  <section id="contact">

    <div class="section-container">

      <div class="contact-box">

        <div class="tag">
          LET'S WORK TOGETHER
        </div>

        <h2>
          Have footage?
          <br>
          Let's make something great.
        </h2>

        <p>
          Send me your project details or footage and let's discuss
          what I can create for you.
        </p>

        <a
          href="mailto:jabezcelestial1@gmail.com?subject=Video%20Editing%20Project"
          class="btn btn-primary">
          📩 Ready to Email Me
        </a>


        <div class="contact-info">

          📧
          <a href="mailto:jabezcelestial1@gmail.com">
            jabezcelestial1@gmail.com
          </a>

          <br>

          📱
          <a href="tel:+639949721920">
            0994 972 1920
          </a>

          <br>

          💼
          <a
            href="https://www.linkedin.com/in/jabez-celestial-460b7a390"
            target="_blank">
            LinkedIn Profile
          </a>

        </div>

      </div>

    </div>

  </section>


  <!-- FOOTER -->
  <footer>

    © 2026 Jabez Celestial. All rights reserved.

    <br>

    Video Editing • Short-Form Content • Thumbnail Design

  </footer>

</body>
</html>
```
