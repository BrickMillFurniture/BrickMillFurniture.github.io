<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Brick Mill Furniture — Virtual Showroom</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;1,400&family=Cormorant+Garamond:wght@300;400&family=Jost:wght@300;400;500&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;}
:root{
  --bark:#2C1F14;--walnut:#4A3728;--cedar:#7A5C44;
  --sand:#C4A882;--cream:#F2EBE0;--gold:#B8946A;
  --danger:#c0392b;
}
body{font-family:'Jost',sans-serif;background:var(--bark);color:var(--cream);overflow:hidden;height:100vh;}

/* ── VIEWS ── */
#view-enter,#view-showroom,#view-admin{position:fixed;inset:0;display:none;}
#view-enter{display:flex;flex-direction:column;align-items:center;justify-content:center;gap:0;background:var(--bark);}

/* ── ENTER ── */
.e-sub{font-family:'Cormorant Garamond',serif;font-size:.85rem;letter-spacing:.3em;text-transform:uppercase;color:var(--sand);margin-bottom:16px;}
.e-title{font-family:'Playfair Display',serif;font-size:2.6rem;text-align:center;line-height:1.2;color:var(--cream);}
.e-title em{font-style:italic;color:var(--gold);}
.e-line{width:60px;height:1px;background:linear-gradient(to right,transparent,var(--gold),transparent);margin:18px auto;}
.e-desc{font-size:.75rem;color:rgba(196,168,130,.5);text-align:center;line-height:1.8;margin-bottom:32px;}
.e-btns{display:flex;gap:12px;flex-wrap:wrap;justify-content:center;margin-bottom:20px;}
.e-link{margin-top:4px;font-size:.62rem;letter-spacing:.12em;text-transform:uppercase;color:rgba(196,168,130,.4);text-align:center;}
.e-link a{color:var(--sand);text-decoration:none;}
.e-link a:hover{color:var(--gold);}
.btn-gold{background:var(--gold);color:var(--bark);border:none;font-family:'Jost',sans-serif;font-size:.68rem;letter-spacing:.22em;text-transform:uppercase;padding:13px 32px;cursor:pointer;transition:background .25s;}
.btn-gold:hover{background:var(--sand);}
.btn-ghost{background:transparent;color:var(--cream);border:1px solid rgba(196,168,130,.4);font-family:'Jost',sans-serif;font-size:.68rem;letter-spacing:.22em;text-transform:uppercase;padding:13px 32px;cursor:pointer;transition:all .25s;text-decoration:none;display:inline-block;}
.btn-ghost:hover{border-color:var(--gold);color:var(--gold);}

/* ── SHOWROOM ── */
#sr-header{position:fixed;top:0;left:0;right:0;z-index:50;display:flex;align-items:center;justify-content:space-between;padding:14px 28px;background:linear-gradient(to bottom,rgba(44,31,20,.95) 60%,transparent);}
#sr-logo{font-family:'Playfair Display',serif;font-size:1.1rem;letter-spacing:.08em;color:var(--cream);}
#sr-logo em{font-style:italic;color:var(--gold);}
#sr-room-name{font-family:'Cormorant Garamond',serif;font-size:.9rem;letter-spacing:.2em;text-transform:uppercase;color:var(--sand);font-weight:300;}
.sr-header-btns{display:flex;gap:10px;align-items:center;}
.sr-header-btns a,.sr-header-btns button{font-size:.58rem;letter-spacing:.15em;text-transform:uppercase;padding:6px 12px;border:1px solid rgba(196,168,130,.2);color:rgba(196,168,130,.5);background:transparent;cursor:pointer;font-family:'Jost',sans-serif;text-decoration:none;transition:all .25s;}
.sr-header-btns a:hover,.sr-header-btns button:hover{border-color:var(--gold);color:var(--gold);}

#sr-tabs{position:fixed;top:56px;left:0;right:0;z-index:49;display:flex;justify-content:center;overflow-x:auto;}
.sr-tab{font-size:.58rem;letter-spacing:.18em;text-transform:uppercase;padding:7px 18px;background:transparent;border:none;border-bottom:1px solid rgba(196,168,130,.1);color:rgba(196,168,130,.35);cursor:pointer;font-family:'Jost',sans-serif;white-space:nowrap;transition:all .25s;}
.sr-tab.active{color:var(--gold);border-bottom-color:var(--gold);}

#sr-viewer{width:100vw;height:100vh;position:relative;overflow:hidden;}
.scene{position:absolute;inset:0;opacity:0;transition:opacity .8s;pointer-events:none;}
.scene.active{opacity:1;pointer-events:all;}

