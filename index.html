<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ATS Resume Checker</title>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
body { font-family: 'Segoe UI', sans-serif; background: #07071a; color: #fff; min-height: 100vh; }

body::before {
  content: '';
  position: fixed; inset: 0; z-index: 0;
  background: radial-gradient(ellipse 80% 50% at 30% 30%, rgba(108,99,255,0.15) 0%, transparent 60%),
              radial-gradient(ellipse 60% 60% at 75% 75%, rgba(0,229,160,0.07) 0%, transparent 60%);
  animation: bgpulse 6s ease-in-out infinite alternate;
}
@keyframes bgpulse { from {opacity:0.6} to {opacity:1} }

.particles { position:fixed; inset:0; z-index:0; pointer-events:none; overflow:hidden; }
.p { position:absolute; border-radius:50%; opacity:0; animation: floatup linear infinite; }
@keyframes floatup {
  0%   { transform:translateY(100vh); opacity:0; }
  10%  { opacity:0.5; }
  90%  { opacity:0.2; }
  100% { transform:translateY(-50px); opacity:0; }
}

/* ── LOGIN ── */
#login-page {
  position: relative; z-index: 1;
  min-height: 100vh;
  display: flex; align-items: center; justify-content: center;
  padding: 20px;
}

.login-card {
  width: 440px; max-width: 100%;
  background: rgba(18,18,35,0.9);
  backdrop-filter: blur(20px);
  border: 1px solid rgba(108,99,255,0.35);
  border-top: 3px solid #6c63ff;
  border-radius: 20px;
  padding: 52px 46px 44px;
  text-align: center;
  box-shadow: 0 40px 100px rgba(0,0,0,0.7), 0 0 80px rgba(108,99,255,0.08);
  animation: rise 0.6s cubic-bezier(.16,1,.3,1) both;
}
@keyframes rise { from{opacity:0;transform:translateY(36px)} to{opacity:1;transform:none} }

.logo-icon {
  width: 68px; height: 68px; border-radius: 18px;
  background: linear-gradient(135deg, #6c63ff, #00e5a0);
  display: flex; align-items: center; justify-content: center;
  font-size: 2rem; margin: 0 auto 18px;
  box-shadow: 0 8px 30px rgba(108,99,255,0.45);
  animation: bounce 2.5s ease-in-out infinite;
}
@keyframes bounce { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-7px)} }

