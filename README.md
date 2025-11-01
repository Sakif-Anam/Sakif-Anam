<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sakif Anam | Animated GitHub Profile</title>
  <style>
    *{box-sizing:border-box;margin:0;padding:0}
    body{
      font-family:Inter,ui-sans-serif,system-ui,"Segoe UI",Roboto,Arial;
      background:radial-gradient(circle at top left,#031426 0%,#001020 60%,#000814 100%);
      color:#c8e9ff;display:flex;align-items:center;justify-content:center;
      min-height:100vh;padding:20px;
    }
    .card{
      background:rgba(0,40,60,0.5);
      border:1px solid rgba(0,200,255,0.2);
      border-radius:20px;
      box-shadow:0 0 30px rgba(0,255,255,0.1);
      display:flex;flex-direction:column;align-items:center;gap:20px;
      padding:30px;max-width:900px;width:100%;position:relative;
    }
    .avatar img{
      width:160px;height:160px;border-radius:50%;
      border:3px solid rgba(0,255,255,0.4);
      box-shadow:0 0 20px rgba(0,255,255,0.3);
    }
    .name{font-size:28px;font-weight:700;color:#8be9ff;}
    .handle{font-size:14px;color:#6fc7ff;}
    .bio{font-size:14px;color:#a0d8ff;text-align:center;max-width:500px;}

    /* looping languages animation */
    .languages{height:40px;overflow:hidden;position:relative;}
    .languages span{
      position:absolute;width:100%;text-align:center;font-size:22px;font-weight:700;
      color:#00ffff;opacity:0;animation:fadeSlide 8s infinite;
    }
    .languages span:nth-child(1){animation-delay:0s;color:#00ffff;}
    .languages span:nth-child(2){animation-delay:2s;color:#22d3ee;}
    .languages span:nth-child(3){animation-delay:4s;color:#38bdf8;}
    .languages span:nth-child(4){animation-delay:6s;color:#7dd3fc;}

    @keyframes fadeSlide{
      0%{opacity:0;transform:translateY(10px)}
      10%,25%{opacity:1;transform:translateY(0)}
      30%,100%{opacity:0;transform:translateY(-10px)}
    }

    .buttons{display:flex;gap:10px;margin-top:10px;}
    .btn{
      text-decoration:none;padding:10px 18px;border-radius:12px;
      border:1px solid rgba(0,255,255,0.3);
      color:#8be9ff;font-weight:600;transition:all .3s;
      background:rgba(0,60,90,0.3);
    }
    .btn:hover{background:rgba(0,200,255,0.2);box-shadow:0 0 20px rgba(0,255,255,0.3);}

    .graph-section{display:flex;flex-wrap:wrap;justify-content:space-around;width:100%;gap:20px;margin-top:20px;}
    .chart{flex:1;min-width:300px;padding:20px;border-radius:14px;background:rgba(0,30,50,0.5);border:1px solid rgba(0,255,255,0.1);}
    .chart h3{text-align:center;color:#7dd3fc;margin-bottom:10px;font-size:18px;}
    .bar{height:12px;background:rgba(0,255,255,0.15);border-radius:10px;margin:8px 0;overflow:hidden;}
    .bar div{height:100%;background:linear-gradient(90deg,#06b6d4,#22d3ee,#67e8f9);border-radius:10px;animation:fill 2s ease-out forwards;}
    @keyframes fill{from{width:0;}to{width:80%;}}

    @media(max-width:700px){.avatar img{width:120px;height:120px}.name{font-size:22px}}
  </style>
</head>
<body>
  <div class="card">
    <div class="avatar"><img src="your-photo.jpg" alt="Sakif Anam"></div>
    <div class="name">Sakif Anam</div>
    <div class="handle">@sakifanam</div>
    <div class="bio">Full‑stack enthusiast • Competitive programmer • Passionate about clean and efficient code</div>

    <div class="languages">
      <span>HTML</span>
      <span>CSS</span>
      <span>C</span>
      <span>C++</span>
    </div>

    <div class="buttons">
      <a class="btn" href="https://codeforces.com/profile/sakifanam0" target="_blank">Codeforces ↗</a>
      <a class="btn" href="#projects">Projects</a>
    </div>

    <div class="graph-section">
      <div class="chart">
        <h3>Codeforces Solved Problems</h3>
        <div class="bar"><div style="width:60%"></div></div>
        <div class="bar"><div style="width:80%"></div></div>
        <div class="bar"><div style="width:50%"></div></div>
      </div>
      <div class="chart">
        <h3>Languages Used</h3>
        <div>HTML<div class="bar"><div style="width:70%"></div></div></div>
        <div>CSS<div class="bar"><div style="width:60%"></div></div></div>
        <div>C<div class="bar"><div style="width:75%"></div></div></div>
        <div>C++<div class="bar"><div style="width:90%"></div></div></div>
      </div>
    </div>
  </div>
</body>
</html>
