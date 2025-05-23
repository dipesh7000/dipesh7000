<!-- Animated Background Elements -->
<div align="center">
  <svg width="0" height="0" style="position: absolute;">
    <defs>
      <filter id="goo">
        <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur" />
        <feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -7" result="goo" />
      </filter>
    </defs>
  </svg>
  <div style="position: absolute; width: 100%; height: 100%; filter: url(#goo); pointer-events: none;">
    <div style="position: absolute; width: 50px; height: 50px; background: #ff6b6b; border-radius: 50%; top: 20%; left: 10%; animation: float 8s infinite;"></div>
    <div style="position: absolute; width: 40px; height: 40px; background: #4ecdc4; border-radius: 50%; top: 60%; right: 15%; animation: float 6s infinite 2s;"></div>
  </div>
</div>

<!-- Main Container -->
<div align="center" style="position: relative; padding: 3rem; overflow: hidden;">
  <style>
    @keyframes hologram {
      0% { transform: rotateX(0deg) rotateY(0deg); }
      25% { transform: rotateX(5deg) rotateY(5deg); }
      50% { transform: rotateX(-5deg) rotateY(-5deg); }
      75% { transform: rotateX(3deg) rotateY(-3deg); }
      100% { transform: rotateX(0deg) rotateY(0deg); }
    }
    @keyframes chromatic {
      0% { text-shadow: 3px 0px 0px cyan, -3px 0px 0px magenta; }
      50% { text-shadow: 5px 2px 0px cyan, -5px -2px 0px magenta; }
      100% { text-shadow: 3px 0px 0px cyan, -3px 0px 0px magenta; }
    }
    .hover-3d { transition: transform 0.3s; }
    .hover-3d:hover { transform: perspective(1000px) rotateX(5deg) rotateY(5deg); }
  </style>

  <!-- Floating Avatar -->
  <div style="position: relative; animation: float 4s ease-in-out infinite;">
    <div style="width: 120px; height: 120px; background: linear-gradient(45deg, #ff6b6b, #4ecdc4); border-radius: 50%; position: relative;">
      <div style="position: absolute; width: 100%; height: 100%; border: 2px solid white; border-radius: 50%; animation: hologram 8s infinite;"></div>
      <div style="position: absolute; width: 100%; height: 100%; border: 2px solid rgba(255,255,255,0.3); border-radius: 50%; animation: hologram 6s infinite reverse;"></div>
    </div>
  </div>

  <!-- Name with Chromatic Effect -->
  <h1 style="font-family: 'Courier New', monospace; margin: 1rem 0; animation: chromatic 4s infinite;">
    <span style="background: linear-gradient(45deg, #ff6b6b, #4ecdc4); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
      DIPESH REGMI
    </span>
  </h1>

  <!-- Animated Terminal Effect -->
  <div style="background: #1a1a1a; padding: 1.5rem; border-radius: 10px; text-align: left; width: 70%; margin: 2rem auto; position: relative;">
    <div style="position: absolute; top: 0; left: 0; right: 0; height: 30px; background: #2d2d2d; border-radius: 10px 10px 0 0; display: flex; align-items: center; padding: 0 1rem;">
      <div style="display: flex; gap: 0.5rem;">
        <div style="width: 12px; height: 12px; background: #ff5f56; border-radius: 50%;"></div>
        <div style="width: 12px; height: 12px; background: #ffbd2e; border-radius: 50%;"></div>
        <div style="width: 12px; height: 12px; background: #27c93f; border-radius: 50%;"></div>
      </div>
    </div>
    <div style="margin-top: 2.5rem; color: #00ff00; font-family: 'Courier New', monospace;">
      <span style="animation: blink 1s infinite;">▋</span> Building intelligent solutions with passion
    </div>
  </div>

  <!-- Holographic Cards Grid -->
  <div style="display: grid; grid-template-columns: repeat(2, 1fr); gap: 2rem; margin: 3rem 0; width: 80%;">
    <!-- Project Card -->
    <div class="hover-3d" style="background: rgba(255,255,255,0.1); padding: 1.5rem; border-radius: 15px; backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.2);">
      <h3 style="margin: 0 0 1rem; color: #4ecdc4;">🚀 Active Project</h3>
      <div style="position: relative;">
        <div style="position: absolute; width: 100%; height: 100%; border: 1px solid rgba(78,205,196,0.3); border-radius: 10px; top: 5px; left: 5px;"></div>
        <div style="background: #2d2d2d; padding: 1rem; border-radius: 10px;">
          <h4 style="margin: 0; color: #ff6b6b;">AHelp Platform</h4>
          <p style="color: #a0a0a0; font-size: 0.9rem;">AI-powered academic collaboration system</p>
          <div style="display: flex; gap: 0.5rem; margin-top: 1rem;">
            <div style="width: 10px; height: 10px; background: #4ecdc4; border-radius: 50%;"></div>
            <div style="width: 10px; height: 10px; background: #ff6b6b; border-radius: 50%;"></div>
            <div style="width: 10px; height: 10px; background: #45b649; border-radius: 50%;"></div>
          </div>
        </div>
      </div>
    </div>

    <!-- Skills Card -->
    <div class="hover-3d" style="background: rgba(255,255,255,0.1); padding: 1.5rem; border-radius: 15px; backdrop-filter: blur(10px); border: 1px solid rgba(255,255,255,0.2);">
      <h3 style="margin: 0 0 1rem; color: #ff6b6b;">🛠 Core Arsenal</h3>
      <div style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 1rem;">
        <div style="text-align: center;">
          <div style="width: 50px; height: 50px; background: #2d2d2d; border-radius: 10px; margin: 0 auto; display: grid; place-items: center;">
            <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="30" style="filter: drop-shadow(0 0 5px #4ecdc4);"/>
          </div>
          <p style="margin: 0.5rem 0 0; font-size: 0.8rem;">Python</p>
        </div>
        <!-- Add more skill items -->
      </div>
    </div>
  </div>

  <!-- Animated Connection Lines -->
  <div style="position: relative; height: 100px; margin: 2rem 0;">
    <div style="position: absolute; height: 2px; background: linear-gradient(90deg, #ff6b6b, #4ecdc4); width: 100%; top: 50%; animation: lineFlow 3s infinite;">
      <div style="position: absolute; width: 20px; height: 20px; background: #4ecdc4; border-radius: 50%; right: -10px; top: -9px; animation: pulse 1.5s infinite;"></div>
    </div>
  </div>

  <!-- Neural Network Animation -->
  <div style="position: relative; height: 150px; margin: 3rem 0;">
    <div style="position: absolute; width: 100%; height: 100%; display: flex; justify-content: space-between;">
      <div style="width: 30%; position: relative;">
        <!-- Nodes and connections -->
        <div style="position: absolute; width: 15px; height: 15px; background: #ff6b6b; border-radius: 50%; top: 20%; left: 30%; animation: nodePulse 2s infinite;"></div>
        <div style="position: absolute; width: 15px; height: 15px; background: #4ecdc4; border-radius: 50%; top: 50%; left: 60%; animation: nodePulse 2s infinite 0.5s;"></div>
        <!-- Add more nodes and animated connection lines -->
      </div>
    </div>
  </div>

  <!-- Animated Contact Button -->
  <div style="position: relative; margin: 2rem 0;">
    <a href="mailto:077bct027.dipesh@pcampus.edu.np" style="text-decoration: none; position: relative;">
      <div style="padding: 1rem 2rem; background: linear-gradient(45deg, #ff6b6b, #4ecdc4); border-radius: 50px; color: white; font-weight: bold; position: relative; overflow: hidden;">
        <div style="position: absolute; width: 100%; height: 100%; background: linear-gradient(45deg, transparent 50%, rgba(255,255,255,0.2) 50%); background-size: 400% 400%; animation: shine 3s infinite;"></div>
        <span style="position: relative;">📧 Let's Connect!</span>
      </div>
    </a>
  </div>
</div>

<style>
  @keyframes nodePulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.2); }
    100% { transform: scale(1); }
  }
  @keyframes lineFlow {
    0% { background-position: 0% 50%; }
    100% { background-position: 100% 50%; }
  }
  @keyframes shine {
    0% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }
  @keyframes pulse {
    0% { transform: scale(1); opacity: 1; }
    100% { transform: scale(2); opacity: 0; }
  }
  @keyframes blink {
    0%, 100% { opacity: 1; }
    50% { opacity: 0; }
  }
</style>
