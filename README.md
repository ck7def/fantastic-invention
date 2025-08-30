<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width,initial-scale=1.0" />
<title>Cooper Kalisek — Portfolio</title>
<style>
  /* ===== Base ===== */
  :root{
    --bg:#0e0f12; --panel:#171921; --panel-2:#1f2230; --text:#e8f0ff;
    --muted:#9fb0c9; --accent:#00f5ff; --accent-2:#7cff6b; --warn:#ffda4a; --danger:#ff5c7a;
    --ring:0 0 0 2px rgba(0,245,255,.3), 0 0 24px rgba(0,245,255,.18);
  }
  *{box-sizing:border-box} html,body{margin:0; padding:0; background:var(--bg); color:var(--text); font:16px/1.6 system-ui,-apple-system,Segoe UI,Roboto,Inter,Arial}
  a{color:var(--accent); text-decoration:none}
  a:hover{opacity:.85}
  h1,h2,h3{letter-spacing:.3px; margin:.2em 0 .5em}
  section{padding:56px 20px}
  .container{max-width:1100px; margin:0 auto}
  .muted{color:var(--muted)}
  .pill{display:inline-flex; align-items:center; gap:.5rem; border:1px solid #2a2e40; padding:.35rem .6rem; border-radius:999px; background:linear-gradient(180deg,#141726,#0f121c)}
  .grid{display:grid; gap:18px}
  @media(min-width:800px){ .grid-3{grid-template-columns:repeat(3,1fr)} .grid-4{grid-template-columns:repeat(4,1fr)} }
  .card{background:var(--panel); border:1px solid #202535; border-radius:12px; padding:18px; transition:transform .15s ease, box-shadow .15s ease, border-color .15s ease}
  .card:hover{transform:translateY(-2px); border-color:#2c3450; box-shadow:var(--ring)}
  .btn{background:var(--accent); color:#021014; border:none; border-radius:10px; padding:10px 14px; font-weight:700; cursor:pointer}
  .btn:hover{filter:brightness(1.05)}
  .btn.secondary{background:#2c3450; color:var(--text); border:1px solid #39425e}
  input,textarea{width:100%; background:#0f1220; color:var(--text); border:1px solid #2a2e40; border-radius:10px; padding:10px 12px}
  textarea{min-height:120px; resize:vertical}
  .row{display:flex; gap:12px; flex-wrap:wrap}
  .kicker{font-size:.9rem; text-transform:uppercase; letter-spacing:.18em; color:var(--muted)}
  .tag{font-size:.8rem; opacity:.9}
  .hr{height:1px; background:#23283a; margin:18px 0}
  /* ===== Header / Nav ===== */
  header{padding:36px 20px 16px; position:sticky; top:0; z-index:40; background:linear-gradient(180deg,#0e0f12 0%, rgba(14,15,18,.92) 70%, rgba(14,15,18,.6) 100%); backdrop-filter:saturate(120%) blur(6px); border-bottom:1px solid #161927}
  nav{display:flex; align-items:center; justify-content:space-between; gap:16px; max-width:1100px; margin:0 auto}
  nav .links{display:flex; gap:14px; flex-wrap:wrap}
  nav a{padding:8px 10px}
  /* ===== Chat ===== */
  #chat-wrap{display:grid; gap:16px}
  @media(min-width:900px){ #chat-wrap{grid-template-columns:2fr 1fr} }
  #chat-container{background:var(--panel); border:1px solid #202535; border-radius:12px; padding:14px; max-height:420px; overflow:auto}
  .msg{max-width:78%; margin:6px 0; padding:8px 10px; border-radius:10px; display:inline-block; word-wrap:break-word; box-shadow:0 0 0 1px rgba(255,255,255,.06) inset}
  .msg.me{align-self:flex-end}
  .stamp{font-size:.72rem; opacity:.7; margin-left:6px}
  .sys{opacity:.8; font-style:italic}
  #chat-input{display:flex; gap:8px}
  .monitor{background:var(--panel); border:1px solid #202535; border-radius:12px; padding:14px}
  .led{width:10px; height:10px; border-radius:50%; display:inline-block; margin-right:8px; background:#444}
  .led.on{background:var(--accent-2); box-shadow:0 0 12px rgba(124,255,107,.6)}
  .trend{font-size:.92rem}
  .trend li{margin:4px 0}
  /* ===== Dev Area ===== */
  #dev-area{display:none}
  .kbd{font-family:ui-monospace, SFMono-Regular, Menlo, Consolas, monospace; background:#0c0f18; border:1px solid #2b3044; padding:2px 6px; border-radius:6px}
  .code{white-space:pre-wrap; background:#0c0f18; border:1px solid #283149; padding:10px; border-radius:8px; font-family:ui-monospace,Menlo,Consolas,monospace}
  .ok{color:var(--accent-2)} .bad{color:var(--danger)}
</style>
</head>
<body>

<header>
  <nav>
    <div class="row" style="align-items:center">
      <span class="pill"><strong>Cooper Kalisek</strong><span class="tag">/ portfolio</span></span>
    </div>
    <div class="links">
      <a href="#about">About</a>
      <a href="#resume">Resume</a>
      <a href="#projects">Projects</a>
      <a href="#partners">Partners</a>
      <a href="#swag">Swag</a>
      <a href="#models">Models</a>
      <a href="#chat">Chat</a>
      <a href="#outreach">Outreach</a>
    </div>
  </nav>
</header>

<!-- ===== About ===== -->
<section id="about">
  <div class="container">
    <div class="kicker">About</div>
    <h2>Building useful systems with taste</h2>
    <p class="muted">Full-stack + AI + security-minded. This page mixes portfolio, live chat, and a private dev space with client-side encryption.</p>
  </div>
</section>

<!-- ===== Resume ===== -->
<section id="resume">
  <div class="container">
    <div class="kicker">Resume</div>
    <h2>Experience Snapshot</h2>
    <div class="grid grid-3">
      <div class="card"><h3>Engineering</h3><div class="hr"></div><p>Web, APIs, data pipelines, infra. Ship fast, de-risk faster.</p></div>
      <div class="card"><h3>AI & Tools</h3><div class="hr"></div><p>NLP, retrieval, agents, evals, and product integrations.</p></div>
      <div class="card"><h3>Security</h3><div class="hr"></div><p>Threat modeling, authN/Z, privacy-by-design, client-side crypto.</p></div>
    </div>
    <p style="margin-top:14px"><a class="pill" href="#" download="Cooper_Kalisek_Resume.pdf">Download PDF Resume</a></p>
  </div>
</section>

<!-- ===== Projects ===== -->
<section id="projects">
  <div class="container">
    <div class="kicker">Projects</div>
    <h2>Selected Work</h2>
    <div class="grid grid-3">
      <div class="card"><h3>AI Web Integration</h3><div class="hr"></div><p>Composable UI + inference hooks. Latency-aware UX.</p></div>
      <div class="card"><h3>Secure Messaging</h3><div class="hr"></div><p>All in browser: AES-GCM, passphrase-derived keys.</p></div>
      <div class="card"><h3>Interactive Portfolio</h3><div class="hr"></div><p>Single-file, dark lab vibe, real-time monitoring.</p></div>
    </div>
  </div>
</section>

<!-- ===== Partners & Watchers ===== -->
<section id="partners">
  <div class="container">
    <div class="kicker">Partners & Watchers</div>
    <h2>Signals & Collabs</h2>
    <div class="grid grid-4">
      <div class="card"><strong>Lab11</strong><div class="muted">research lab</div></div>
      <div class="card"><strong>Firebase</strong><div class="muted">auth + realtime</div></div>
      <div class="card"><strong>AllSaints</strong><div class="muted">brand</div></div>
      <div class="card"><strong>More</strong><div class="muted">+ add logos</div></div>
    </div>
  </div>
</section>

<!-- ===== Swag ===== -->
<section id="swag">
  <div class="container">
    <div class="kicker">Swag</div>
    <h2>Patches, Stickers, Kits</h2>
    <div class="grid grid-4">
      <div class="card">🔖 Neon Badge</div>
      <div class="card">🎛️ Control Panel Sticker</div>
      <div class="card">🧪 Lab Tag</div>
      <div class="card">👕 Mock Tee</div>
    </div>
  </div>
</section>

<!-- ===== Models / Tools ===== -->
<section id="models">
  <div class="container">
    <div class="kicker">Models & Tools</div>
    <h2>Showcase</h2>
    <div class="grid grid-3">
      <div class="card"><h3>NLP-Ops</h3><div class="hr"></div><p>Prompt router + guardrails.</p></div>
      <div class="card"><h3>Vision Lite</h3><div class="hr"></div><p>Fast local detection demo.</p></div>
      <div class="card"><h3>Eval Kit</h3><div class="hr"></div><p>Regression + data cards.</p></div>
    </div>
  </div>
</section>

<!-- ===== Chat, Trending, Monitoring ===== -->
<section id="chat">
  <div class="container">
    <div class="kicker">Chat</div>
    <h2>Public Chat + Trending</h2>

    <div id="chat-wrap">
      <!-- Chat Panel -->
      <div class="card">
        <div id="chat-container"></div>
        <div id="chat-input" style="margin-top:10px">
          <input id="chat-text" placeholder="Type a message and press Enter…" />
          <button class="btn" id="send">Send</button>
          <button class="btn secondary" id="unlock-btn" title="Unlock Dev Area">Unlock</button>
        </div>
        <div class="muted" style="margin-top:8px">
          Messages are color-coded by a hash of content for quick context scanning.
        </div>
      </div>

      <!-- Monitoring / Trending -->
      <aside class="monitor">
        <h3>Monitoring</h3>
        <p><span class="led" id="led"></span><strong id="health">Idle</strong> <span class="muted" id="lastStamp">—</span></p>
        <div class="hr"></div>
        <h3>Trending</h3>
        <ul id="trends" class="trend"></ul>
        <div class="hr"></div>
        <h3>Actions</h3>
        <div class="row">
          <button class="btn secondary" id="clear-chat">Clear</button>
          <button class="btn secondary" id="export-chat">Export</button>
        </div>
      </aside>
    </div>
  </div>
</section>

<!-- ===== Outreach ===== -->
<section id="outreach">
  <div class="container">
    <div class="kicker">Outreach</div>
    <h2>Let’s build something</h2>
    <div class="grid grid-3">
      <div class="card">
        <h3>Contact</h3><div class="hr"></div>
        <form id="contact-form" onsubmit="event.preventDefault(); alert('Thanks! (wire up later)'); this.reset();">
          <label>Name</label><input required />
          <label>Email</label><input type="email" required />
          <label>Message</label><textarea required></textarea>
          <div style="margin-top:10px"><button class="btn">Send</button></div>
        </form>
      </div>
      <div class="card">
        <h3>Signals</h3><div class="hr"></div>
        <p class="muted">Short note on collaboration areas, availability, and preferred contact windows.</p>
      </div>
      <div class="card">
        <h3>Swag Drop</h3><div class="hr"></div>
        <p>Collect a digital badge when we ship together.</p>
        <button class="btn secondary" onclick="alert('Badge minted (demo).')">Mint Badge</button>
      </div>
    </div>
  </div>
</section>

<!-- ===== Dev Area (Locked) ===== -->
<section id="dev">
  <div class="container">
    <div class="kicker">Dev</div>
    <h2>Private Dev Area</h2>
    <div id="dev-area" class="card">
      <p><strong>Status:</strong> <span id="dev-status" class="bad">Locked</span></p>
      <div class="hr"></div>
      <div class="row">
        <button class="btn" id="set-pass">Set/Change Dev Password</button>
        <button class="btn secondary" id="lock-dev">Lock</button>
      </div>
      <div class="hr"></div>
      <h3>Encrypted Messages (Client-side AES-GCM)</h3>
      <p class="muted">Use a passphrase to derive a key. Works fully in the browser.</p>
      <div class="row" style="align-items:flex-end">
        <div style="flex:2">
          <label>Passphrase</label>
          <input id="enc-pass" type="password" placeholder="Enter decryption passphrase"/>
        </div>
        <div><button class="btn secondary" id="enc-bind">Bind Key</button></div>
      </div>
      <div class="hr"></div>
      <div class="row">
        <div style="flex:1">
          <label>Plaintext</label>
          <textarea id="enc-plain" placeholder="Type secret…"></textarea>
          <div style="margin-top:8px"><button class="btn" id="enc-do">Encrypt & Save (local)</button></div>
        </div>
        <div style="flex:1">
          <label>Ciphertext (base64)</label>
          <textarea id="enc-cipher" readonly></textarea>
          <div class="row" style="margin-top:8px">
            <button class="btn secondary" id="dec-do">Decrypt Selected</button>
            <button class="btn secondary" id="wipe-secrets">Wipe Stored</button>
          </div>
        </div>
      </div>
      <div class="hr"></div>
      <h4>Stored Encrypted Messages</h4>
      <div id="enc-list" class="code">[]</div>
    </div>
  </div>
</section>

<script>
/* ========== Utilities ========== */
const $ = sel => document.querySelector(sel);
const $$ = sel => Array.from(document.querySelectorAll(sel));
const nowStamp = () => new Date().toLocaleTimeString();

/* ========== Chat Logic (color-coded by content hash) ========== */
const chatBox = $('#chat-container');
const input = $('#chat-text');
const sendBtn = $('#send');
const clearBtn = $('#clear-chat');
const exportBtn = $('#export-chat');

let CHAT = []; // {text, ts}
let trendMap = new Map();
let lastActivity = 0;

function hashHue(str){
  let h=0; for(let i=0;i<str.length;i++){ h = (h*31 + str.charCodeAt(i)) >>> 0; }
  return h % 360;
}
function addMsg(text, role='me'){
  if(!text) return;
  const ts = Date.now();
  CHAT.push({text, ts});
  // update trends (simple: top keywords excluding stopwords)
  const words = text.toLowerCase().match(/\b[a-z0-9]{3,}\b/g) || [];
  const stop = new Set(['the','and','for','that','with','this','have','you','are','but','not','just','your','from','into','then','they','them','our','out']);
  words.forEach(w=>{ if(!stop.has(w)) trendMap.set(w,(trendMap.get(w)||0)+1); });

  const hue = hashHue(text);
  const el = document.createElement('div');
  el.className = 'msg ' + (role==='me'?'me':'you');
  el.style.background = `hsl(${hue} 80% 60% / .2)`;
  el.style.border = `1px solid hsl(${hue} 60% 45% / .55)`;
  el.innerHTML = `${escapeHtml(text)} <span class="stamp">${nowStamp()}</span>`;
  chatBox.appendChild(el);
  chatBox.scrollTop = chatBox.scrollHeight;

  lastActivity = ts;
  refreshMonitor();
  renderTrends();
}
function escapeHtml(s){ return s.replace(/[&<>"]/g, c=>({ '&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;' }[c]) ); }

sendBtn.addEventListener('click', () => {
  const val = input.value.trim();
  if(!val) return;
  addMsg(val,'me');
  input.value = '';
  // demo echo “watcher”
  setTimeout(()=> addMsg('Watcher: ' + val.slice(0,80), 'you'), 350);
});
input.addEventListener('keydown', e => { if(e.key==='Enter'){ sendBtn.click(); } });

clearBtn.addEventListener('click', ()=>{
  CHAT = []; trendMap.clear(); chatBox.innerHTML=''; renderTrends(); refreshMonitor(true);
});
exportBtn.addEventListener('click', ()=>{
  const blob = new Blob([JSON.stringify(CHAT,null,2)], {type:'application/json'});
  const a = document.createElement('a');
  a.href = URL.createObjectURL(blob);
  a.download = 'chat-export.json';
  a.click();
});

/* ========== Monitoring & Trending ========== */
const led = $('#led'); const health = $('#health'); const lastStamp = $('#lastStamp'); const trends = $('#trends');
function refreshMonitor(reset=false){
  if(reset){ health.textContent='Idle'; led.classList.remove('on'); lastStamp.textContent='—'; return; }
  const delta = Date.now() - lastActivity;
  if(delta < 15000){ health.textContent='Active'; led.classList.add('on'); }
  else { health.textContent='Idle'; led.classList.remove('on'); }
  lastStamp.textContent = 'Last: ' + new Date(lastActivity||Date.now()).toLocaleTimeString();
}
function renderTrends(){
  const arr = Array.from(trendMap.entries()).sort((a,b)=>b[1]-a[1]).slice(0,8);
  trends.innerHTML = arr.map(([w,c])=>`<li><span class="pill">${w}</span> × ${c}</li>`).join('') || '<li class="muted">No trends yet.</li>';
}
setInterval(refreshMonitor, 5000);

/* ========== Simple Password Lock for Dev Area ========== */
const unlockBtn = $('#unlock-btn');
const devArea = $('#dev-area');
const devStatus = $('#dev-status');
const setPassBtn = $('#set-pass');
const lockBtn = $('#lock-dev');
const PASS_KEY = 'dev-pass-v1';

function isUnlocked(){ return devArea.style.display === 'block'; }
function lockDev(){ devArea.style.display='none'; devStatus.textContent='Locked'; devStatus.classList.remove('ok'); devStatus.classList.add('bad'); }
function unlockDevFlow(){
  const stored = localStorage.getItem(PASS_KEY) || 'letmein'; // default
  const pass = prompt('Enter dev password:');
  if(pass === stored){ devArea.style.display='block'; devStatus.textContent='Unlocked'; devStatus.classList.add('ok'); devStatus.classList.remove('bad'); }
  else alert('Incorrect password.');
}
unlockBtn.addEventListener('click', unlockDevFlow);
lockBtn.addEventListener('click', lockDev);
setPassBtn.addEventListener('click', ()=>{
  const current = localStorage.getItem(PASS_KEY) || 'letmein';
  const old = prompt('Current password:');
  if(old !== current){ alert('Wrong current password.'); return; }
  const np = prompt('New password (min 4 chars):') || '';
  if(np.length < 4){ alert('Too short.'); return; }
  localStorage.setItem(PASS_KEY, np);
  alert('Password updated.');
});

/* ========== Client-side Encryption (AES-GCM via Web Crypto) ========== */
const encPass = $('#enc-pass'), bindBtn = $('#enc-bind'), encPlain = $('#enc-plain'),
      encCipher = $('#enc-cipher'), encDo = $('#enc-do'), decDo = $('#dec-do'),
      wipeBtn = $('#wipe-secrets'), encList = $('#enc-list');

const STORE_KEY = 'enc-messages-v1';
let cryptoKey = null;

async function deriveKey(passphrase){
  const enc = new TextEncoder();
  const salt = enc.encode('ck-salt-fixed-demo'); // replace w/ random & store if you want per-user salts
  const baseKey = await crypto.subtle.importKey('raw', enc.encode(passphrase), 'PBKDF2', false, ['deriveKey']);
  return crypto.subtle.deriveKey(
    {name:'PBKDF2', salt, iterations:100000, hash:'SHA-256'},
    baseKey,
    {name:'AES-GCM', length:256},
    false,
    ['encrypt','decrypt']
  );
}
function b64(buf){ return btoa(String.fromCharCode(...new Uint8Array(buf))); }
function fromB64(b){ return Uint8Array.from(atob(b), c=>c.charCodeAt(0)); }

async function encryptText(plain){
  if(!cryptoKey) throw new Error('Bind a key first.');
  const iv = crypto.getRandomValues(new Uint8Array(12));
  const ct = await crypto.subtle.encrypt({name:'AES-GCM', iv}, cryptoKey, new TextEncoder().encode(plain));
  return { iv: b64(iv), ct: b64(ct) };
}
async function decryptText(ivB64, ctB64){
  if(!cryptoKey) throw new Error('Bind a key first.');
  const iv = fromB64(ivB64);
  const pt = await crypto.subtle.decrypt({name:'AES-GCM', iv}, cryptoKey, fromB64(ctB64));
  return new TextDecoder().decode(pt);
}
function loadStore(){ try{ return JSON.parse(localStorage.getItem(STORE_KEY)||'[]'); }catch{return[]} }
function saveStore(arr){ localStorage.setItem(STORE_KEY, JSON.stringify(arr)); renderStore(); }
function renderStore(){
  const data = loadStore();
  encList.textContent = JSON.stringify(data, null, 2);
  if(data.length){ encCipher.value = data[data.length-1].ct; }
}
bindBtn.addEventListener('click', async ()=>{
  if(!encPass.value){ alert('Enter a passphrase.'); return; }
  cryptoKey = await deriveKey(encPass.value);
  alert('Key bound. You can encrypt/decrypt now.');
});
encDo.addEventListener('click', async ()=>{
  try{
    const msg = encPlain.value.trim(); if(!msg) return;
    const {iv, ct} = await encryptText(msg);
    const arr = loadStore(); arr.push({iv, ct, ts: Date.now()}); saveStore(arr);
    encPlain.value=''; encCipher.value=ct;
  }catch(e){ alert('Encrypt failed: '+e.message); }
});
decDo.addEventListener('click', async ()=>{
  try{
    const ct = encCipher.value.trim(); if(!ct){ alert('No ciphertext.'); return; }
    const arr = loadStore(); // try last item with matching ct
    const rec = arr.reverse().find(x=>x.ct===ct) || {iv: prompt('IV (base64)?'), ct};
    const plain = await decryptText(rec.iv, rec.ct);
    alert('Decrypted:\n\n' + plain);
  }catch(e){ alert('Decrypt failed: '+e.message); }
});
wipeBtn.addEventListener('click', ()=>{ if(confirm('Wipe all stored encrypted messages?')){ localStorage.removeItem(STORE_KEY); renderStore(); }});

renderStore();
refreshMonitor(true);

/* Demo seed messages */
['Welcome to the feed.','Color coding helps context.','Trending shows hot terms.'].forEach(t=>addMsg(t,'you'));
</script>

</body>
</html>