/* Gradient room backgrounds */
.bg-dining{background:linear-gradient(170deg,#2a1a0d,#4a3020 25%,#664030 45%,#7a5035 55%,#251508);}
.bg-bedroom{background:linear-gradient(168deg,#1e1409,#382618 28%,#503420 48%,#604030 58%,#1a0f07);}
.bg-office{background:linear-gradient(172deg,#251708,#40280f 25%,#58381a 44%,#6a4520 55%,#1e1208);}
.bg-living{background:linear-gradient(175deg,#3d2a1a,#5c3d24 25%,#7a5230 45%,#8b6240 55%,#2c1a0e);}
.bg-other{background:linear-gradient(170deg,#221508,#3a2814 25%,#503822 45%,#1c1006);}

.scene-bg{position:absolute;inset:0;}
.scene-img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;}
.scene-dim{position:absolute;inset:0;background:linear-gradient(to bottom,rgba(20,10,3,.45) 0%,transparent 22%,transparent 65%,rgba(20,10,3,.55) 100%);pointer-events:none;}

/* Hotspots */
.hotspot{position:absolute;transform:translate(-50%,-50%);cursor:pointer;z-index:20;}
.hs-ring{width:36px;height:36px;border-radius:50%;border:1.5px solid rgba(196,168,130,.65);display:flex;align-items:center;justify-content:center;animation:pulse 2.8s ease-in-out infinite;transition:border-color .3s;}
.hotspot:hover .hs-ring{border-color:var(--gold);animation:none;}
.hs-dot{width:8px;height:8px;border-radius:50%;background:var(--gold);transition:transform .3s;}
.hotspot:hover .hs-dot{transform:scale(1.3);}
.hs-tip{position:absolute;bottom:calc(100% + 8px);left:50%;transform:translateX(-50%);background:rgba(44,31,20,.95);border:1px solid rgba(196,168,130,.3);color:var(--cream);font-size:.6rem;letter-spacing:.1em;text-transform:uppercase;padding:4px 9px;white-space:nowrap;opacity:0;pointer-events:none;transition:opacity .2s;}
.hotspot:hover .hs-tip{opacity:1;}
@keyframes pulse{0%,100%{box-shadow:0 0 0 0 rgba(196,168,130,.4);}50%{box-shadow:0 0 0 8px rgba(196,168,130,0);}}

/* Nav */
#sr-nav{position:fixed;bottom:28px;left:50%;transform:translateX(-50%);z-index:50;display:flex;align-items:center;gap:12px;}
.nav-btn{width:46px;height:46px;border-radius:50%;background:rgba(44,31,20,.75);border:1px solid rgba(196,168,130,.28);color:var(--cream);font-size:.95rem;cursor:pointer;display:flex;align-items:center;justify-content:center;backdrop-filter:blur(6px);transition:all .25s;}
.nav-btn:hover{border-color:var(--gold);}
.nav-btn:disabled{opacity:.2;cursor:default;}
#sr-dots{display:flex;gap:6px;align-items:center;flex-wrap:wrap;max-width:180px;justify-content:center;}
.sr-dot{width:5px;height:5px;border-radius:50%;background:rgba(196,168,130,.25);cursor:pointer;transition:all .3s;}
.sr-dot.active{background:var(--gold);transform:scale(1.5);}

/* Product panel */
#sr-panel{position:fixed;top:0;right:0;width:330px;height:100vh;background:var(--bark);border-left:1px solid rgba(196,168,130,.15);z-index:200;transform:translateX(100%);transition:transform .45s cubic-bezier(.25,.46,.45,.94);display:flex;flex-direction:column;}
#sr-panel.open{transform:translateX(0);}
#panel-img{width:100%;height:200px;background:linear-gradient(135deg,var(--walnut),var(--cedar));display:flex;align-items:center;justify-content:center;font-size:3rem;flex-shrink:0;overflow:hidden;position:relative;}
#panel-img img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;}
#panel-close{position:absolute;top:12px;left:12px;width:28px;height:28px;border-radius:50%;background:rgba(44,31,20,.75);border:1px solid rgba(196,168,130,.3);color:var(--cream);cursor:pointer;font-size:.75rem;z-index:10;display:flex;align-items:center;justify-content:center;}
#panel-body{padding:22px 24px;flex:1;overflow-y:auto;}
#panel-cat{font-size:.56rem;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:5px;}
#panel-name{font-family:'Playfair Display',serif;font-size:1.4rem;line-height:1.2;margin-bottom:7px;}
#panel-price{font-family:'Cormorant Garamond',serif;font-size:1rem;color:var(--sand);margin-bottom:12px;font-weight:300;}
#panel-desc{font-size:.78rem;line-height:1.8;color:rgba(242,235,224,.65);font-weight:300;margin-bottom:16px;}
#panel-details{border-top:1px solid rgba(196,168,130,.1);padding-top:14px;}
.det-row{display:flex;justify-content:space-between;font-size:.68rem;padding:4px 0;border-bottom:1px solid rgba(196,168,130,.05);color:rgba(242,235,224,.55);}
.det-row span:first-child{font-size:.56rem;letter-spacing:.14em;text-transform:uppercase;color:var(--sand);}
#panel-cta{display:block;margin:16px 24px 18px;background:var(--gold);color:var(--bark);text-align:center;padding:12px;font-size:.64rem;letter-spacing:.2em;text-transform:uppercase;font-family:'Jost',sans-serif;text-decoration:none;flex-shrink:0;transition:background .25s;}
#panel-cta:hover{background:var(--sand);}

/* Empty scene */
#sr-empty{position:absolute;inset:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:10px;color:rgba(196,168,130,.35);pointer-events:none;}
#sr-empty h3{font-family:'Playfair Display',serif;font-size:1.3rem;font-weight:400;}
#sr-empty p{font-size:.72rem;letter-spacing:.1em;}

/* ── ADMIN ── */
#view-admin{flex-direction:column;background:#120d07;}
#admin-topbar{display:flex;align-items:center;background:#0e0904;border-bottom:1px solid rgba(196,168,130,.1);flex-shrink:0;}
.atab{font-size:.6rem;letter-spacing:.18em;text-transform:uppercase;padding:15px 20px;background:transparent;border:none;border-bottom:2px solid transparent;color:rgba(196,168,130,.38);cursor:pointer;font-family:'Jost',sans-serif;transition:all .25s;}
.atab.active{color:var(--gold);border-bottom-color:var(--gold);}
.atab:hover{color:var(--sand);}
#admin-right{margin-left:auto;display:flex;gap:8px;padding-right:12px;}
.atab-sm{padding:8px 14px;font-size:.58rem;}

#admin-stats{display:flex;background:#0a0704;border-bottom:1px solid rgba(196,168,130,.07);flex-shrink:0;}
.stat{padding:10px 22px;border-right:1px solid rgba(196,168,130,.07);}
.stat-n{font-family:'Playfair Display',serif;font-size:1.3rem;color:var(--gold);}
.stat-l{font-size:.52rem;letter-spacing:.16em;text-transform:uppercase;color:rgba(196,168,130,.35);}

#admin-body{flex:1;overflow:hidden;display:flex;}
.apanel{display:none;flex:1;overflow:hidden;flex-direction:column;}
.apanel.active{display:flex;}

/* Split layout */
.asplit{display:flex;flex:1;overflow:hidden;}
.alist{width:300px;border-right:1px solid rgba(196,168,130,.1);display:flex;flex-direction:column;flex-shrink:0;}
.alist-hdr{padding:14px 18px;border-bottom:1px solid rgba(196,168,130,.1);display:flex;align-items:center;justify-content:space-between;flex-shrink:0;}
.alist-hdr h3{font-family:'Playfair Display',serif;font-size:.95rem;font-weight:400;}
.asearch{padding:10px 14px;border-bottom:1px solid rgba(196,168,130,.07);}
.asearch input{width:100%;background:rgba(255,255,255,.04);border:1px solid rgba(196,168,130,.13);color:var(--cream);padding:7px 11px;font-family:'Jost',sans-serif;font-size:.73rem;outline:none;}
.asearch input:focus{border-color:rgba(196,168,130,.35);}
.asearch input::placeholder{color:rgba(196,168,130,.3);}
.alist-scroll{flex:1;overflow-y:auto;}
.aitem{padding:11px 18px;border-bottom:1px solid rgba(196,168,130,.06);cursor:pointer;display:flex;align-items:center;gap:9px;transition:background .2s;}
.aitem:hover{background:rgba(196,168,130,.05);}
.aitem.sel{background:rgba(184,148,106,.1);border-left:2px solid var(--gold);}
.aitem-icon{font-size:1.1rem;flex-shrink:0;}
.aitem-name{font-size:.78rem;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;}
.aitem-meta{font-size:.6rem;color:rgba(196,168,130,.4);margin-top:2px;}
.alist-empty{padding:36px 18px;text-align:center;color:rgba(196,168,130,.28);font-size:.72rem;}

/* Form */
.aform{flex:1;overflow-y:auto;padding:24px 28px;}
.aform h3{font-family:'Playfair Display',serif;font-size:1.1rem;font-weight:400;margin-bottom:20px;padding-bottom:10px;border-bottom:1px solid rgba(196,168,130,.1);}
.frow{margin-bottom:15px;}
.frow label{display:block;font-size:.57rem;letter-spacing:.18em;text-transform:uppercase;color:var(--sand);margin-bottom:5px;}
.frow input,.frow select,.frow textarea{width:100%;background:rgba(255,255,255,.04);border:1px solid rgba(196,168,130,.13);color:var(--cream);padding:9px 12px;font-family:'Jost',sans-serif;font-size:.78rem;outline:none;transition:border-color .2s;}
.frow input:focus,.frow select:focus,.frow textarea:focus{border-color:rgba(196,168,130,.4);}
.frow select option{background:#2c1f14;}
.frow textarea{resize:vertical;min-height:80px;}
.fgrid{display:grid;grid-template-columns:1fr 1fr;gap:12px;}
.faction{display:flex;gap:8px;margin-top:20px;padding-top:16px;border-top:1px solid rgba(196,168,130,.08);}
.fph{display:flex;flex-direction:column;align-items:center;justify-content:center;height:100%;color:rgba(196,168,130,.25);gap:8px;}
.fph span{font-size:2.2rem;}
.fph p{font-size:.7rem;letter-spacing:.1em;}

/* Buttons */
.btn-sm{font-size:.56rem;letter-spacing:.16em;text-transform:uppercase;padding:7px 13px;background:var(--gold);color:var(--bark);border:none;cursor:pointer;font-family:'Jost',sans-serif;transition:background .2s;}
.btn-sm:hover{background:var(--sand);}
.btn-ghost-sm{background:transparent;border:1px solid rgba(196,168,130,.28);color:var(--sand);}
.btn-ghost-sm:hover{background:rgba(196,168,130,.08);color:var(--cream);}
.btn-danger{background:var(--danger);color:#fff;}
.btn-danger:hover{background:#a93226;}

/* Hotspot editor */
#hs-wrap{flex:1;position:relative;overflow:hidden;background:#08050e;display:flex;}
#hs-canvas{flex:1;position:relative;cursor:crosshair;overflow:hidden;}
#hs-canvas-bg{position:absolute;inset:0;}
#hs-canvas-img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;display:none;}
#hs-canvas-dots{position:absolute;inset:0;pointer-events:none;}
#hs-canvas-click{position:absolute;inset:0;z-index:10;}
#hs-empty-msg{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;color:rgba(196,168,130,.28);font-size:.75rem;letter-spacing:.1em;pointer-events:none;}
#hs-hint-bar{position:absolute;bottom:10px;left:50%;transform:translateX(-50%);font-size:.52rem;letter-spacing:.12em;text-transform:uppercase;color:rgba(196,168,130,.4);background:rgba(0,0,0,.5);padding:3px 10px;white-space:nowrap;pointer-events:none;z-index:5;display:none;}
.hs-dot{position:absolute;transform:translate(-50%,-50%);width:30px;height:30px;border-radius:50%;border:2px solid var(--gold);background:rgba(184,148,106,.18);display:flex;align-items:center;justify-content:center;pointer-events:none;}
.hs-dot-in{width:7px;height:7px;border-radius:50%;background:var(--gold);}
.hs-dot-lbl{position:absolute;bottom:calc(100% + 5px);left:50%;transform:translateX(-50%);background:rgba(44,31,20,.92);border:1px solid rgba(196,168,130,.25);color:var(--cream);font-size:.52rem;padding:2px 7px;white-space:nowrap;}
.hs-dot-rm{position:absolute;top:-5px;right:-5px;width:15px;height:15px;border-radius:50%;background:var(--danger);border:none;color:#fff;font-size:.5rem;cursor:pointer;display:flex;align-items:center;justify-content:center;pointer-events:all;}
#hs-sidebar{width:250px;border-left:1px solid rgba(196,168,130,.1);display:flex;flex-direction:column;overflow-y:auto;padding:18px;flex-shrink:0;}
#hs-sidebar h4{font-family:'Playfair Display',serif;font-size:.9rem;font-weight:400;margin-bottom:4px;}
#hs-sidebar p{font-size:.62rem;color:rgba(196,168,130,.4);line-height:1.6;margin-bottom:14px;}
.hs-item{padding:8px 10px;background:rgba(255,255,255,.03);border:1px solid rgba(196,168,130,.08);margin-bottom:6px;display:flex;align-items:center;gap:7px;}
.hs-item-num{font-size:.62rem;color:var(--gold);font-weight:500;flex-shrink:0;}
.hs-item select{flex:1;background:rgba(255,255,255,.04);border:1px solid rgba(196,168,130,.1);color:var(--cream);padding:3px 6px;font-family:'Jost',sans-serif;font-size:.65rem;}
.hs-item button{background:none;border:none;color:var(--danger);cursor:pointer;font-size:.75rem;flex-shrink:0;}
.hs-empty-txt{font-size:.62rem;color:rgba(196,168,130,.3);text-align:center;margin-top:10px;line-height:1.6;}

/* Image uploader */
.img-uploader{margin-top:6px;}
.img-drop{width:100%;height:110px;border:1.5px dashed rgba(196,168,130,.22);display:flex;flex-direction:column;align-items:center;justify-content:center;cursor:pointer;position:relative;background:rgba(255,255,255,.02);transition:all .25s;}
.img-drop:hover,.img-drop.over{border-color:var(--gold);background:rgba(184,148,106,.06);}
.img-drop input{position:absolute;inset:0;opacity:0;cursor:pointer;width:100%;height:100%;}
.img-drop-icon{font-size:1.4rem;opacity:.45;margin-bottom:4px;}
.img-drop-lbl{font-size:.58rem;letter-spacing:.1em;color:rgba(196,168,130,.35);text-align:center;pointer-events:none;}
.img-drop-lbl strong{color:var(--gold);font-weight:400;}
.img-preview{display:none;position:relative;margin-top:6px;}
.img-preview img{width:100%;height:100px;object-fit:cover;display:block;}
.img-preview-rm{position:absolute;top:5px;right:5px;width:20px;height:20px;border-radius:50%;background:rgba(192,57,43,.85);border:none;color:#fff;cursor:pointer;font-size:.6rem;display:flex;align-items:center;justify-content:center;}
.img-note{font-size:.56rem;color:rgba(196,168,130,.3);margin-top:4px;line-height:1.5;}

/* Toast */
#toast{position:fixed;bottom:20px;left:50%;transform:translateX(-50%) translateY(50px);background:rgba(74,55,40,.96);border:1px solid rgba(196,168,130,.25);color:var(--cream);padding:9px 20px;font-size:.7rem;letter-spacing:.1em;z-index:9999;transition:transform .3s;pointer-events:none;white-space:nowrap;}
#toast.show{transform:translateX(-50%) translateY(0);}

/* PW modal */
#pw-modal{position:fixed;inset:0;z-index:5000;background:rgba(18,10,4,.9);display:none;align-items:center;justify-content:center;flex-direction:column;gap:14px;backdrop-filter:blur(4px);}
#pw-modal.show{display:flex;}
#pw-modal h3{font-family:'Playfair Display',serif;font-size:1.2rem;font-weight:400;}
#pw-input{background:rgba(255,255,255,.05);border:1px solid rgba(196,168,130,.28);color:var(--cream);padding:11px 16px;font-family:'Jost',sans-serif;font-size:.85rem;width:220px;outline:none;text-align:center;letter-spacing:.2em;}
#pw-err{font-size:.62rem;color:var(--danger);min-height:14px;}

/* Scrollbar */
::-webkit-scrollbar{width:3px;}
::-webkit-scrollbar-track{background:rgba(255,255,255,.02);}
::-webkit-scrollbar-thumb{background:rgba(196,168,130,.18);border-radius:2px;}
</style>
</head>
<body>

<!-- PW MODAL -->
<div id="pw-modal">
  <h3>Admin Access</h3>
  <input type="password" id="pw-input" placeholder="Password" onkeydown="if(event.key==='Enter')checkPw()">
  <div id="pw-err"></div>
  <button class="btn-gold" onclick="checkPw()">Enter</button>
  <button class="btn-ghost" style="padding:10px 24px;" onclick="document.getElementById('pw-modal').classList.remove('show')">Cancel</button>
</div>

<!-- TOAST -->
<div id="toast"></div>

<!-- ═══════════════════════════════
     ENTER
═══════════════════════════════ -->
<div id="view-enter">
  <p class="e-sub">Virtual Showroom</p>
  <div class="e-line"></div>
  <h1 class="e-title">Brick Mill<br><em>Furniture</em></h1>
  <div class="e-line"></div>
  <p class="e-desc">Explore our handcrafted collection<br>across curated room settings</p>
  <div class="e-btns">
    <button class="btn-ghost" onclick="showPw()">⚙ Manage</button>
    <button class="btn-gold" onclick="goShowroom()">Enter Showroom</button>
  </div>
  <div class="e-link">
    <a href="https://my.matterport.com/show/?m=Gdbhu5AyJJS" target="_blank">🏛 Tour our real showroom →</a>
  </div>
</div>

<!-- ═══════════════════════════════
     SHOWROOM
═══════════════════════════════ -->
<div id="view-showroom">
  <div id="sr-header">
    <div id="sr-logo">Brick Mill <em>Furniture</em></div>
    <div id="sr-room-name"></div>
    <div class="sr-header-btns">
      <a href="https://my.matterport.com/show/?m=Gdbhu5AyJJS" target="_blank">🏛 Real Showroom</a>
      <a href="https://brickmillfurniture.com" target="_blank">Visit Website</a>
      <button onclick="showPw()">⚙ Manage</button>
      <button onclick="goEnter()">← Exit</button>
    </div>
  </div>
  <div id="sr-tabs"></div>
  <div id="sr-viewer">
    <div id="sr-empty">
      <span style="font-size:2.5rem">🪑</span>
      <h3>No Rooms Yet</h3>
      <p>Add rooms in the admin panel</p>
    </div>
  </div>
  <div id="sr-panel">
    <button id="panel-close" onclick="closePanel()">✕</button>
    <div id="panel-img"><span id="panel-emoji">🪑</span></div>
    <div id="panel-body">
      <div id="panel-cat"></div>
      <div id="panel-name"></div>
      <div id="panel-price"></div>
      <div id="panel-desc"></div>
      <div id="panel-details"></div>
    </div>
    <a id="panel-cta" href="#" target="_blank">View on Website →</a>
  </div>
  <div id="sr-nav">
    <button class="nav-btn" id="btn-prev" onclick="navigate(-1)">←</button>
    <div id="sr-dots"></div>
    <button class="nav-btn" id="btn-next" onclick="navigate(1)">→</button>
  </div>
</div>

<!-- ═══════════════════════════════
     ADMIN
═══════════════════════════════ -->
<div id="view-admin">
  <div id="admin-topbar">
    <button class="atab active" onclick="switchTab(this,'ap-products')">Products</button>
    <button class="atab" onclick="switchTab(this,'ap-rooms')">Rooms</button>
    <button class="atab" onclick="switchTab(this,'ap-hotspots')">Place Hotspots</button>
    <div id="admin-right">
      <button class="atab atab-sm" onclick="exportData()" style="color:var(--gold);">⬇ Export</button>
      <label class="atab atab-sm" style="cursor:pointer;">⬆ Import<input type="file" accept=".json" onchange="importData(event)" style="display:none;"></label>
      <button class="atab atab-sm" onclick="goEnter()">← Back</button>
    </div>
  </div>
  <div id="admin-stats">
    <div class="stat"><div class="stat-n" id="sn-p">0</div><div class="stat-l">Products</div></div>
    <div class="stat"><div class="stat-n" id="sn-r">0</div><div class="stat-l">Rooms</div></div>
    <div class="stat"><div class="stat-n" id="sn-h">0</div><div class="stat-l">Hotspots</div></div>
  </div>
  <div id="admin-body">

    <!-- PRODUCTS -->
    <div class="apanel active" id="ap-products">
      <div class="asplit">
        <div class="alist">
          <div class="alist-hdr"><h3>Products</h3><button class="btn-sm" onclick="newProduct()">+ Add</button></div>
          <div class="asearch"><input id="psearch" placeholder="Search…" oninput="renderPList()"></div>
          <div class="alist-scroll" id="plist"></div>
        </div>
        <div class="aform" id="pform"><div class="fph"><span>📦</span><p>Select or add a product</p></div></div>
      </div>
    </div>

    <!-- ROOMS -->
    <div class="apanel" id="ap-rooms">
      <div class="asplit">
        <div class="alist">
          <div class="alist-hdr"><h3>Rooms</h3><button class="btn-sm" onclick="newRoom()">+ Add</button></div>
          <div class="asearch"><input id="rsearch" placeholder="Search…" oninput="renderRList()"></div>
          <div class="alist-scroll" id="rlist"></div>
        </div>
        <div class="aform" id="rform"><div class="fph"><span>🏠</span><p>Select or add a room</p></div></div>
      </div>
    </div>

    <!-- HOTSPOTS -->
    <div class="apanel" id="ap-hotspots">
      <div style="display:flex;flex:1;overflow:hidden;">
        <div class="alist" style="width:220px;">
          <div class="alist-hdr"><h3>Rooms</h3></div>
          <div class="alist-scroll" id="hs-rlist"></div>
        </div>
        <div id="hs-wrap">
          <div id="hs-canvas">
            <div id="hs-canvas-bg"></div>
            <img id="hs-canvas-img" alt="">
            <div id="hs-canvas-dots"></div>
            <div id="hs-canvas-click"></div>
            <div id="hs-empty-msg">Select a room to place hotspots</div>
            <div id="hs-hint-bar">Click anywhere to place a hotspot</div>
          </div>
          <div id="hs-sidebar">
            <h4>Hotspots</h4>
            <p>Click the room preview to place a dot, then assign a product.</p>
            <div id="hs-list"></div>
            <div class="hs-empty-txt" id="hs-empty-txt">Select a room to begin</div>
          </div>
        </div>
      </div>
    </div>

  </div>
</div>

<script>
// ═══════════════════════════
// CONFIG
// ═══════════════════════════
const PW = 'showroom2024';
const CATS = ['Dining Room','Bedroom','Office','Living Room','Other'];
const CAT_BG = {'Dining Room':'bg-dining','Bedroom':'bg-bedroom','Office':'bg-office','Living Room':'bg-living','Other':'bg-other'};
const CAT_EM = {'Dining Room':'🍽️','Bedroom':'🛏️','Office':'📚','Living Room':'🛋️','Other':'🏠'};

// ═══════════════════════════
// STATE
// ═══════════════════════════
let db = {products:[], rooms:[]};
let selProduct = null, selRoom = null, selHsRoom = null;
let curScene = 0, curCatRooms = [], activeCat = null;
const imgStore = {};

// ═══════════════════════════
// STORAGE
// ═══════════════════════════
async function saveDb() {
  try { await window.storage.set('bm-showroom', JSON.stringify(db)); } catch(e){}
}
async function loadDb() {
  try {
    const r = await window.storage.get('bm-showroom');
    if (r && r.value) { const p = JSON.parse(r.value); db.products = p.products||[]; db.rooms = p.rooms||[]; }
  } catch(e){}
}

// ═══════════════════════════
// VIEWS
// ═══════════════════════════
function goEnter() { show('view-enter'); }
function goShowroom() { show('view-showroom'); buildShowroom(); }
function goAdmin() { show('view-admin'); refreshAdmin(); }
function show(id) {
  ['view-enter','view-showroom','view-admin'].forEach(v => {
    document.getElementById(v).style.display = v===id ? 'flex' : 'none';
  });
}

// ═══════════════════════════
// PASSWORD
// ═══════════════════════════
function showPw() {
  document.getElementById('pw-modal').classList.add('show');
  document.getElementById('pw-input').value='';
  document.getElementById('pw-err').textContent='';
  setTimeout(()=>document.getElementById('pw-input').focus(),100);
}
function checkPw() {
  if (document.getElementById('pw-input').value === PW) {
    document.getElementById('pw-modal').classList.remove('show');
    goAdmin();
  } else {
    document.getElementById('pw-err').textContent = 'Incorrect password';
  }
}

// ═══════════════════════════
// TOAST
// ═══════════════════════════
function toast(msg) {
  const t = document.getElementById('toast');
  t.textContent = msg; t.classList.add('show');
  setTimeout(()=>t.classList.remove('show'), 2500);
}

// ═══════════════════════════
// SHOWROOM
// ═══════════════════════════
function buildShowroom() {
  const viewer = document.getElementById('sr-viewer');
  const tabs = document.getElementById('sr-tabs');
  const dots = document.getElementById('sr-dots');
  viewer.querySelectorAll('.scene').forEach(s=>s.remove());
  tabs.innerHTML=''; dots.innerHTML='';

  const cats = [...new Set(db.rooms.map(r=>r.category))].filter(Boolean);
  if (!cats.length) { document.getElementById('sr-empty').style.display='flex'; updateNav(); return; }
  document.getElementById('sr-empty').style.display='none';

  cats.forEach((cat,i)=>{
    const btn = document.createElement('button');
    btn.className = 'sr-tab'+(i===0?' active':'');
    btn.textContent = cat;
    btn.onclick = ()=>{
      document.querySelectorAll('.sr-tab').forEach(b=>b.classList.remove('active'));
      btn.classList.add('active');
      activeCat=cat; curScene=0;
      buildScenes(cat);
    };
    tabs.appendChild(btn);
  });

  activeCat = cats[0];
  buildScenes(cats[0]);
}

function buildScenes(cat) {
  const viewer = document.getElementById('sr-viewer');
  const dots = document.getElementById('sr-dots');
  viewer.querySelectorAll('.scene').forEach(s=>s.remove());
  dots.innerHTML='';

  curCatRooms = db.rooms.filter(r=>r.category===cat);
  if (!curCatRooms.length) { updateNav(); return; }

  curCatRooms.forEach((room,i)=>{
    const scene = document.createElement('div');
    scene.className = 'scene'+(i===0?' active':'');

    const bg = document.createElement('div');
    bg.className = 'scene-bg '+(CAT_BG[room.category]||'bg-other');

    if (room.imageUrl) {
      const img = document.createElement('img');
      img.className='scene-img'; img.src=room.imageUrl; bg.appendChild(img);
    }

    const dim = document.createElement('div'); dim.className='scene-dim'; bg.appendChild(dim);

    // Hotspots
    (room.hotspots||[]).forEach(hs=>{
      const prod = db.products.find(p=>p.id===hs.productId);
      if (!prod) return;
      const dot = document.createElement('div');
      dot.className='hotspot'; dot.style.left=hs.x+'%'; dot.style.top=hs.y+'%';
      dot.innerHTML=`<div class="hs-tip">${esc(prod.name)}</div><div class="hs-ring"><div class="hs-dot"></div></div>`;
      dot.onclick=(e)=>{e.stopPropagation();openPanel(prod);};
      scene.appendChild(dot);
    });

    scene.appendChild(bg);
    viewer.appendChild(scene);

    const dot = document.createElement('div');
    dot.className='sr-dot'+(i===0?' active':'');
    dot.onclick=()=>goScene(i);
    dots.appendChild(dot);
  });

  curScene=0; updateRoomLabel(); updateNav();
}

function goScene(i) {
  const scenes = document.querySelectorAll('#sr-viewer .scene');
  if(!scenes[i]) return;
  scenes[curScene]?.classList.remove('active');
  curScene=i; scenes[i].classList.add('active');
  document.querySelectorAll('#sr-dots .sr-dot').forEach((d,j)=>d.classList.toggle('active',j===i));
  updateRoomLabel(); updateNav(); closePanel();
}
function navigate(d) { goScene(curScene+d); }
function updateNav() {
  document.getElementById('btn-prev').disabled = curScene===0;
  document.getElementById('btn-next').disabled = curScene>=curCatRooms.length-1;
}
function updateRoomLabel() {
  const r = curCatRooms[curScene];
  document.getElementById('sr-room-name').textContent = r?r.name:'';
}

function openPanel(prod) {
  document.getElementById('panel-cat').textContent = prod.category||'';
  document.getElementById('panel-name').textContent = prod.name;
  document.getElementById('panel-price').textContent = prod.price||'';
  document.getElementById('panel-desc').textContent = prod.description||'';
  document.getElementById('panel-cta').href = prod.url||'#';

  const imgWrap = document.getElementById('panel-img');
  imgWrap.innerHTML='';
  const closeBtn = document.createElement('button');
  closeBtn.id='panel-close'; closeBtn.textContent='✕'; closeBtn.onclick=closePanel;
  imgWrap.appendChild(closeBtn);
  if (prod.imageUrl) {
    const img=document.createElement('img'); img.src=prod.imageUrl; imgWrap.appendChild(img);
  } else {
    const em=document.createElement('span'); em.textContent=prod.emoji||'🪑'; imgWrap.appendChild(em);
  }

  const dets=[];
  if(prod.wood) dets.push(['Wood',prod.wood]);
  if(prod.upholstery) dets.push(['Upholstery',prod.upholstery]);
  if(prod.dimensions) dets.push(['Dimensions',prod.dimensions]);
  if(prod.leadTime) dets.push(['Lead Time',prod.leadTime]);
  document.getElementById('panel-details').innerHTML=dets.map(([k,v])=>
    `<div class="det-row"><span>${k}</span><span>${v}</span></div>`).join('');

  document.getElementById('sr-panel').classList.add('open');
}
function closePanel() { document.getElementById('sr-panel').classList.remove('open'); }

document.getElementById('sr-viewer').addEventListener('click', closePanel);
document.addEventListener('keydown',e=>{
  if(e.key==='ArrowRight') navigate(1);
  if(e.key==='ArrowLeft') navigate(-1);
  if(e.key==='Escape') closePanel();
});

// ═══════════════════════════
// ADMIN
// ═══════════════════════════
function switchTab(el, panelId) {
  document.querySelectorAll('.atab').forEach(t=>t.classList.remove('active'));
  el.classList.add('active');
  document.querySelectorAll('.apanel').forEach(p=>p.classList.remove('active'));
  document.getElementById(panelId).classList.add('active');
  if(panelId==='ap-hotspots') renderHsRList();
}

function refreshAdmin() {
  renderPList(); renderRList(); renderHsRList(); updateStats();
}

function updateStats() {
  document.getElementById('sn-p').textContent = db.products.length;
  document.getElementById('sn-r').textContent = db.rooms.length;
  document.getElementById('sn-h').textContent = db.rooms.reduce((a,r)=>a+(r.hotspots||[]).length,0);
}

// ═══════════════════════════
// PRODUCTS
// ═══════════════════════════
function renderPList() {
  const q=(document.getElementById('psearch').value||'').toLowerCase();
  const list=document.getElementById('plist');
  const items=db.products.filter(p=>p.name.toLowerCase().includes(q)||(p.category||'').toLowerCase().includes(q));
  if(!items.length){list.innerHTML='<div class="alist-empty">No products found</div>';return;}
  list.innerHTML=items.map(p=>`
    <div class="aitem${selProduct===p.id?' sel':''}" onclick="selectProduct('${p.id}')">
      <div class="aitem-icon">${p.emoji||'🪑'}</div>
      <div><div class="aitem-name">${esc(p.name)}</div><div class="aitem-meta">${p.category||'—'} · ${p.price||'—'}</div></div>
    </div>`).join('');
}

function selectProduct(id) {
  selProduct=id; renderPList();
  const p=db.products.find(x=>x.id===id); if(p) showPForm(p);
}

function newProduct() {
  selProduct='__new__'; renderPList(); showPForm({});
}

function showPForm(p) {
  imgStore['pf']= p.imageUrl||'';
  document.getElementById('pform').innerHTML=`
    <h3>${p.id?'Edit Product':'New Product'}</h3>
    <div class="frow"><label>Product Name *</label><input id="pf-name" value="${esc(p.name||'')}"></div>
    <div class="fgrid">
      <div class="frow"><label>Category</label><select id="pf-cat">${CATS.map(c=>`<option${p.category===c?' selected':''}>${c}</option>`).join('')}</select></div>
      <div class="frow"><label>Price</label><input id="pf-price" value="${esc(p.price||'')}" placeholder="From $1,200"></div>
    </div>
    <div class="frow"><label>Description</label><textarea id="pf-desc">${esc(p.description||'')}</textarea></div>
    <div class="fgrid">
      <div class="frow"><label>Wood / Material</label><input id="pf-wood" value="${esc(p.wood||'')}"></div>
      <div class="frow"><label>Upholstery / Finish</label><input id="pf-uph" value="${esc(p.upholstery||'')}"></div>
    </div>
    <div class="fgrid">
      <div class="frow"><label>Dimensions</label><input id="pf-dim" value="${esc(p.dimensions||'')}"></div>
      <div class="frow"><label>Lead Time</label><input id="pf-lead" value="${esc(p.leadTime||'')}"></div>
    </div>
    <div class="frow"><label>Product URL</label><input id="pf-url" value="${esc(p.url||'')}" placeholder="https://brickmillfurniture.com/products/…"></div>
    <div class="frow">
      <label>Product Photo</label>
      <div class="img-uploader">
        <div class="img-drop" id="pf-drop" ondragover="dzOver(event,'pf')" ondragleave="dzOut(event,'pf')" ondrop="dzDrop(event,'pf',900)">
          <input type="file" accept="image/*" onchange="dzChange(event,'pf',900)">
          <div class="img-drop-icon">📷</div>
          <div class="img-drop-lbl"><strong>Drop photo</strong> or click to browse</div>
        </div>
        <div class="img-preview" id="pf-preview"${p.imageUrl?' style="display:block;"':''}>
          <img id="pf-preview-img" src="${p.imageUrl||''}" alt="">
          <button class="img-preview-rm" onclick="dzClear('pf')">✕</button>
        </div>
      </div>
      <div class="img-note">Photos are stored locally — no hosting needed</div>
    </div>
    <div class="frow"><label>Emoji (fallback)</label><input id="pf-emoji" value="${esc(p.emoji||'🪑')}" style="width:70px;"></div>
    <div class="faction">
      <button class="btn-sm" onclick="saveProduct('${p.id||''}')">Save</button>
      ${p.id?`<button class="btn-sm btn-danger" onclick="deleteProduct('${p.id}')">Delete</button>`:''}
      <button class="btn-sm btn-ghost-sm" onclick="cancelPForm()">Cancel</button>
    </div>`;
  if(p.imageUrl) document.getElementById('pf-drop').style.display='none';
}

function cancelPForm() {
  selProduct=null; renderPList();
  document.getElementById('pform').innerHTML='<div class="fph"><span>📦</span><p>Select or add a product</p></div>';
}

function saveProduct(id) {
  const name=document.getElementById('pf-name').value.trim();
  if(!name){toast('Name required');return;}
  const data={
    id:id||uid(), name,
    category:document.getElementById('pf-cat').value,
    price:document.getElementById('pf-price').value.trim(),
    description:document.getElementById('pf-desc').value.trim(),
    wood:document.getElementById('pf-wood').value.trim(),
    upholstery:document.getElementById('pf-uph').value.trim(),
    dimensions:document.getElementById('pf-dim').value.trim(),
    leadTime:document.getElementById('pf-lead').value.trim(),
    url:document.getElementById('pf-url').value.trim(),
    imageUrl:imgStore['pf']||'',
    emoji:document.getElementById('pf-emoji').value.trim()||'🪑',
  };
  if(id){const i=db.products.findIndex(p=>p.id===id);if(i>-1)db.products[i]=data;}
  else db.products.push(data);
  selProduct=data.id; saveDb(); refreshAdmin(); toast('Product saved ✓');
}

function deleteProduct(id) {
  if(!confirm('Delete this product?')) return;
  db.products=db.products.filter(p=>p.id!==id);
  db.rooms.forEach(r=>{r.hotspots=(r.hotspots||[]).filter(h=>h.productId!==id);});
  selProduct=null; saveDb(); refreshAdmin(); toast('Deleted');
  document.getElementById('pform').innerHTML='<div class="fph"><span>📦</span><p>Select or add a product</p></div>';
}

// ═══════════════════════════
// ROOMS
// ═══════════════════════════
function renderRList() {
  const q=(document.getElementById('rsearch').value||'').toLowerCase();
  const list=document.getElementById('rlist');
  const items=db.rooms.filter(r=>r.name.toLowerCase().includes(q)||(r.category||'').toLowerCase().includes(q));
  if(!items.length){list.innerHTML='<div class="alist-empty">No rooms yet</div>';return;}
  list.innerHTML=items.map(r=>`
    <div class="aitem${selRoom===r.id?' sel':''}" onclick="selectRoom('${r.id}')">
      <div class="aitem-icon">${CAT_EM[r.category]||'🏠'}</div>
      <div><div class="aitem-name">${esc(r.name)}</div><div class="aitem-meta">${r.category||'—'} · ${(r.hotspots||[]).length} hotspot(s)</div></div>
    </div>`).join('');
}

function selectRoom(id) {
  selRoom=id; renderRList();
  const r=db.rooms.find(x=>x.id===id); if(r) showRForm(r);
}

function newRoom() { selRoom='__new__'; renderRList(); showRForm({}); }

function showRForm(r) {
  imgStore['rf']=r.imageUrl||'';
  document.getElementById('rform').innerHTML=`
    <h3>${r.id?'Edit Room':'New Room'}</h3>
    <div class="frow"><label>Room Name *</label><input id="rf-name" value="${esc(r.name||'')}"></div>
    <div class="frow"><label>Category</label><select id="rf-cat">${CATS.map(c=>`<option${r.category===c?' selected':''}>${c}</option>`).join('')}</select></div>
    <div class="frow">
      <label>Room Photo</label>
      <div class="img-uploader">
        <div class="img-drop" id="rf-drop" ondragover="dzOver(event,'rf')" ondragleave="dzOut(event,'rf')" ondrop="dzDrop(event,'rf',1440)">
          <input type="file" accept="image/*" onchange="dzChange(event,'rf',1440)">
          <div class="img-drop-icon">📷</div>
          <div class="img-drop-lbl"><strong>Drop room photo</strong> or click to browse<br>Wide landscape works best</div>
        </div>
        <div class="img-preview" id="rf-preview"${r.imageUrl?' style="display:block;"':''}>
          <img id="rf-preview-img" src="${r.imageUrl||''}" alt="">
          <button class="img-preview-rm" onclick="dzClear('rf')">✕</button>
        </div>
      </div>
      <div class="img-note">Leave blank to use a warm gradient background</div>
    </div>
    <div class="frow"><label>Notes (internal)</label><textarea id="rf-notes">${esc(r.notes||'')}</textarea></div>
    <div class="faction">
      <button class="btn-sm" onclick="saveRoom('${r.id||''}')">Save</button>
      ${r.id?`<button class="btn-sm btn-danger" onclick="deleteRoom('${r.id}')">Delete</button>`:''}
      <button class="btn-sm btn-ghost-sm" onclick="cancelRForm()">Cancel</button>
    </div>`;
  if(r.imageUrl) document.getElementById('rf-drop').style.display='none';
}

function cancelRForm() {
  selRoom=null; renderRList();
  document.getElementById('rform').innerHTML='<div class="fph"><span>🏠</span><p>Select or add a room</p></div>';
}

function saveRoom(id) {
  const name=document.getElementById('rf-name').value.trim();
  if(!name){toast('Name required');return;}
  const existing=id?db.rooms.find(r=>r.id===id):null;
  const data={id:id||uid(), name, category:document.getElementById('rf-cat').value,
    imageUrl:imgStore['rf']||'', notes:document.getElementById('rf-notes').value.trim(),
    hotspots:existing?existing.hotspots||[]:[],
  };
  if(id){const i=db.rooms.findIndex(r=>r.id===id);if(i>-1)db.rooms[i]=data;}
  else db.rooms.push(data);
  selRoom=data.id; saveDb(); refreshAdmin(); toast('Room saved ✓');
}

function deleteRoom(id) {
  if(!confirm('Delete room and all its hotspots?'))return;
  db.rooms=db.rooms.filter(r=>r.id!==id);
  selRoom=null; saveDb(); refreshAdmin(); toast('Deleted');
  document.getElementById('rform').innerHTML='<div class="fph"><span>🏠</span><p>Select or add a room</p></div>';
}

// ═══════════════════════════
// HOTSPOTS
// ═══════════════════════════
function renderHsRList() {
  const list=document.getElementById('hs-rlist');
  if(!db.rooms.length){list.innerHTML='<div class="alist-empty">Add rooms first</div>';return;}
  list.innerHTML=db.rooms.map(r=>`
    <div class="aitem${selHsRoom===r.id?' sel':''}" onclick="selectHsRoom('${r.id}')">
      <div class="aitem-icon">${CAT_EM[r.category]||'🏠'}</div>
      <div><div class="aitem-name">${esc(r.name)}</div><div class="aitem-meta">${(r.hotspots||[]).length} hotspot(s)</div></div>
    </div>`).join('');
}

function selectHsRoom(id) {
  selHsRoom=id; renderHsRList(); buildHsCanvas(); renderHsList();
}

function buildHsCanvas() {
  const room=db.rooms.find(r=>r.id===selHsRoom);
  const emptyMsg=document.getElementById('hs-empty-msg');
  const hintBar=document.getElementById('hs-hint-bar');
  const clickEl=document.getElementById('hs-canvas-click');

  if(!room){ emptyMsg.style.display='flex'; hintBar.style.display='none'; clickEl.onclick=null; return; }

  emptyMsg.style.display='none'; hintBar.style.display='block';

  // Background
  const bgEl=document.getElementById('hs-canvas-bg');
  const imgEl=document.getElementById('hs-canvas-img');
  if(room.imageUrl){ imgEl.src=room.imageUrl; imgEl.style.display='block'; bgEl.className=''; bgEl.style.background=''; }
  else { imgEl.style.display='none'; bgEl.className='scene-bg '+(CAT_BG[room.category]||'bg-other'); }

  // Click handler — clean assignment
  clickEl.onclick = function(e) {
    const rect=clickEl.getBoundingClientRect();
    const x=parseFloat(((e.clientX-rect.left)/rect.width*100).toFixed(2));
    const y=parseFloat(((e.clientY-rect.top)/rect.height*100).toFixed(2));
    if(!room.hotspots) room.hotspots=[];
    room.hotspots.push({x,y,productId:null});
    saveDb(); buildHsCanvas(); renderHsList(); updateStats();
    toast('Hotspot placed — assign a product →');
  };

  // Dots
  const dotsEl=document.getElementById('hs-canvas-dots');
  dotsEl.innerHTML='';
  (room.hotspots||[]).forEach((hs,i)=>{
    const prod=db.products.find(p=>p.id===hs.productId);
    const d=document.createElement('div');
    d.className='hs-dot'; d.style.left=hs.x+'%'; d.style.top=hs.y+'%';
    d.innerHTML='<div class="hs-dot-in"></div>';
    if(prod){const lbl=document.createElement('div');lbl.className='hs-dot-lbl';lbl.textContent=prod.name;d.appendChild(lbl);}
    const rm=document.createElement('button'); rm.className='hs-dot-rm'; rm.textContent='✕';
    rm.onclick=(e)=>{e.stopPropagation();room.hotspots.splice(i,1);saveDb();buildHsCanvas();renderHsList();updateStats();toast('Removed');};
    d.appendChild(rm); dotsEl.appendChild(d);
  });
}

function renderHsList() {
  const room=db.rooms.find(r=>r.id===selHsRoom);
  const list=document.getElementById('hs-list');
  const empty=document.getElementById('hs-empty-txt');
  if(!room){list.innerHTML='';empty.textContent='Select a room to begin';return;}
  if(!(room.hotspots||[]).length){list.innerHTML='';empty.textContent='Click the room to place hotspots';return;}
  empty.textContent='';
  list.innerHTML=(room.hotspots||[]).map((hs,i)=>`
    <div class="hs-item">
      <div class="hs-item-num">#${i+1}</div>
      <select onchange="assignHs(${i},this.value)">
        <option value="">— Assign product —</option>
        ${db.products.map(p=>`<option value="${p.id}"${hs.productId===p.id?' selected':''}>${esc(p.name)}</option>`).join('')}
      </select>
      <button onclick="removeHs(${i})">✕</button>
    </div>`).join('');
}

function assignHs(i,productId) {
  const room=db.rooms.find(r=>r.id===selHsRoom);
  if(!room||!room.hotspots[i])return;
  room.hotspots[i].productId=productId||null;
  saveDb(); buildHsCanvas(); toast('Product assigned ✓');
}

function removeHs(i) {
  const room=db.rooms.find(r=>r.id===selHsRoom);
  if(!room)return;
  room.hotspots.splice(i,1);
  saveDb(); buildHsCanvas(); renderHsList(); updateStats(); toast('Removed');
}

// ═══════════════════════════
// IMAGE UPLOADER
// ═══════════════════════════
function dzOver(e,key){e.preventDefault();document.getElementById(key+'-drop').classList.add('over');}
function dzOut(e,key){document.getElementById(key+'-drop').classList.remove('over');}
function dzDrop(e,key,maxW){e.preventDefault();dzOut(e,key);const f=e.dataTransfer.files[0];if(f)processImg(f,key,maxW);}
function dzChange(e,key,maxW){const f=e.target.files[0];if(f)processImg(f,key,maxW);}
function dzClear(key){
  imgStore[key]='';
  document.getElementById(key+'-preview').style.display='none';
  document.getElementById(key+'-preview-img').src='';
  document.getElementById(key+'-drop').style.display='flex';
}
function processImg(file,key,maxW) {
  if(!file.type.startsWith('image/')){toast('Please use an image file');return;}
  if(file.size>10*1024*1024){toast('File too large — please use under 10MB');return;}
  const reader=new FileReader();
  reader.onload=e=>{
    const img=new Image();
    img.onload=()=>{
      const canvas=document.createElement('canvas');
      let w=img.width,h=img.height;
      if(w>maxW){h=Math.round(h*maxW/w);w=maxW;}
      canvas.width=w;canvas.height=h;
      canvas.getContext('2d').drawImage(img,0,0,w,h);
      const data=canvas.toDataURL('image/jpeg',0.82);
      imgStore[key]=data;
      document.getElementById(key+'-preview-img').src=data;
      document.getElementById(key+'-preview').style.display='block';
      document.getElementById(key+'-drop').style.display='none';
      toast('Photo ready ✓');
    };
    img.src=e.target.result;
  };
  reader.readAsDataURL(file);
}

// ═══════════════════════════
// EXPORT / IMPORT
// ═══════════════════════════
function exportData() {
  const blob=new Blob([JSON.stringify(db,null,2)],{type:'application/json'});
  const url=URL.createObjectURL(blob);
  const a=document.createElement('a');
  a.href=url; a.download='brickmill-showroom-'+new Date().toISOString().slice(0,10)+'.json';
  a.click(); URL.revokeObjectURL(url);
  toast('Exported ✓ — save this file safely');
}
function importData(e) {
  const file=e.target.files[0]; if(!file)return;
  const reader=new FileReader();
  reader.onload=ev=>{
    try{
      const parsed=JSON.parse(ev.target.result);
      if(!parsed.products||!parsed.rooms){toast('Invalid backup file — check the file and try again');return;}
      // Merge products — add new ones, skip duplicates by id
      const existingIds = new Set(db.products.map(p=>p.id));
      const newProducts = parsed.products.filter(p=>!existingIds.has(p.id));
      db.products = [...db.products, ...newProducts];
      // Merge rooms same way
      const existingRoomIds = new Set(db.rooms.map(r=>r.id));
      const newRooms = parsed.rooms.filter(r=>!existingRoomIds.has(r.id));
      db.rooms = [...db.rooms, ...newRooms];
      saveDb(); refreshAdmin();
      toast(`Added ${newProducts.length} products, ${newRooms.length} rooms ✓`);
    }catch(err){toast('Could not read file — is it a valid backup?');}
  };
  reader.readAsText(file); e.target.value='';
}

// ═══════════════════════════
// HELPERS
// ═══════════════════════════
function uid(){return Math.random().toString(36).slice(2,10)+Date.now().toString(36);}
function esc(s){return String(s||'').replace(/&/g,'&amp;').replace(/"/g,'&quot;').replace(/</g,'&lt;').replace(/>/g,'&gt;');}

// ═══════════════════════════
// INIT
// ═══════════════════════════
(async()=>{
  await loadDb();
  refreshAdmin();
})();
</script>
</body>
</html>
