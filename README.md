<style>
  @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');

  .profile-container {
    max-width: 900px;
    margin: 0 auto;
    padding: 40px;
    background: linear-gradient(135deg, #1a1a1a, #2a2a2a);
    color: #f0f0f0;
    font-family: 'Orbitron', sans-serif;
    position: relative;
    overflow: hidden;
  }

  .dynamic-background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: radial-gradient(circle, rgba(0,170,255,0.1) 0%, transparent 70%);
    animation: pulse 10s infinite alternate;
    pointer-events: none;
  }

  @keyframes pulse {
    0% { transform: scale(1); opacity: 0.5; }
    100% { transform: scale(1.2); opacity: 0.8; }
  }

  .profile-header {
    text-align: center;
    margin-bottom: 40px;
    position: relative;
    z-index: 1;
  }

  .profile-header h1 {
    font-size: 3em;
    color: #00aaff;
    animation: glow 2s infinite alternate;
  }

  @keyframes glow {
    from { text-shadow: 0 0 5px #00aaff, 0 0 10px #00aaff; }
    to { text-shadow: 0 0 20px #00aaff, 0 0 30px #00aaff; }
  }

  .profile-header h3 {
    font-size: 1.5em;
    color: #ccc;
    animation: fadeInUp 1s ease-in;
  }

  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .section {
    background-color: rgba(51, 51, 51, 0.8);
    padding: 30px;
    border-radius: 15px;
    margin-bottom: 30px;
    position: relative;
    z-index: 1;
    transition: transform 0.3s, box-shadow 0.3s;
  }

  .section:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 20px rgba(0,170,255,0.2);
  }

  .section h2 {
    color: #00aaff;
    border-bottom: 2px solid #444;
    padding-bottom: 10px;
    position: relative;
  }

  .section h2::after {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 0;
    height: 2px;
    background-color: #00aaff;
    animation: underline 2s infinite;
  }

  @keyframes underline {
    0% { width: 0; }
    50% { width: 100%; }
    100% { width: 0; }
  }

  .icon-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(60px, 1fr));
    gap: 20px;
    justify-items: center;
  }

  .icon-container img {
    width: 50px;
    height: 50px;
    transition: transform 0.3s, filter 0.3s;
  }

  .icon-container img:hover {
    transform: rotate(15deg) scale(1.2);
    filter: drop-shadow(0 0 10px #00aaff);
  }

  .project-link {
    display: inline-block;
    padding: 10px 20px;
    background-color: #00aaff;
    color: #fff;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s, transform 0.3s;
  }

  .project-link:hover {
    background-color: #0088cc;
    transform: scale(1.05);
  }

  .footer {
    text-align: center;
    margin-top: 40px;
    font-size: 0.9em;
    color: #888;
    position: relative;
    z-index: 1;
  }

  .footer::before {
    content: '';
    position: absolute;
    top: -10px;
    left: 50%;
    transform: translateX(-50%);
    width: 50px;
    height: 2px;
    background-color: #00aaff;
  }
</style>

<div class="profile-container">
  <div class="dynamic-background"></div>
  
  <div class="profile-header">
    <h1>👋 Hi, I’m Dipesh Regmi</h1>
    <h3>A passionate Computer Engineer with a foundation in scripting, automation, and backend development.</h3>
  </div>
  
  <div class="section about-me">
    <h2>About Me</h2>
    <p>I'm a computer engineer with a keen interest in backend development, automation, and machine learning. I enjoy solving complex problems and building efficient systems.</p>
  </div>
  
  <div class="section current-project">
    <h2>🔭 Current Project</h2>
    <p><a href="https://github.com/dipesh7002/AHelp" class="project-link">AHelp</a> - Matching service providers with students seeking thesis and dissertation help.</p>
  </div>
  
  <div class="section learning">
    <h2>🌱 Learning</h2>
    <p>Fine-tuning LLMs: LoRA, prompt engineering, Hugging Face.</p>
  </div>
  
  <div class="section contact">
    <h2>📫 Contact</h2>
    <p>✉️ <code>077bct027.dipesh@pcampus.edu.np</code></p>
  </div>
  
  <div class="section social-links">
    <h2>🔗 Connect with me</h2>
    <div class="icon-container">
      <a href="https://linkedin.com/in/dipesh-regmi-941bab32b" target="_blank">
        <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" title="LinkedIn" />
      </a>
      <a href="https://leetcode.com/user1063ha" target="_blank">
        <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/leet-code.svg" alt="LeetCode" title="LeetCode" />
      </a>
    </div>
  </div>
  
  <div class="section languages">
    <h2>📝 Programming Languages</h2>
    <div class="icon-container">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/c/c-original.svg" alt="C" title="C" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/cplusplus/cplusplus-original.svg" alt="C++" title="C++" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" title="Python" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" title="JavaScript" />
      <img src="https://www.vectorlogo.zone/logos/kotlinlang/kotlinlang-icon.svg" alt="Kotlin" title="Kotlin" />
    </div>
  </div>
  
  <div class="section web-technologies">
    <h2>🌐 Web Technologies</h2>
    <div class="icon-container">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="HTML5" title="HTML5" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="CSS3" title="CSS3" />
    </div>
  </div>
  
  <div class="section databases">
    <h2>🗄️ Databases</h2>
    <div class="icon-container">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original-wordmark.svg" alt="PostgreSQL" title="PostgreSQL" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="MySQL" title="MySQL" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mongodb/mongodb-original-wordmark.svg" alt="MongoDB" title="MongoDB" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/0d6c64dbbf311879f7d563bfc3ccf559f9ed111c/icons/couchdb/couchdb-original.svg" alt="CouchDB" title="CouchDB" />
    </div>
  </div>
  
  <div class="section tools">
    <h2>🛠️ Tools</h2>
    <div class="icon-container">
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/django/django-original.svg" alt="Django" title="Django" />
      <img src="https://www.vectorlogo.zone/logos/elastic/elastic-icon.svg" alt="Elasticsearch" title="Elasticsearch" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg" alt="Git" title="Git" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="Linux" title="Linux" />
      <img src="https://upload.wikimedia.org/wikipedia/commons/2/21/Matlab_Logo.png" alt="MATLAB" title="MATLAB" />
      <img src="https://raw.githubusercontent.com/devicons/devicon/2ae2a900d2f041da66e950e4d48052658d850630/icons/pandas/pandas-original.svg" alt="Pandas" title="Pandas" />
    </div>
  </div>
  
  <div class="footer">
    <p>© 2025 Dipesh Regmi. All rights reserved.</p>
  </div>
</div>
