<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Dipesh Regmi - Animated Profile</title>
  <style>
    /* Root variables for easy customization */
    :root {
      --primary: #2196f3;
      --secondary: #ffc107;
      --accent: #e91e63;
      --bg-dark: #0d1117;
      --text-light: #c9d1d9;
    }

    /* Basic reset */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: var(--bg-dark);
      color: var(--text-light);
      overflow-x: hidden;
      line-height: 1.6;
    }

    a {
      color: var(--primary);
      text-decoration: none;
      position: relative;
      overflow: hidden;
    }

    a::after {
      content: '';
      position: absolute;
      width: 100%;
      height: 2px;
      background: var(--secondary);
      bottom: 0;
      left: -100%;
      transition: left 0.3s ease;
    }

    a:hover::after {
      left: 0;
    }

    header {
      padding: 100px 20px;
      text-align: center;
      position: relative;
      overflow: hidden;
    }

    /* Animated gradient background */
    header::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: linear-gradient(45deg,
          var(--primary), var(--secondary), var(--accent), var(--primary));
      background-size: 600% 600%;
      animation: gradientShift 20s ease infinite;
      z-index: -1;
    }

    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    h1 {
      font-size: 3em;
      margin-bottom: 0.2em;
      animation: fadeInDown 1s ease both;
    }

    h3 {
      font-size: 1.5em;
      margin-bottom: 0.5em;
      animation: fadeInUp 1s ease both;
    }

    @keyframes fadeInDown { from { opacity: 0; transform: translateY(-30px); } to { opacity: 1; transform: translateY(0); } }
    @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }

    /* Profile badge container */
    .badge {
      margin: 20px auto;
      width: 120px;
      border-radius: 50%;
      overflow: hidden;
      animation: rotateBadge 10s linear infinite;
    }

    .badge img {
      width: 100%;
      display: block;
    }

    @keyframes rotateBadge {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }

    .content {
      max-width: 800px;
      margin: 0 auto;
      padding: 40px 20px;
    }

    section {
      margin-bottom: 60px;
    }

    section h2 {
      border-left: 4px solid var(--accent);
      padding-left: 10px;
      margin-bottom: 20px;
      font-size: 2em;
    }

    .card-list {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 20px;
    }

    .card {
      background: #161b22;
      border-radius: 12px;
      padding: 20px;
      position: relative;
      overflow: hidden;
      cursor: pointer;
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-10px);
    }

    .card::before {
      content: '';
      position: absolute;
      top: -50%; left: -50%;
      width: 200%; height: 200%;
      background: radial-gradient(circle, rgba(33,150,243,0.2) 20%, transparent 20%);
      background-size: 50px 50px;
      animation: pulse 4s linear infinite;
      z-index: 0;
    }

    @keyframes pulse {
      0% { transform: scale(0.8); }
      50% { transform: scale(1.2); }
      100% { transform: scale(0.8); }
    }

    .card-content {
      position: relative;
      z-index: 1;
      text-align: center;
    }

    .card img {
      width: 40px;
      height: 40px;
      margin-bottom: 10px;
    }

    /* Marquee style for "Connect with me" */
    .marquee {
      overflow: hidden;
      white-space: nowrap;
      box-sizing: border-box;
      animation: marqueeAnim 15s linear infinite;
    }

    .marquee a {
      display: inline-block;
      margin: 0 30px;
      animation: linkPop 1s ease infinite;
    }

    @keyframes marqueeAnim {
      0% { transform: translateX(100%); }
      100% { transform: translateX(-100%); }
    }

    @keyframes linkPop {
      0%,100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }
  </style>
</head>

<body>

  <header>
    <div class="badge">
      <img src="https://komarev.com/ghpvc/?username=dipesh7002&color=blue" alt="Profile views" />
    </div>
    <h1>👋 Hi, I’m <strong>Dipesh Regmi</strong></h1>
    <h3>A passionate Computer Engineer with a foundation in scripting, automation, and backend development.</h3>
  </header>

  <div class="content">

    <section>
      <h2>🔭 Current Project</h2>
      <div class="card-list">
        <div class="card">
          <div class="card-content">
            <img src="https://github.githubassets.com/favicons/favicon.svg" alt="GitHub" />
            <p><strong><a href="https://github.com/dipesh7002/AHelp" target="_blank">AHelp</a></strong></p>
            <p>Matching service providers with students seeking thesis and dissertation help.</p>
          </div>
        </div>
      </div>
    </section>

    <section>
      <h2>🌱 Learning</h2>
      <div class="card-list">
        <div class="card">
          <div class="card-content">
            <img src="https://huggingface.co/front/assets/huggingface_logo.svg" alt="Hugging Face" />
            <p>LoRA Fine-tuning</p>
          </div>
        </div>
        <div class="card">
          <div class="card-content">
            <img src="https://raw.githubusercontent.com/get-icon/geticon/master/icons/prompt.svg" alt="Prompt Engineering" />
            <p>Prompt Engineering</p>
          </div>
        </div>
      </div>
    </section>

    <section>
      <h2>📫 Contact</h2>
      <p>✉️ <code>077bct027.dipesh@pcampus.edu.np</code></p>
    </section>

    <section>
      <h2>🔗 Connect with me</h2>
      <div class="marquee">
        <a href="https://linkedin.com/in/dipesh-regmi-941bab32b" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" width="30" height="30" alt="LinkedIn" /></a>
        <a href="https://leetcode.com/user1063ha" target="_blank"><img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" width="30" height="30" alt="LeetCode" /></a>
      </div>
    </section>

    <section>
      <h2>📝 Languages</h2>
      <div class="card-list">
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="C" /><p>C</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="C++" /><p>C++</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" /><p>Python</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" /><p>JavaScript</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5" /><p>HTML5</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3" /><p>CSS3</p></div></div>
        <div class="card"><div class="card-content"><img src="https://www.vectorlogo.zone/logos/kotlinlang/kotlinlang-icon.svg" alt="Kotlin" /><p>Kotlin</p></div></div>
      </div>
    </section>

    <section>
      <h2>🛠️ Tools & Technologies</h2>
      <div class="card-list">
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/django/django-original.svg" alt="Django" /><p>Django</p></div></div>
        <div class="card"><div class="card-content"><img src="https://www.vectorlogo.zone/logos/elastic/elastic-icon.svg" alt="Elasticsearch" /><p>Elasticsearch</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git" /><p>Git</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="Linux" /><p>Linux</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="PostgreSQL" /><p>PostgreSQL</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="MySQL" /><p>MySQL</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="MongoDB" /><p>MongoDB</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/0d6c64dbbf311879f7d563bfc3ccf559f9ed111c/icons/couchdb/couchdb-original.svg" alt="CouchDB" /><p>CouchDB</p></div></div>
        <div class="card"><div class="card-content"><img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png" alt="MATLAB" /><p>MATLAB</p></div></div>
        <div class="card"><div class="card-content"><img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="Pandas" /><p>Pandas</p></div></div>
      </div>
    </section>

  </div>

</body>

</html>
