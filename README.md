# Cybers-Security
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Kenzo | Ethical Hacker</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <style>
    /* Animated Gradient Background */
    body {
      background: linear-gradient(-45deg, #0f172a, #1e293b, #0c4a6e, #1e3a8a);
      background-size: 400% 400%;
      animation: gradientMove 15s ease infinite;
      font-family: 'Courier New', monospace;
      color: #e2e8f0;
    }
    @keyframes gradientMove {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    /* Neon Border Glow */
    .card {
      border: 1px solid #00fff7;
      border-radius: 0.5rem;
      padding: 1rem;
      background-color: rgba(15, 23, 42, 0.8);
      position: relative;
      overflow: hidden;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .card::before {
      content: "";
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: conic-gradient(
        from 0deg,
        #00fff7,
        transparent,
        #00fff7,
        transparent
      );
      animation: spin 6s linear infinite;
      z-index: 0;
    }
    .card > * {
      position: relative;
      z-index: 1;
    }
    .card:hover {
      transform: scale(1.03);
      box-shadow: 0 0 20px #00fff7;
    }
    @keyframes spin {
      100% { transform: rotate(360deg); }
    }

    /* Floating Particles */
    .particles {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      z-index: -1;
      overflow: hidden;
    }
    .particle {
      position: absolute;
      width: 4px; height: 4px;
      background: #00fff7;
      border-radius: 50%;
      opacity: 0.6;
      animation: float 12s linear infinite;
    }
    @keyframes float {
      from { transform: translateY(100vh) scale(0.5); opacity: 0; }
      20% { opacity: 1; }
      to { transform: translateY(-10vh) scale(1); opacity: 0; }
    }
  </style>
</head>
<body>
  <!-- Floating Particles -->
  <div class="particles">
    <div class="particle" style="left: 10%; animation-delay: 0s;"></div>
    <div class="particle" style="left: 30%; animation-delay: 2s;"></div>
    <div class="particle" style="left: 50%; animation-delay: 4s;"></div>
    <div class="particle" style="left: 70%; animation-delay: 6s;"></div>
    <div class="particle" style="left: 90%; animation-delay: 8s;"></div>
  </div>

  <main class="max-w-sm mx-auto px-4 py-6 space-y-6">
    <!-- Header -->
    <header class="text-center" data-aos="fade-down">
      <h1 class="text-xl font-bold text-cyan-400">Kenzo — Ethical Hacker</h1>
      <p class="text-sm text-slate-400">Security Researcher & Pentester</p>
    </header>

    <!-- About -->
    <section class="card" data-aos="fade-up">
      <h2 class="text-base font-bold text-cyan-300 mb-2">About Me</h2>
      <p class="text-xs text-slate-300">Saya Kenzo, fokus dalam keamanan siber & ethical hacking. 
      Tujuan saya adalah mengamankan sistem dan berbagi pengetahuan dengan komunitas.</p>
      <div class="mt-2 text-xs">
        <div><strong>Email:</strong> <a href="mailto:pykcyber@gmail.com" class="underline">pykcyber@gmail.com</a></div>
        <div><strong>WA:</strong> <a href="https://wa.me/6283143490913" class="underline">+62 831-4349-0913</a></div>
      </div>
    </section>

    <!-- Skills -->
    <section class="card" data-aos="fade-up">
      <h3 class="text-base font-bold text-cyan-300 mb-2">Skills</h3>
      <ul class="space-y-1 text-xs">
        <li>Web App Pentesting ⭐⭐⭐⭐⭐</li>
        <li>API Security ⭐⭐⭐⭐☆</li>
        <li>Network Hardening ⭐⭐⭐⭐☆</li>
        <li>Reverse Engineering ⭐⭐⭐☆</li>
        <li>OSINT & Threat Intel ⭐⭐⭐⭐⭐</li>
      </ul>
    </section>

    <!-- Projects -->
    <section class="card" data-aos="fade-up">
      <h3 class="text-base font-bold text-cyan-300 mb-2">Projects</h3>
      <ul class="space-y-1 text-xs">
        <li>Enterprise Audit ⭐⭐⭐⭐⭐</li>
        <li>Cloud Infra Review ⭐⭐⭐⭐☆</li>
        <li>Bug Bounty Findings ⭐⭐⭐⭐⭐</li>
        <li>API Security Hardening ⭐⭐⭐⭐☆</li>
      </ul>
    </section>

    <!-- Contact -->
    <section class="card" data-aos="fade-up">
      <h3 class="text-base font-bold text-cyan-300 mb-2">Contact</h3>
      <form class="space-y-2">
        <textarea rows="3" placeholder="Your message..."
          class="w-full text-xs p-2 rounded bg-black text-white border border-cyan-400"></textarea>
        <button class="w-full bg-cyan-500 text-black py-1 rounded font-bold text-xs hover:bg-cyan-400">Send Message</button>
      </form>
    </section>

    <!-- Footer -->
    <footer class="text-center text-[10px] text-slate-500" data-aos="fade-up">
      <div>Website ini dibuat oleh <strong>Kenzo</strong></div>
      <div>© 2025 Kenzo. Semua hak cipta dilindungi.</div>
    </footer>
  </main>

  <script>AOS.init();</script>
</body>
</html>