.brand { font-size: 2.1rem; font-weight: 900; letter-spacing: 4px; color: #fff; margin-bottom: 5px; }
.brand span { color: #6c63ff; }
.tagline { font-size: 0.72rem; letter-spacing: 3px; text-transform: uppercase; color: #5555aa; margin-bottom: 38px; }

.field { margin-bottom: 18px; text-align: left; }
.field label { display:block; font-size:0.68rem; font-weight:700; letter-spacing:2px; text-transform:uppercase; color:#7777bb; margin-bottom:7px; }
.field input {
  width: 100%;
  background: rgba(10,10,28,0.8);
  border: 1.5px solid #2a2a50;
  border-radius: 10px;
  color: #ffffff;
  padding: 13px 16px;
  font-size: 0.95rem;
  outline: none;
  transition: border-color 0.25s, box-shadow 0.25s;
  font-family: inherit;
}
.field input:focus { border-color: #6c63ff; box-shadow: 0 0 0 4px rgba(108,99,255,0.18); }
.field input::placeholder { color: #333360; }

.login-btn {
  display: block;
  width: 100%;
  margin-top: 10px;
  padding: 15px 20px;
  background: #6c63ff;
  color: #ffffff;
  border: none;
  border-radius: 10px;
  font-size: 1rem;
  font-weight: 800;
  letter-spacing: 2px;
  cursor: pointer;
  box-shadow: 0 5px 25px rgba(108,99,255,0.5);
  transition: background 0.2s, transform 0.15s, box-shadow 0.2s;
  font-family: inherit;
}
.login-btn:hover { background: #8880ff; transform: translateY(-2px); box-shadow: 0 10px 35px rgba(108,99,255,0.6); }
.login-btn:active { transform: scale(0.97); }

.err-msg { color: #ff4d6d; font-size: 0.82rem; margin-top: 12px; min-height: 18px; }

.hint { margin-top: 20px; padding: 11px 16px; background: rgba(108,99,255,0.09); border: 1px solid rgba(108,99,255,0.2); border-radius: 8px; font-size: 0.76rem; color: #5555aa; }
.hint strong { color: #a89cff; }

/* ── APP ── */
#app { display: none; position: relative; z-index: 1; }

.navbar {
  display: flex; align-items: center; justify-content: space-between;
  padding: 0 36px; height: 62px;
  background: rgba(14,14,28,0.92); backdrop-filter: blur(16px);
  border-bottom: 1px solid rgba(108,99,255,0.2);
  position: sticky; top: 0; z-index: 99;
}
.nav-brand { font-size: 1.2rem; font-weight: 900; letter-spacing: 3px; }
.nav-brand span { color: #6c63ff; }
.nav-right { display: flex; align-items: center; gap: 14px; }
.nav-user { font-size: 0.78rem; color: #6666aa; }
.logout-btn {
  background: transparent; border: 1.5px solid #2a2a50;
  border-radius: 7px; color: #7777aa; padding: 6px 16px;
  font-size: 0.75rem; font-weight: 700; cursor: pointer;
  transition: all 0.2s; font-family: inherit;
}
.logout-btn:hover { border-color: #ff4d6d; color: #ff4d6d; }

.wrap { max-width: 900px; margin: 0 auto; padding: 48px 28px; text-align: center; }

.pg-title { font-size: 2.6rem; font-weight: 900; letter-spacing: 2px; margin-bottom: 8px; }
.pg-title span { color: #6c63ff; }
.pg-sub { font-size: 0.8rem; color: #5555aa; letter-spacing: 1px; margin-bottom: 40px; }

.upload-row {
  display: flex; align-items: center; justify-content: center; gap: 14px;
  flex-wrap: wrap; padding: 18px 24px; margin-bottom: 22px;
  background: rgba(18,18,35,0.7); border: 1.5px dashed rgba(108,99,255,0.35);
  border-radius: 12px; transition: border-color 0.3s, background 0.3s;
}
.upload-row:hover { border-color: #6c63ff; background: rgba(108,99,255,0.07); }
.upload-lbl { font-size: 0.78rem; font-weight: 700; letter-spacing: 1px; text-transform: uppercase; color: #7777aa; }
.file-wrap { position: relative; display: inline-block; }
.file-wrap input[type=file] { position: absolute; inset: 0; opacity: 0; cursor: pointer; width: 100%; height: 100%; }
.file-btn-ui {
  background: rgba(108,99,255,0.18); border: 1.5px solid rgba(108,99,255,0.4);
  border-radius: 8px; color: #a89cff; padding: 9px 22px;
  font-size: 0.84rem; font-weight: 700; cursor: pointer; transition: all 0.2s;
}
.file-btn-ui:hover { background: rgba(108,99,255,0.3); }
#fname { font-size: 0.8rem; color: #00e5a0; font-family: monospace; }

.ta-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 18px; margin-bottom: 22px; }
@media(max-width:620px){ .ta-grid { grid-template-columns: 1fr; } }

.ta-box {
  background: rgba(18,18,35,0.75); border: 1.5px solid #1e1e3a;
  border-radius: 12px; padding: 18px; text-align: left;
  transition: border-color 0.25s, transform 0.2s;
}
.ta-box:focus-within { border-color: #6c63ff; transform: translateY(-2px); }
.ta-box label { display: block; font-size: 0.68rem; font-weight: 700; letter-spacing: 2px; text-transform: uppercase; color: #7777aa; margin-bottom: 10px; }
.ta-box textarea {
  width: 100%; height: 220px;
  background: rgba(8,8,22,0.7); border: 1px solid #1e1e3a;
  border-radius: 8px; color: #eeeef4; padding: 14px;
  font-size: 0.86rem; resize: vertical; outline: none;
  line-height: 1.65; font-family: inherit;
  transition: border-color 0.2s;
}
.ta-box textarea:focus { border-color: #6c63ff; }
.ta-box textarea::placeholder { color: #252545; }

.check-btn {
  display: block; width: 100%; max-width: 480px; margin: 0 auto 36px;
  padding: 17px 40px;
  background: linear-gradient(135deg, #6c63ff 0%, #00e5a0 100%);
  color: #fff; border: none; border-radius: 12px;
  font-size: 1.08rem; font-weight: 800; letter-spacing: 1px;
  cursor: pointer;
  box-shadow: 0 6px 28px rgba(108,99,255,0.42);
  transition: transform 0.2s, box-shadow 0.2s, opacity 0.2s;
  font-family: inherit; position: relative; overflow: hidden;
}
.check-btn::before {
  content: ''; position: absolute; top: -50%; left: -70%; width: 40%; height: 200%;
  background: rgba(255,255,255,0.18); transform: skewX(-20deg);
  transition: left 0.5s;
}
.check-btn:hover { transform: translateY(-3px); box-shadow: 0 14px 40px rgba(108,99,255,0.52); }
.check-btn:hover::before { left: 130%; }
.check-btn:active { transform: scale(0.98); opacity: 0.9; }

/* Result */
.result { display: none; background: rgba(18,18,35,0.88); backdrop-filter: blur(10px); border: 1px solid rgba(108,99,255,0.3); border-left: 4px solid #6c63ff; border-radius: 16px; padding: 38px; margin-bottom: 16px; }

.score-num { font-size: 7rem; font-weight: 900; line-height: 1; margin-bottom: 6px; animation: popScore 0.8s cubic-bezier(.16,1,.3,1) both; }
@keyframes popScore { from{opacity:0;transform:scale(0.4)} to{opacity:1;transform:scale(1)} }
.verdict { font-size: 1.2rem; font-weight: 800; margin-bottom: 4px; }
.score-sub { font-size: 0.7rem; letter-spacing: 2px; text-transform: uppercase; color: #5555aa; margin-bottom: 26px; }

.bar-bg { width:100%; max-width:480px; background:rgba(10,10,25,0.8); height:10px; border-radius:5px; overflow:hidden; margin:0 auto 34px; }
.bar-fg { height:100%; border-radius:5px; width:0%; transition:width 1.4s cubic-bezier(.4,0,.2,1); }

.cols { display:grid; grid-template-columns:1fr 1fr; gap:18px; margin-bottom:22px; text-align:left; }
@media(max-width:540px){ .cols { grid-template-columns:1fr; } }
.col-box { background:rgba(8,8,22,0.6); border:1px solid #1a1a30; border-radius:12px; padding:18px; }
.col-box h4 { font-size:0.7rem; font-weight:800; letter-spacing:2px; text-transform:uppercase; margin-bottom:13px; }
.green { color:#00e5a0; } .red { color:#ff4d6d; } .gold { color:#ffb347; }

.tags { display:flex; flex-wrap:wrap; gap:7px; }
.tag { font-size:0.73rem; padding:4px 11px; border-radius:20px; font-family:monospace; animation:popin 0.3s ease both; cursor:default; transition:transform 0.2s; }
.tag:hover { transform:scale(1.1); }
@keyframes popin { from{opacity:0;transform:scale(0.6)} to{opacity:1;transform:scale(1)} }
.tg { background:rgba(0,229,160,0.1); color:#00e5a0; border:1px solid rgba(0,229,160,0.28); }
.tr { background:rgba(255,77,109,0.1); color:#ff4d6d; border:1px solid rgba(255,77,109,0.28); }

.tips-box { background:rgba(255,179,71,0.05); border:1px solid rgba(255,179,71,0.2); border-radius:12px; padding:22px; text-align:left; }
.tips-box h4 { margin-bottom:14px; }
.tips-list { list-style:none; display:flex; flex-direction:column; gap:11px; }
.tips-list li { font-size:0.87rem; line-height:1.65; color:#ccccdd; padding-left:22px; position:relative; animation:fadeup 0.4s ease both; }
.tips-list li::before { content:'→'; position:absolute; left:0; color:#ffb347; font-weight:bold; }
@keyframes fadeup { from{opacity:0;transform:translateY(10px)} to{opacity:1;transform:none} }

/* History */
.hist-title { font-size:0.76rem; font-weight:700; letter-spacing:2px; text-transform:uppercase; color:#5555aa; margin:44px 0 18px; padding-top:28px; border-top:1px solid rgba(108,99,255,0.15); }
.hist-grid { display:grid; grid-template-columns:repeat(auto-fill,minmax(170px,1fr)); gap:13px; justify-items:center; }
.hcard { width:100%; background:rgba(18,18,35,0.75); border:1px solid #1e1e3a; border-radius:12px; padding:20px; position:relative; text-align:center; transition:border-color 0.2s,transform 0.2s,box-shadow 0.2s; animation:popin 0.4s ease both; }
.hcard:hover { border-color:#6c63ff; transform:translateY(-4px); box-shadow:0 10px 28px rgba(108,99,255,0.2); }
.hcard-score { font-size:2.4rem; font-weight:900; line-height:1; margin-bottom:5px; }
.hcard-job { font-size:0.78rem; font-weight:600; color:#9999bb; margin-bottom:4px; overflow:hidden; text-overflow:ellipsis; white-space:nowrap; }
.hcard-date { font-size:0.67rem; color:#444466; font-family:monospace; }
.hcard-del { position:absolute; top:9px; right:9px; background:none; border:none; color:#1e1e3a; cursor:pointer; font-size:0.9rem; transition:color 0.2s; }
.hcard-del:hover { color:#ff4d6d; }
</style>
</head>
<body>

<div class="particles">
  <div class="p" style="left:8%;  width:3px;height:3px;background:#6c63ff;animation-duration:13s;animation-delay:0s;"></div>
  <div class="p" style="left:22%; width:2px;height:2px;background:#00e5a0;animation-duration:16s;animation-delay:2s;"></div>
  <div class="p" style="left:38%; width:4px;height:4px;background:#a89cff;animation-duration:11s;animation-delay:4s;"></div>
  <div class="p" style="left:54%; width:2px;height:2px;background:#6c63ff;animation-duration:14s;animation-delay:1s;"></div>
  <div class="p" style="left:68%; width:3px;height:3px;background:#00e5a0;animation-duration:10s;animation-delay:3s;"></div>
  <div class="p" style="left:82%; width:2px;height:2px;background:#a89cff;animation-duration:15s;animation-delay:5s;"></div>
</div>

<!-- LOGIN -->
<div id="login-page">
  <div class="login-card">
    <div class="logo-icon">📄</div>
    <div class="brand">ATS<span>.</span>CHECK</div>
    <div class="tagline">Resume Score Checker</div>

    <div class="field">
      <label>Username</label>
      <input type="text" id="u" placeholder="Enter username" autocomplete="off" />
    </div>
    <div class="field">
      <label>Password</label>
      <input type="password" id="p" placeholder="Enter password" />
    </div>

    <button class="login-btn" id="loginBtn">SIGN IN →</button>
    <div class="err-msg" id="err"></div>
    <div class="hint">Demo → Username: <strong>admin</strong> &nbsp;/&nbsp; Password: <strong>1234</strong></div>
  </div>
</div>

<!-- APP -->
<div id="app">
  <div class="navbar">
    <div class="nav-brand">ATS<span>.</span>CHECK</div>
    <div class="nav-right">
      <span class="nav-user" id="navUser"></span>
      <button class="logout-btn" id="logoutBtn">Logout</button>
    </div>
  </div>

  <div class="wrap">
    <div class="pg-title">Resume <span>ATS</span> Checker</div>
    <div class="pg-sub">Upload or paste your resume · Add job description · Get your score instantly</div>

    <div class="upload-row">
      <span class="upload-lbl">📄 Upload Resume (.txt)</span>
      <div class="file-wrap">
        <div class="file-btn-ui">Choose File</div>
        <input type="file" id="rfile" accept=".txt" />
      </div>
      <span id="fname">No file chosen</span>
    </div>

    <div class="ta-grid">
      <div class="ta-box">
        <label>📝 Your Resume / CV</label>
        <textarea id="rtxt" placeholder="Paste your resume here...&#10;&#10;Include skills, experience, education and achievements."></textarea>
      </div>
      <div class="ta-box">
        <label>💼 Job Description</label>
        <textarea id="jdtxt" placeholder="Paste the job description here...&#10;&#10;Include required skills and qualifications."></textarea>
      </div>
    </div>

    <button class="check-btn" id="checkBtn">⚡ Check ATS Score Now</button>

    <div class="result" id="result">
      <div class="score-num" id="scoreNum">0</div>
      <div class="verdict" id="verdict"></div>
      <div class="score-sub">ATS Match Score out of 100</div>
      <div class="bar-bg"><div class="bar-fg" id="barFg"></div></div>
      <div class="cols">
        <div class="col-box">
          <h4 class="green">✅ Matched Keywords</h4>
          <div class="tags" id="matched"></div>
        </div>
        <div class="col-box">
          <h4 class="red">❌ Missing Keywords</h4>
          <div class="tags" id="missing"></div>
        </div>
      </div>
      <div class="tips-box">
        <h4 class="gold">💡 Tips to Improve</h4>
        <ul class="tips-list" id="tips"></ul>
      </div>
    </div>

    <div id="histSec" style="display:none">
      <div class="hist-title">📋 Recent Scores</div>
      <div class="hist-grid" id="histGrid"></div>
    </div>
  </div>
</div>

<script>
// ── users ──
var USERS = { admin: '1234', krishna: 'pass123' };
var CU = null; // current user

// ── login ──
function tryLogin() {
  var u = document.getElementById('u').value.trim();
  var p = document.getElementById('p').value.trim();
  var e = document.getElementById('err');
  if (!u || !p) { e.textContent = '⚠️ Please enter username and password'; return; }
  if (USERS[u] && USERS[u] === p) {
    CU = u;
    document.getElementById('login-page').style.display = 'none';
    document.getElementById('app').style.display = 'block';
    document.getElementById('navUser').textContent = '👤 ' + u;
    loadHist();
  } else {
    e.textContent = '❌ Wrong details. Use: admin / 1234';
  }
}

document.getElementById('loginBtn').onclick = tryLogin;
document.getElementById('p').onkeydown = function(e){ if(e.key==='Enter') tryLogin(); };
document.getElementById('u').onkeydown = function(e){ if(e.key==='Enter') tryLogin(); };

// ── logout ──
document.getElementById('logoutBtn').onclick = function() {
  CU = null;
  document.getElementById('app').style.display = 'none';
  document.getElementById('login-page').style.display = 'flex';
  document.getElementById('u').value = '';
  document.getElementById('p').value = '';
  document.getElementById('err').textContent = '';
  document.getElementById('result').style.display = 'none';
};

// ── file upload ──
document.getElementById('rfile').onchange = function() {
  var file = this.files[0];
  if (!file) return;
  document.getElementById('fname').textContent = '✓ ' + file.name;
  var r = new FileReader();
  r.onload = function(e) { document.getElementById('rtxt').value = e.target.result; };
  r.readAsText(file);
};

// ── ATS logic ──
var STOP = new Set('a an the and or but in on at to for of with by from is are was were be been have has had do does did will would could should may might this that these those we our you your they their it its as not no up out into about such than too very just more most also both each can use using used over all any i me my'.split(' '));

function tokens(t) {
  return t.toLowerCase().replace(/[^a-z0-9+#.\s]/g,' ').split(/\s+/).filter(function(w){ return w.length>2 && !STOP.has(w); });
}

var PH = 'machine learning,deep learning,data analysis,data science,project management,agile methodology,software development,full stack,front end,back end,devops,ci/cd,cloud computing,restful api,microservices,version control,digital marketing,seo,content marketing,social media,financial analysis,risk management,customer service,problem solving,critical thinking,time management,leadership,communication skills,team player,attention to detail,react.js,node.js,next.js,vue.js,angular,express.js,aws,google cloud,microsoft azure,docker,kubernetes,mongodb,postgresql,mysql,redis,python,javascript,typescript,java,git,github,figma,bachelor,master,phd,certified'.split(',');

function phrases(t) {
  var low = t.toLowerCase();
  return PH.filter(function(p){ return low.indexOf(p)>-1; });
}

function animNum(el, n, color) {
  var s=0, dur=1100, t0=null;
  (function step(ts){
    if(!t0) t0=ts;
    var prog = Math.min((ts-t0)/dur,1);
    var ease = 1-Math.pow(1-prog,3);
    el.textContent = Math.round(ease*n);
    if(prog<1) requestAnimationFrame(step);
    else { el.textContent=n; el.style.color=color; }
  })(performance.now());
}

document.getElementById('checkBtn').onclick = function() {
  var res = document.getElementById('rtxt').value.trim();
  var jd  = document.getElementById('jdtxt').value.trim();
  if (!res || !jd) { alert('Please fill in BOTH the Resume and Job Description!'); return; }

  var jt=tokens(jd), rt=tokens(res), rs=new Set(rt);
  var jp=phrases(jd), rp=phrases(res);
  var freq={}; jt.forEach(function(w){ freq[w]=(freq[w]||0)+1; });
  var kws=Object.keys(freq);
  var km=kws.filter(function(w){ return rs.has(w); });
  var miss=kws.filter(function(w){ return !rs.has(w); });
  var pm=jp.filter(function(p){ return rp.indexOf(p)>-1; });
  var pmiss=jp.filter(function(p){ return rp.indexOf(p)===-1; });

  var score = Math.min(100,Math.max(0,Math.round(
    (kws.length>0?km.length/kws.length:0)*60 +
    (jp.length>0?pm.length/jp.length:0)*40
  )));

  var sm = pm.concat(km).filter(function(v,i,a){ return a.indexOf(v)===i; }).slice(0,14);
  var sx = pmiss.concat(miss).filter(function(v,i,a){ return a.indexOf(v)===i; }).slice(0,12);

  var tips=[];
  if(pmiss.length>0) tips.push('Add these key phrases: "'+pmiss.slice(0,3).join('", "')+'"');
  if(km.length/Math.max(kws.length,1)<0.6) tips.push('Use more keywords from the job description — ATS scans for exact matches.');
  if(res.toLowerCase().indexOf('increased')===-1 && res.toLowerCase().indexOf('%')===-1 && res.toLowerCase().indexOf('improved')===-1) tips.push('Quantify achievements e.g. Increased efficiency by 30 percent to boost your score.');
  if(res.split(/\s+/).length<250) tips.push('Resume is too short. Aim for 400–700 words for best results.');
  if(score>=70) tips.push('Great match! Write a tailored cover letter to stand out.');
  if(tips.length<2) tips.push('Use standard headings: Skills, Experience, Education.');

  var col=score>=80?'#00e5a0':score>=60?'#a89cff':score>=40?'#ffb347':'#ff4d6d';
  var verd=score>=80?'🟢 Excellent Match':score>=60?'🟡 Good Match':score>=40?'🟠 Needs Improvement':'🔴 Poor Match';

  var rd=document.getElementById('result');
  rd.style.display='block';

  var sn=document.getElementById('scoreNum');
  sn.style.color=col;
  animNum(sn,score,col);

  document.getElementById('verdict').textContent=verd;
  document.getElementById('verdict').style.color=col;
  document.getElementById('barFg').style.background='linear-gradient(90deg,'+col+','+col+'88)';
  setTimeout(function(){ document.getElementById('barFg').style.width=score+'%'; },80);

  document.getElementById('matched').innerHTML = sm.length
    ? sm.map(function(w,i){ return '<span class="tag tg" style="animation-delay:'+(i*.05)+'s">'+w+'</span>'; }).join('')
    : '<span style="color:#333355;font-size:.8rem">None found</span>';

  document.getElementById('missing').innerHTML = sx.length
    ? sx.map(function(w,i){ return '<span class="tag tr" style="animation-delay:'+(i*.05)+'s">'+w+'</span>'; }).join('')
    : '<span style="color:#00e5a0;font-size:.82rem">🎉 None missing!</span>';

  document.getElementById('tips').innerHTML = tips.map(function(t,i){
    return '<li style="animation-delay:'+(i*.1)+'s">'+t+'</li>';
  }).join('');

  rd.scrollIntoView({behavior:'smooth',block:'start'});
  saveHist(score, jd.substring(0,44)+'…', col);
};

// ── history ──
function getHist(){ try{ return JSON.parse(localStorage.getItem('h_'+CU)||'[]'); }catch(e){ return []; } }

function saveHist(score,job,col){
  var h=getHist();
  h.unshift({id:Date.now(),score:score,job:job,col:col,
    date:new Date().toLocaleDateString('en-IN',{day:'2-digit',month:'short',year:'numeric'})});
  localStorage.setItem('h_'+CU,JSON.stringify(h.slice(0,20)));
  loadHist();
}

function delHist(id){
  localStorage.setItem('h_'+CU,JSON.stringify(getHist().filter(function(x){ return x.id!==id; })));
  loadHist();
}

function loadHist(){
  var h=getHist();
  var s=document.getElementById('histSec');
  if(!h.length){ s.style.display='none'; return; }
  s.style.display='block';
  document.getElementById('histGrid').innerHTML=h.map(function(x){
    return '<div class="hcard"><button class="hcard-del" onclick="delHist('+x.id+')">✕</button>'
      +'<div class="hcard-score" style="color:'+x.col+'">'+x.score+'</div>'
      +'<div class="hcard-job">'+x.job+'</div>'
      +'<div class="hcard-date">'+x.date+'</div></div>';
  }).join('');
}
</script>
</body>
</html>
