<div align="center">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Aileron&family=Helvetica+Neue');

    :root {
      --color-primary-1: #FFFB00;
      --color-primary-2: #00FFFB;
      --color-accent: #FB00FF;
      --anim-duration: 25s; /* Total animation duration */
      --step-duration: calc(var(--anim-duration) / 7); /* Duration per step (7 interests) */
    }

    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 150px; /* Adjust height as needed */
      overflow: hidden;
      font-family: 'Aileron', 'Helvetica Neue', sans-serif;
      font-size: 3.5em;
      color: var(--color-primary-1);
      text-shadow: 0 0 10px var(--color-primary-2), 0 0 20px var(--color-primary-2);
    }

    .interests h1 {
      opacity: 0;
      position: absolute;
      text-align: center;
      width: 100%;
      animation:
        typing var(--step-duration) steps(20, end) infinite,
        flicker 1.5s step-end infinite,
        fade-out var(--step-duration) forwards infinite;
      animation-delay: 0s;
    }

    .interests h1:nth-child(1) { animation-delay: 0s, 0s, 0s; }
    .interests h1:nth-child(2) { animation-delay: calc(var(--step-duration) * 1), calc(var(--step-duration) * 1), calc(var(--step-duration) * 1); }
    .interests h1:nth-child(3) { animation-delay: calc(var(--step-duration) * 2), calc(var(--step-duration) * 2), calc(var(--step-duration) * 2); }
    .interests h1:nth-child(4) { animation-delay: calc(var(--step-duration) * 3), calc(var(--step-duration) * 3), calc(var(--step-duration) * 3); }
    .interests h1:nth-child(5) { animation-delay: calc(var(--step-duration) * 4), calc(var(--step-duration) * 4), calc(var(--step-duration) * 4); }
    .interests h1:nth-child(6) { animation-delay: calc(var(--step-duration) * 5), calc(var(--step-duration) * 5), calc(var(--step-duration) * 5); }
    .interests h1:nth-child(7) { animation-delay: calc(var(--step-duration) * 6), calc(var(--step-duration) * 6), calc(var(--step-duration) * 6); }

    /* Typing Animation */
    @keyframes typing {
      0%, 10% { opacity: 1; width: 0; }
      10%, 80% { opacity: 1; width: 100%; }
      80%, 100% { opacity: 0; width: 100%; }
    }

    /* Flicker Animation */
    @keyframes flicker {
      0%, 19.99%, 22%, 62.99%, 64%, 69.99%, 71%, 100% {
        text-shadow: 0 0 10px var(--color-primary-2), 0 0 20px var(--color-primary-2);
        color: var(--color-primary-1);
      }
      20%, 21.99%, 63%, 63.99%, 70%, 70.99% {
        text-shadow: none;
        color: var(--color-primary-2);
      }
    }

  </style>

  <div class="container">
    <div class="interests">
      <h1>Comp Sci</h1>
      <h1>DECA</h1>
      <h1>Robotics</h1>
      <h1>Web Design</h1>
      <h1>YouTube Channel (@ROHAN-MODI)</h1>
      <h1>Tech</h1>
      <h1>Writing Tech News (at TecRes)</h1>
    </div>
  </div>

  <p>Hello, my name's Rohan. I'm passionate about tech and creating things! </p>
  
  </div>
