[centro-formacion-piensa-seguro-ltda.html](https://github.com/user-attachments/files/30285560/centro-formacion-piensa-seguro-ltda.html)
<!DOCTYPE html>
<html lang="es"><head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Centro de Formación · Piensa Seguro Ltda.</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@500;600;700;800&amp;family=Source+Sans+3:wght@400;500;600;700&amp;family=IBM+Plex+Mono:wght@500;600&amp;display=swap" rel="stylesheet">
<style>
:root{
  --ink:#14213D;
  --ink-2:#1B2A4A;
  --ink-3:#233355;
  --paper:#F4F3EF;
  --paper-2:#EAE7DF;
  --accent:#9C7A34;
  --accent-dim:#7C611F;
  --green:#2E7D32;
  --green-soft:#E4F1E4;
  --red:#C1121F;
  --red-soft:#FBE4E4;
  --muted:#69707E;
  --line-dark:rgba(255,255,255,0.14);
  --line-light:rgba(20,33,61,0.14);
  --display:'Barlow Condensed', sans-serif;
  --body:'Source Sans 3', sans-serif;
  --mono:'IBM Plex Mono', monospace;
}

*{box-sizing:border-box;}
html,body{margin:0;padding:0;}
body{
  font-family:var(--body);
  background:var(--paper);
  color:var(--ink);
  min-height:100vh;
  -webkit-font-smoothing:antialiased;
}
@media (prefers-reduced-motion: reduce){
  *{animation-duration:0.001ms !important; transition-duration:0.001ms !important;}
}

/* ---------- Topbar ---------- */
.topbar{
  background:var(--ink);
  color:#fff;
  padding:16px 28px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  flex-wrap:wrap;
  gap:12px;
  border-bottom:3px solid var(--accent);
}
.brand{
  display:flex;
  align-items:center;
  gap:10px;
  font-family:var(--display);
  font-weight:700;
  font-size:20px;
  letter-spacing:0.03em;
  text-transform:uppercase;
}
.brand .mark{
  width:30px;height:30px;
  border:2px solid var(--accent);
  border-radius:6px;
  display:flex;align-items:center;justify-content:center;
  color:var(--accent);
  font-weight:800;
  font-size:15px;
  transform:rotate(-6deg);
  overflow:hidden;
}
.brand .mark img{ width:100%; height:100%; object-fit:contain; transform:rotate(6deg); background:#fff; }
.steps{
  display:flex;
  gap:6px;
  font-family:var(--mono);
  font-size:11px;
  letter-spacing:0.03em;
}
.step{
  padding:6px 12px;
  border-radius:999px;
  background:rgba(255,255,255,0.06);
  color:rgba(255,255,255,0.45);
  border:1px solid var(--line-dark);
  text-transform:uppercase;
}
.step.active{
  background:var(--accent);
  color:var(--ink);
  border-color:var(--accent);
  font-weight:600;
}
.step.done{
  background:rgba(156,122,52,0.14);
  color:var(--accent);
  border-color:rgba(156,122,52,0.4);
}

/* ---------- Layout ---------- */
main{
  max-width:1040px;
  margin:0 auto;
  padding:48px 24px 90px;
}
.screen{display:none;}
.screen.active{display:block; animation:rise 0.45s ease both;}
@keyframes rise{
  from{opacity:0; transform:translateY(10px);}
  to{opacity:1; transform:translateY(0);}
}

/* ---------- Home ---------- */
.hero{
  background:var(--ink);
  color:#fff;
  border-radius:18px;
  padding:52px 40px;
  position:relative;
  overflow:hidden;
  margin-bottom:34px;
}
.hero::after{
  content:"";
  position:absolute;
  top:-40px; right:-60px;
  width:280px; height:280px;
  border:70px solid rgba(156,122,52,0.10);
  border-radius:50%;
}
.eyebrow{
  font-family:var(--mono);
  font-size:12px;
  letter-spacing:0.14em;
  text-transform:uppercase;
  color:var(--accent);
  margin:0 0 14px;
}
.hero h1{
  font-family:var(--display);
  font-weight:800;
  font-size:44px;
  line-height:1.02;
  letter-spacing:0.01em;
  margin:0 0 16px;
  max-width:640px;
}
.hero p{
  font-size:17px;
  color:rgba(255,255,255,0.72);
  max-width:560px;
  line-height:1.5;
  margin:0 0 30px;
}
.search-row{
  display:flex;
  gap:10px;
  max-width:560px;
  position:relative;
  z-index:2;
}
.search-row input{
  flex:1;
  font-family:var(--body);
  font-size:16px;
  padding:15px 18px;
  border-radius:10px;
  border:1px solid var(--line-dark);
  background:rgba(255,255,255,0.06);
  color:#fff;
}
.search-row input::placeholder{color:rgba(255,255,255,0.4);}
.search-row input:focus{outline:2px solid var(--accent); outline-offset:2px;}
.btn{
  font-family:var(--body);
  font-weight:600;
  font-size:15px;
  padding:14px 22px;
  border-radius:10px;
  border:none;
  cursor:pointer;
  transition:transform 0.15s ease, box-shadow 0.15s ease;
}
.btn:focus-visible{outline:3px solid var(--accent); outline-offset:2px;}
.btn-accent{background:var(--accent); color:var(--ink);}
.btn-accent:hover{transform:translateY(-2px); box-shadow:0 8px 18px rgba(156,122,52,0.22);}
.btn-outline{background:transparent; color:#fff; border:1px solid var(--line-dark);}
.btn-outline:hover{border-color:var(--accent); color:var(--accent);}
.btn-ghost{background:transparent; color:var(--ink); border:1px solid var(--line-light);}
.btn-ghost:hover{border-color:var(--ink);}
.hint-msg{
  font-family:var(--mono);
  font-size:12.5px;
  color:var(--accent);
  margin-top:12px;
  min-height:18px;
}

.section-label{
  font-family:var(--mono);
  font-size:12px;
  letter-spacing:0.12em;
  text-transform:uppercase;
  color:var(--muted);
  margin:0 0 14px 2px;
}
.topics-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit, minmax(190px, 1fr));
  gap:14px;
}
.topic-tile{
  background:var(--ink);
  color:#fff;
  border-radius:14px;
  padding:22px 18px;
  cursor:pointer;
  border:1px solid var(--ink);
  text-align:left;
  transition:transform 0.15s ease, border-color 0.15s ease;
  font-family:var(--body);
  position:relative;
}
.topic-tile:hover{transform:translateY(-3px); border-color:var(--accent);}
.topic-tile:focus-visible{outline:3px solid var(--accent); outline-offset:2px;}
.topic-tile .icon{
  width:38px;height:38px;
  margin-bottom:14px;
  color:var(--accent);
}
.topic-tile .icon svg{width:100%;height:100%;}
.topic-tile .name{
  font-family:var(--display);
  font-weight:700;
  font-size:19px;
  letter-spacing:0.01em;
  margin-bottom:4px;
  text-transform:uppercase;
}
.topic-tile .desc{
  font-size:13px;
  color:rgba(255,255,255,0.55);
  line-height:1.4;
}

/* ---------- Content / slides ---------- */
.content-header{
  display:flex;
  justify-content:space-between;
  align-items:flex-start;
  gap:16px;
  margin-bottom:22px;
  flex-wrap:wrap;
}
.content-header .tag{
  font-family:var(--mono);
  font-size:12px;
  letter-spacing:0.1em;
  text-transform:uppercase;
  color:var(--accent-dim);
  background:#EDE6D3;
  padding:6px 12px;
  border-radius:999px;
  display:inline-block;
  margin-bottom:8px;
}
.content-header h2{
  font-family:var(--display);
  font-size:32px;
  font-weight:700;
  margin:0;
  letter-spacing:0.01em;
}
.listen-btn{
  display:inline-flex; align-items:center; gap:8px;
  font-family:var(--mono); font-size:12.5px;
  padding:9px 14px; border-radius:999px;
  border:1px solid var(--line-light); background:#fff; color:var(--ink);
  cursor:pointer;
}
.listen-btn.playing{border-color:var(--accent); color:var(--accent-dim); background:#F1ECDD;}
.listen-btn svg{width:14px;height:14px;}

.continue-row{
  margin-top:22px;
  display:flex;
  justify-content:space-between;
  gap:10px;
}

/* ---------- Camino de módulos del pilar ---------- */
.pillar-progress-wrap{ margin-bottom:26px; }
.pillar-progress-bar{
  width:100%; height:8px; border-radius:999px; background:var(--paper-2); overflow:hidden;
  border:1px solid var(--line-light);
}
.pillar-progress-fill{
  height:100%; background:linear-gradient(90deg, var(--accent-dim), var(--accent));
  border-radius:999px; width:0%; transition:width 0.6s cubic-bezier(.3,1,.4,1);
}
.pillar-progress-label{
  font-family:var(--mono); font-size:12px; color:var(--muted); margin-top:8px;
}
.module-list{ display:flex; flex-direction:column; gap:10px; }
.module-row{
  display:flex; align-items:center; gap:16px;
  background:#fff; border:1px solid var(--line-light); border-radius:14px;
  padding:16px 20px; position:relative; overflow:hidden;
  animation:rowIn 0.4s ease both;
}
@keyframes rowIn{ from{opacity:0; transform:translateX(-8px);} to{opacity:1; transform:translateX(0);} }
.module-row.done{ border-color:rgba(46,125,50,0.35); background:#F4F9F4; }
.module-row.locked{ opacity:0.6; }
.module-num{
  width:36px; height:36px; border-radius:50%; flex-shrink:0;
  display:flex; align-items:center; justify-content:center;
  font-family:var(--mono); font-weight:600; font-size:13px;
  background:var(--paper-2); color:var(--muted); border:1px solid var(--line-light);
}
.module-row.done .module-num{ background:var(--green); color:#fff; border-color:var(--green); }
.module-row.available .module-num{ background:var(--ink); color:#fff; border-color:var(--ink); }
.module-row.locked .module-num svg{ width:16px; height:16px; }
.module-info{ flex:1; min-width:0; }
.module-info .m-title{ font-family:var(--body); font-weight:600; font-size:15px; color:var(--ink); }
.module-info .m-status{ font-family:var(--mono); font-size:11.5px; color:var(--muted); margin-top:2px; }
.module-row.done .module-info .m-status{ color:var(--green); }
.module-row-action{ flex-shrink:0; }
.btn-module{
  font-family:var(--body); font-weight:600; font-size:13px;
  padding:9px 16px; border-radius:8px; border:1px solid var(--ink);
  background:var(--ink); color:#fff; cursor:pointer;
}
.btn-module:hover{ opacity:0.88; }
.btn-module.secondary{ background:#fff; color:var(--ink); }
.btn-module:disabled{ background:var(--paper-2); border-color:var(--line-light); color:var(--muted); cursor:not-allowed; }

/* ---------- Carrusel de diapositivas del módulo (más visual y lúdico) ---------- */
.deck{ position:relative; }
.deck-slide{
  border-radius:22px; overflow:hidden; position:relative;
  min-height:420px; display:flex; flex-direction:column; align-items:center; justify-content:center;
  padding:52px 46px; text-align:center;
}
.pslide{ width:100%; max-width:640px; margin:0 auto; animation:slideIn 0.45s cubic-bezier(.2,.9,.3,1) both; position:relative; z-index:2; }
@keyframes slideIn{ from{opacity:0; transform:translateX(18px) scale(0.98);} to{opacity:1; transform:translateX(0) scale(1);} }

/* Fondo por tipo de diapositiva */
.deck-slide.bg-dark{ background:var(--ink); color:#fff; }
.deck-slide.bg-paper{ background:#fff; border:1px solid var(--line-light); }
.deck-slide.bg-tint{ background:linear-gradient(160deg, #FBF7EC, #F3ECDA); border:1px solid var(--line-light); }
.deck-slide.bg-dark .deck-blob{
  position:absolute; border-radius:50%; pointer-events:none;
  background:radial-gradient(circle, rgba(156,122,52,0.22), transparent 70%);
}
.deck-slide.bg-dark .deck-blob.b1{ width:280px; height:280px; top:-100px; left:-90px; animation:blobDrift 9s ease-in-out infinite; }
.deck-slide.bg-dark .deck-blob.b2{ width:220px; height:220px; bottom:-90px; right:-70px; animation:blobDrift 11s ease-in-out infinite reverse; }
@keyframes blobDrift{ 0%,100%{ transform:translate(0,0) scale(1); } 50%{ transform:translate(14px,-10px) scale(1.08); } }
.deck-dotgrid{
  position:absolute; inset:0; pointer-events:none; opacity:0.5;
  background-image:radial-gradient(rgba(255,255,255,0.16) 1.4px, transparent 1.4px);
  background-size:20px 20px;
}
.deck-wave{ position:absolute; left:0; right:0; bottom:-2px; width:100%; height:auto; opacity:0.9; pointer-events:none; }

/* Stickers flotantes alrededor del ícono principal (estilo collage) */
.hook-stage{ position:relative; width:150px; height:150px; margin:0 auto 22px; }
.hook-sticker{
  position:absolute; border-radius:50%; display:flex; align-items:center; justify-content:center;
  background:rgba(255,255,255,0.12); border:1.5px solid rgba(255,255,255,0.28); color:var(--accent);
  opacity:0; animation:stickerIn 0.5s ease both, stickerFloat 4s ease-in-out infinite;
}
.hook-sticker svg{ width:55%; height:55%; }
.hook-sticker.s1{ width:44px; height:44px; top:-6px; left:-14px; animation-delay:0.35s, 0.9s; }
.hook-sticker.s2{ width:36px; height:36px; bottom:2px; right:-16px; color:#fff; background:rgba(156,122,52,0.35); animation-delay:0.5s, 1.3s; }
@keyframes stickerIn{ from{opacity:0; transform:scale(0.3) rotate(-30deg);} to{opacity:1; transform:scale(1) rotate(0deg);} }
@keyframes stickerFloat{ 0%,100%{ transform:translateY(0) rotate(0deg); } 50%{ transform:translateY(-6px) rotate(6deg); } }

/* Portada (hook) */
.pslide-hook .hook-icon{
  width:104px; height:104px; border-radius:28px; background:var(--accent); color:var(--ink);
  display:flex; align-items:center; justify-content:center; padding:24px; margin:0 auto;
  animation:popIn 0.55s cubic-bezier(.2,1.4,.4,1) both, iconFloat 3.4s ease-in-out 0.6s infinite;
  box-shadow:0 16px 32px rgba(0,0,0,0.28); position:relative; z-index:2;
}
.pslide-hook .hook-icon svg{ width:100%; height:100%; }
.pslide-hook .hook-eyebrow{ font-family:var(--mono); font-size:12px; letter-spacing:0.14em; text-transform:uppercase; color:var(--accent); margin-bottom:10px; }
.pslide-hook .hook-title{ font-family:var(--display); font-weight:800; font-size:32px; line-height:1.15; margin:0 0 10px; }
.pslide-hook .hook-sub{ font-size:14.5px; color:rgba(255,255,255,0.65); }
.pslide-hook .hook-module-count{
  display:inline-flex; align-items:center; gap:6px; margin-top:16px; padding:6px 14px;
  background:rgba(255,255,255,0.08); border:1px solid rgba(255,255,255,0.18); border-radius:999px;
  font-family:var(--mono); font-size:11px; color:rgba(255,255,255,0.7);
}
@keyframes popIn{ from{opacity:0; transform:scale(0.5) rotate(-8deg);} to{opacity:1; transform:scale(1) rotate(0deg);} }
@keyframes iconFloat{ 0%,100%{transform:translateY(0) rotate(0deg);} 50%{transform:translateY(-8px) rotate(-2deg);} }

/* Concepto */
.pslide-concept .concept-icon{ width:56px; height:56px; margin:0 auto 20px; color:var(--accent-dim); animation:popIn 0.5s ease both; }
.pslide-concept .concept-icon svg{ width:100%; height:100%; }
.pslide-concept .concept-label{ font-family:var(--mono); font-size:12px; letter-spacing:0.12em; text-transform:uppercase; color:var(--muted); margin-bottom:14px; }
.pslide-concept .concept-text{ font-size:21px; line-height:1.6; color:#22262F; font-family:var(--display); font-weight:500; }
.pslide-concept .concept-rule{ width:52px; height:4px; background:var(--accent); border-radius:4px; margin:22px auto 0; }

/* Punto clave */
.pslide-point .point-badge{
  width:74px; height:74px; border-radius:50%; margin:0 auto 22px;
  display:flex; align-items:center; justify-content:center;
  font-family:var(--display); font-weight:800; font-size:30px; color:#fff;
  animation:badgeSpin 0.55s cubic-bezier(.2,1.3,.4,1) both;
  box-shadow:0 12px 26px rgba(0,0,0,0.18);
}
.pslide-point .point-badge.c1{ background:var(--accent); }
.pslide-point .point-badge.c2{ background:var(--ink); }
.pslide-point .point-badge.c3{ background:var(--green); }
@keyframes badgeSpin{ from{opacity:0; transform:scale(0.4) rotate(-40deg);} to{opacity:1; transform:scale(1) rotate(0deg);} }
.pslide-point .point-label{ font-family:var(--mono); font-size:12px; letter-spacing:0.12em; text-transform:uppercase; color:var(--muted); margin-bottom:12px; }
.pslide-point .point-text{ font-size:22px; line-height:1.5; color:var(--ink); font-family:var(--display); font-weight:600; }
.pslide-point .point-deco{ position:absolute; top:14px; right:22px; width:26px; height:26px; color:var(--line-light); opacity:0.7; animation:iconFloat 3s ease-in-out infinite; }

/* Aplícalo (nueva diapositiva de aplicación práctica) */
.pslide-apply .apply-ribbon{
  display:inline-flex; align-items:center; gap:7px; padding:6px 14px; border-radius:999px;
  background:var(--ink); color:var(--accent); font-family:var(--mono); font-size:11px; text-transform:uppercase;
  letter-spacing:0.08em; margin-bottom:20px; animation:popIn 0.45s ease both;
}
.pslide-apply .apply-ribbon svg{ width:14px; height:14px; }
.pslide-apply .apply-text{ font-size:19px; line-height:1.6; color:#22262F; font-family:var(--body); font-weight:500; max-width:540px; margin:0 auto; }
.pslide-apply .apply-icon{ width:46px; height:46px; margin:0 auto 16px; color:var(--accent-dim); animation:iconFloat 3.6s ease-in-out infinite; }
.pslide-apply .apply-icon svg{ width:100%; height:100%; }

/* Cierre / repaso */
.pslide-recap .recap-trophy{ width:52px; height:52px; margin:0 auto 14px; color:var(--accent); animation:popIn 0.5s cubic-bezier(.2,1.4,.4,1) both, iconFloat 3.6s ease-in-out 0.5s infinite; }
.pslide-recap .recap-trophy svg{ width:100%; height:100%; }
.pslide-recap .recap-title{ font-family:var(--display); font-weight:800; font-size:26px; margin:0 0 22px; }
.recap-list{ display:flex; flex-direction:column; gap:10px; text-align:left; max-width:480px; margin:0 auto; }
.recap-item{
  display:flex; align-items:flex-start; gap:10px; background:rgba(255,255,255,0.06);
  border:1px solid rgba(255,255,255,0.12); border-radius:12px; padding:12px 14px;
  opacity:0; animation:fadeUp 0.4s ease forwards;
}
.recap-item svg{ width:18px; height:18px; flex-shrink:0; color:var(--accent); margin-top:1px; }
.recap-item span{ font-size:14px; line-height:1.5; color:rgba(255,255,255,0.88); }
@keyframes fadeUp{ from{opacity:0; transform:translateY(10px);} to{opacity:1; transform:translateY(0);} }
.recap-norm{
  display:inline-flex; align-items:center; gap:8px; margin-top:22px; padding:9px 16px;
  background:rgba(156,122,52,0.18); color:var(--accent); border-radius:999px;
  font-family:var(--mono); font-size:11.5px;
  animation:fadeUp 0.4s ease 0.5s both;
}
.recap-norm svg{ width:14px; height:14px; }
.recap-cheer{
  margin-top:24px; font-family:var(--mono); font-size:12.5px; color:var(--accent);
  animation:fadeUp 0.4s ease 0.6s both;
}

/* Controles del carrusel */
.deck-controls{
  display:flex; align-items:center; justify-content:space-between;
  margin-top:16px; padding:0 4px;
}
.deck-dots{ display:flex; gap:7px; }
.deck-dot{ width:8px; height:8px; border-radius:50%; background:var(--line-light); transition:background 0.2s ease, transform 0.2s ease; cursor:pointer; }
.deck-dot.on{ background:var(--accent); transform:scale(1.3); }
.deck-dot.seen:not(.on){ background:#C9BFA0; }
.deck-nav-btns{ display:flex; gap:8px; }
.btn-small{
  font-family:var(--body); font-weight:600; font-size:13.5px;
  padding:9px 16px; border-radius:8px; border:1px solid var(--line-light);
  background:#fff; color:var(--ink); cursor:pointer;
}
.btn-small:disabled{ opacity:0.35; cursor:not-allowed; }
.btn-small:not(:disabled):hover{ border-color:var(--ink); }


/* ---------- Quiz ---------- */
.identity-card{
  background:#fff;
  border:1px solid var(--line-light);
  border-radius:14px;
  padding:26px 28px;
  margin-bottom:24px;
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:16px;
}
.identity-card .field{display:flex; flex-direction:column; gap:6px;}
.identity-card label{
  font-family:var(--mono); font-size:11.5px; letter-spacing:0.06em;
  text-transform:uppercase; color:var(--muted);
}
.identity-card input{
  font-family:var(--body); font-size:15px;
  padding:11px 13px; border-radius:8px; border:1px solid var(--line-light);
}
.identity-card input:focus{outline:2px solid var(--accent); outline-offset:1px;}

.q-card{
  background:#fff;
  border:1px solid var(--line-light);
  border-radius:14px;
  padding:24px 26px;
  margin-bottom:14px;
}
.q-card .q-num{
  font-family:var(--mono); font-size:12px; color:var(--accent-dim); margin-bottom:8px;
}
.q-card h4{
  font-family:var(--body); font-weight:600; font-size:16.5px;
  margin:0 0 16px; line-height:1.4;
}
.opt{
  display:flex; align-items:flex-start; gap:10px;
  padding:11px 12px; border-radius:9px;
  cursor:pointer; border:1px solid transparent;
  margin-bottom:4px;
}
.opt:hover{background:var(--paper-2);}
.opt input{margin-top:3px;}
.opt span{font-size:15px; line-height:1.45;}

.quiz-footer{
  display:flex; justify-content:space-between; align-items:center;
  margin-top:8px; flex-wrap:wrap; gap:12px;
}
.quiz-progress{
  font-family:var(--mono); font-size:12.5px; color:var(--muted);
}
.error-msg{
  font-family:var(--mono); font-size:12.5px; color:var(--red); margin-top:8px;
}

/* ---------- Result ---------- */
.result-wrap{
  text-align:center;
  background:#fff;
  border:1px solid var(--line-light);
  border-radius:18px;
  padding:52px 30px;
}
.gauge{
  width:180px; height:180px;
  border-radius:50%;
  margin:0 auto 26px;
  display:flex; align-items:center; justify-content:center;
  position:relative;
}
.gauge .ring{
  position:absolute; inset:0; border-radius:50%;
}
.gauge .center{
  position:relative; z-index:2;
  font-family:var(--display); font-weight:800; font-size:44px;
  color:var(--ink);
}
.gauge .center small{
  display:block; font-family:var(--mono); font-size:12px; font-weight:500;
  color:var(--muted); margin-top:2px;
}
.result-title{
  font-family:var(--display); font-weight:700; font-size:30px; margin:0 0 10px;
}
.result-msg{font-size:16px; color:#33394A; max-width:460px; margin:0 auto 26px; line-height:1.55;}
.badge-pass{color:var(--green);}
.badge-fail{color:var(--red);}
.result-actions{display:flex; gap:12px; justify-content:center; flex-wrap:wrap;}

/* ---------- Certificate ---------- */
.cert-stage{
  background:var(--ink);
  border-radius:18px;
  padding:56px 20px;
  display:flex;
  flex-direction:column;
  align-items:center;
}
.certificate{
  width:100%;
  max-width:760px;
  background:var(--paper);
  border:2px solid var(--ink);
  border-radius:6px;
  padding:0;
  position:relative;
  box-shadow:0 20px 60px rgba(0,0,0,0.35);
}
.cert-inner{
  border:1px solid rgba(20,33,61,0.35);
  margin:10px;
  padding:44px 46px 38px;
  position:relative;
}
.cert-brand-row{
  display:flex; align-items:center; justify-content:center; gap:12px;
  margin-bottom:16px;
}
.cert-brand-row img{ width:44px; height:44px; object-fit:contain; border-radius:6px; }
.cert-eyebrow{
  font-family:var(--mono); font-size:11.5px; letter-spacing:0.16em;
  text-transform:uppercase; color:var(--accent-dim); text-align:center;
  margin:0 0 6px;
}
.cert-org{
  text-align:center; font-family:var(--display); font-weight:700;
  font-size:16px; letter-spacing:0.08em; text-transform:uppercase; color:var(--ink);
  margin:0;
}
.cert-nit{
  text-align:center; font-family:var(--mono); font-size:10.5px; color:var(--muted);
  margin:2px 0 0;
}
.cert-title{
  text-align:center; font-family:var(--display); font-weight:800;
  font-size:34px; letter-spacing:0.02em; text-transform:uppercase; color:var(--ink);
  margin:0 0 6px;
  padding:0 108px;
}
.cert-sub{
  text-align:center; font-family:var(--body); font-size:14px; color:var(--muted);
  margin:0 0 30px;
}
.cert-name{
  text-align:center; font-family:var(--display); font-weight:700;
  font-size:30px; color:var(--ink); margin:0 0 4px;
  border-bottom:2px solid var(--accent);
  display:inline-block; padding:0 10px 6px;
}
.cert-name-wrap{text-align:center; margin-bottom:22px;}
.cert-doc{font-family:var(--mono); font-size:12.5px; color:var(--muted);}
.cert-body-text{
  text-align:center; font-size:15px; line-height:1.6; color:#33394A;
  max-width:560px; margin:0 auto 26px;
}
.cert-body-text b{color:var(--ink);}
.cert-meta{
  display:flex; justify-content:space-between;
  border-top:1px dashed rgba(20,33,61,0.3);
  padding-top:18px; margin-top:6px;
  font-family:var(--mono); font-size:11.5px; color:var(--muted);
}
.stamp{
  position:absolute; top:26px; right:26px;
  width:78px; height:78px; border-radius:50%;
  border:3px solid var(--green);
  display:flex; align-items:center; justify-content:center;
  transform:rotate(-14deg);
  color:var(--green);
  animation:stampIn 0.5s cubic-bezier(.2,1.4,.4,1) both;
  animation-delay:0.25s;
}
.stamp svg{width:34px;height:34px;}
@keyframes stampIn{
  from{opacity:0; transform:rotate(-14deg) scale(1.8);}
  to{opacity:1; transform:rotate(-14deg) scale(1);}
}
.cert-actions{
  display:flex; gap:12px; margin-top:26px; justify-content:center; flex-wrap:wrap;
}

@media print{
  body *{visibility:hidden;}
  #certificate-print, #certificate-print *{visibility:visible;}
  #certificate-print{position:absolute; top:0; left:0; width:100%;}
  .no-print{display:none !important;}
}

@media (max-width:640px){
  .deck-slide{ padding:34px 24px; min-height:380px; }
  .pslide-hook .hook-icon{ width:80px; height:80px; }
  .pslide-hook .hook-title{ font-size:25px; }
  .pslide-point .point-badge{ width:60px; height:60px; font-size:24px; }
  .pslide-point .point-text{ font-size:18px; }
  .pslide-concept .concept-text{ font-size:18px; }
  .identity-card{grid-template-columns:1fr;}
  .hero h1{font-size:32px;}
  .steps{display:none;}
}

footer.app-footer{
  text-align:center; padding:20px; font-family:var(--mono); font-size:11.5px; color:var(--muted);
}

/* ---------- Login ---------- */
.user-badge{
  display:flex; align-items:center; gap:12px;
  font-family:var(--mono); font-size:12px; color:rgba(255,255,255,0.75);
}
.link-btn{
  background:none; border:none; color:var(--accent); font-family:var(--mono); font-size:11.5px;
  text-decoration:underline; cursor:pointer; padding:0;
}
.login-wrap{ display:flex; justify-content:center; padding:24px 0 40px; }
.login-card{
  width:100%; max-width:440px; background:#fff; border:1px solid var(--line-light);
  border-radius:16px; padding:38px 34px; box-shadow:0 1px 2px rgba(20,33,61,0.06);
}
.login-title{
  font-family:var(--display); font-weight:700; font-size:26px; margin:6px 0 10px; color:var(--ink);
}
.login-sub{ font-size:14.5px; color:var(--muted); line-height:1.5; margin:0; }
.login-card .field{ display:flex; flex-direction:column; gap:6px; margin-bottom:10px; }
.login-card label{
  font-family:var(--mono); font-size:11px; letter-spacing:0.05em; text-transform:uppercase; color:var(--muted);
}
.login-card input{
  font-family:var(--body); font-size:15px; padding:12px 13px; border-radius:8px; border:1px solid var(--line-light);
}
.login-card input:focus{ outline:2px solid var(--accent); outline-offset:1px; }
.login-divider{
  display:flex; align-items:center; gap:10px; margin:22px 0 14px;
  font-family:var(--mono); font-size:11px; color:var(--muted); text-transform:uppercase;
}
.login-divider::before, .login-divider::after{ content:""; flex:1; height:1px; background:var(--line-light); }
.btn-link-toggle{
  width:100%; background:none; border:1px dashed var(--line-light); border-radius:8px;
  padding:11px; font-family:var(--body); font-size:13.5px; color:var(--ink); cursor:pointer;
}
.btn-link-toggle:hover{ border-color:var(--ink); }
.btn-outline-dark{
  background:var(--ink); color:#fff; border:none;
}
.btn-outline-dark:hover{ opacity:0.9; }
.upload-label{
  display:block; text-align:center; font-family:var(--body); font-size:13.5px; font-weight:600;
  color:var(--ink); border:1px solid var(--line-light); border-radius:8px; padding:11px; cursor:pointer;
}
.upload-label:hover{ border-color:var(--ink); }
#registerBox{ margin-top:14px; }

/* ---------- Admin: lista de bloqueo de cursos ---------- */
.lock-row{
  display:flex; align-items:center; justify-content:space-between; gap:12px;
  padding:12px 4px; border-bottom:1px solid var(--line-light);
}
.lock-row:last-child{ border-bottom:none; }
.lock-row-name{ display:flex; align-items:center; gap:10px; font-size:14.5px; color:var(--ink); }
.lock-row-name .icon-sm{ width:20px; height:20px; color:var(--muted); flex-shrink:0; }
.lock-row-name .icon-sm svg{ width:100%; height:100%; }
.toggle{
  position:relative; width:44px; height:24px; border-radius:999px; background:#D8D3C4;
  border:none; cursor:pointer; flex-shrink:0; transition:background 0.15s ease;
}
.toggle::after{
  content:""; position:absolute; top:3px; left:3px; width:18px; height:18px; border-radius:50%;
  background:#fff; transition:transform 0.15s ease; box-shadow:0 1px 2px rgba(0,0,0,0.25);
}
.toggle.on{ background:var(--green); }
.toggle.on::after{ transform:translateX(20px); }
.lock-status{ font-family:var(--mono); font-size:10.5px; text-transform:uppercase; color:var(--muted); min-width:64px; text-align:right; }

/* ---------- Tiles bloqueados en Home ---------- */
.topic-tile.locked{ cursor:not-allowed; opacity:0.55; }
.topic-tile.locked:hover{ transform:none; border-color:var(--ink); }
.tile-lock-badge{
  position:absolute; top:14px; right:14px; display:flex; align-items:center; gap:5px;
  font-family:var(--mono); font-size:9.5px; text-transform:uppercase; color:rgba(255,255,255,0.55);
}
.tile-lock-badge svg{ width:12px; height:12px; }

</style>
</head>
<body>

<div class="topbar">
  <div class="brand" id="brandBlock"><span class="mark" id="brandMark"><img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAMCAgICAgMCAgIDAwMDBAYEBAQEBAgGBgUGCQgKCgkICQkKDA8MCgsOCwkJDRENDg8QEBEQCgwSExIQEw8QEBD/2wBDAQMDAwQDBAgEBAgQCwkLEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBD/wAARCALQA8ADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD9U6KKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAoor4k/4KPftdan8F/DUHwu+HepLb+LfEERa4uUP7yxtCMb19GbkA9qASufRnxC/aY+Bfwt+0L42+I+kWMlqu6aJZfNkT2Kpk59q47w9+3p+yl4oeePSPi1pzm3UNJ5kUkeAemNyjNfhfd3F1qF3L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EyfQ06KKKCAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA8U/bS1e/0H9lf4latpkix3VvojmNmXIBLqDx9Ca/BWMlkDnqw3H6nk1+7X7d9xFB+yP8TBK20y6OY092MiYH6V+EkX+qT/dH8qC47D6KKKCgooooAK9i/Y+8HW3jr9pTwNoV3C0kcWoLf7VODmEhgfpXjtfW/wDwS98KHXf2orLXW5j0LTrmRlxwWdMKfwNAnsfs5RVHV9d0Tw/afb9f1ix022zt868uEhjz6bnIGar6T4t8Ka9j+wvE+k6ju6fZL2ObP/fLGgzNaiivHP2ov2jvC/7N3w3u/Fer3EMmqzo0WlWJYb7ifHBx12g8mgD5w/4Kd/tSJ4E8Hj4HeD9QI17xJFnUpYW5tbTuhI+6zcY9q/J1RtAGc+/rW/478c+JfiV4v1Txz4v1CS81TVp2nld2yEBPCL6KOgrBoNErBRRRQMKtaXpepa5qdpomjWj3V/fTLBbwoMs7scAcVV5yAoJLEAAdST0FfqR/wTn/AGJj4Tt7T47/ABT0of2zcx79EsZ1z9liYf61lPRiOlAm7H0B+xF+zFZfs3/CqC01GJZfFOthbvVrgrhlYj5Yh6BQcfWvouiigzCiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA+eP+CgH/JpXxA/68B/6GK/DGL/VJ/uiv3O/4KAf8mlfED/rwH/oYr8MYv8AVJ/uiguOw6iiigoKKKKACvv7/gj7py3PxK8faiyZNnptsoPoXYj+lfANfqH/AMEgNHWPwZ4x14GPNxerb4C/P8vPJ9KBS2K//BXrw58QL7QfCOv6ZJdyeEbPzYdTt4iSn2hmzG7gdgAea/Nrw94w8XeFHjl8K+KtV0kxNuQ2d00eD+Ff0UeKPC+geM9BvfDPifS4NQ0zUIjDcW8y7ldT/nrX5k/tDf8ABKjxTpWoXniP4C6pHqWnys0i6LdvtmjJ52o542+neglPozzv4P8A/BUD47/DbS30bxbY2fjW2RQlq903kzRcfxSDl/xr59+OXxz8eftA+N7jxt471BpHYlbSzU/ubSPsqDp+NZfjX4QfFL4dahLpnjTwHrGnTQ8uzWztEP8AgYG01xq3Nu33Z0P0YUFJLoSUUA5GRUbXEC8NMgJ/2qBklKiSSyJDDG0kkjBURBlmJ6AAV6J8Lf2d/jP8ZtSTTvAPgPUbsNhmuZozDAqH+LewwfXiv04/ZR/4Ju+DPg3eWvjn4m3MPifxTGoaGEpmzs265VT95h69OKBNpHkH7BP/AAT/ALi4nsvjN8c9FaKOMrPo+h3KcseommX09F71+mccaRIsUSKiIAqqowAB0ApVVVUKqgADAAHAFLQQ3cKKKKBBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAfPH/BQD/k0r4gf9eA/9DFfhjF/qk/3RX7nf8FAP+TSviB/14D/ANDFfhjF/qk/3RQXHYdRRRQUFFFFABX62f8ABIu0Cfs/a3fGJQZvENwgfHJ2gZH4ZFfkkx2qT6DNfsj/AMEsdAOhfswxymcSf2lrN1egf3NwXj9KBS2PsOiiigzKGr6FoviC1Nlrmk2moW7Agx3MKyKQevBFeT+Iv2Of2bfEztJffCrRYWbkm1gEP/oNez0UAfJs/wDwS+/ZFuLqS7bwhqytJIZSq6tKFBznAHYe1ekeGP2NP2bPCjB9P+FmkTsMEG8iE+CP96vaqKB3KelaRpWh2Uem6Np1tY2sQwkNvEI0UewHFXKKKBBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQB88f8FAP+TSviB/14D/0MV+GMX+qT/dFfuf8At/qzfsk/EDapOLAE4HQbxzX4YRf6pP8AdFBcdh1FFFBQUUUUANk/1bfQ1+2P/BNuyuLP9lrQGnTaJ5pZU91OMGvxOl/1T/7pr9xv+CfH/Jqvg7/rg386CZH0fRRRQQFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAHhv7cFrc3n7JnxOtrOB5ppNEcJGgyzfvE6V+DkWREoPUAA1/Qn+0Fp8mq/BPxpp8UiRvNpE4DN0GBn+lfz3EYkkU/wyuPyY0FxCiiigoKKKKAGy/6p/8AdNfuN/wT4/5NV8Hf9cG/nX4cycxsP9k1+3P/AATm1JNR/ZY8MokZT7IZLc57kY5/WgmR9OUUUUEBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQBieN7FNT8G65p7oHFxp1xHtIyCTG2OK/nMvIZbbUL22niaOSK6mRkYYK4kav6SrmEXFvLA3SRGQ/iMV/Pd+0Foo8OfHXx5oAUL9h1qeLA7c5/rQVE4GiiigsKKKKAEcEowHoa/aH/gmPf2V9+y7pi2lwkptr+eGUKc7HG3Kn3r8X6/XT/gkdNG37N2qWy/fi8S3jN/wILj+RoJlsfb9FFFBAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFfiR/wUe8Iw+Ef2q9faGFI/7cgj1VtoxuL8ZPvxX7b1+W3/AAV+8GW9h4v8E+PY4v32qQy6dI4HURDcB+tBUdz89aKKKCwooooAK/V3/gkNfyN8G/Eumnbsi1p5R65YV+UVfpN/wR58QxzP8QPCwikElotvdlyfkIdiMAetApbH6W0UUUGYUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFfGX/BVTwSniH9nD/hJ4rRp7vw5qEUsWxclVlIVz9MCvs2vP/j94NXx98GfF/hURLJLeaTcCAMMjzQhKfqBQCP57AQRkUU+exudLuZtLvABcWUjW8wH99Tg/qKZQahRRRQAV97f8Eg9RNt8VfG+n4OLzS4CcHj5WzzXwTX1z/wS78RrpP7UdnojK2NZ026XcGwAY0yM+uaBS2P2aooooMwooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKa6q6lHUMrDBB6EU6igD8Ev2w/hefhH+0X4v8LwwTrZXF2dRtpJBxIJ8udp7gZx7V4zX6af8Fc/g/Ld6Z4Y+NOmxyMdPY6VfRxpkbHO5ZWPtjFfmX15FBondBRRRQMK9/wD2CtYTQ/2rvBd67Kod5bfJ/wBsAV4BXcfAnWbvQPjZ4E1OynMLpr9mjsBk+W0gDD8RQD2P6G6KRWDKGU5BGRS0GQUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAHGfGP4ZaP8Yvhpr/AMOdcX/RtatHg3jrG/VWHpggV+A/xP8Ahv4k+EXj7WPh34sspba/0i4aIF0KiaPPyyIe6kY5r+iuvn39rD9jrwF+1D4fQ6g39keJ7BT/AGfrEKDev/TOT+8h/TtQNOx+F1FfRXxM/YB/ac+G+pS20XgWbxFYISVv9MIaPGeMgnOcV5fL8CPjRDI0Uvw01wOhww+zNwfyoNLo4Wt/4esyfEPws6kgjWLUgjt+8FbcXwI+NE8iwxfDPXGdzhR9mbk/lX0R+yx/wT/+N3jP4j6H4j8f+Grnwr4b0e8iv5ZbsDzLry2BEaL79DmgLo/YTRWL6PYsxJJtoiSe/wAgq7TIo0hiSGJdqIoVR6AdKfQZBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFACdeDTPIhJyYU/wC+RUlFAEfkQg5EKf8AfIqTpRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFfnv8Atpf8FBvir8BvjPN8MPAHhzRJbays4bma4v1ZnkZxnAxwBX6EV+Kn/BTX/k7fWf8AsFWf/oJoKirs7Qf8Fcf2iQAD4G8Fn3xP/wDFUv8Aw9y/aJ/6EXwV+U//AMVXxFRQVyo+3f8Ah7l+0T/0Ivgr8p//AIqtjwz/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/wCEE8FD/mVNK/8AARP8KClKx+D/AOzn8TPGfwD+L+hfEbTtA1dobaYW9/ELSXEts5w4xjk4r98dH1KLWdIsdXgRkjvraK5RXGGVXUMAR681nDwL4LBBHhXSsjkf6In+FbaIsaKiKFVQAABgAelAm7jqKKKBBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFRz3EFrE09zMkUSDLO7BVA9yaNgJKK4PWPjz8FfD9x9k1v4p+GLGb+5PqcSn8ia0fD3xX+Gfi1lTwz490LU2f7otb6OQn6YNC97YH7u51dFHWigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigBGJVSQM4Gcetfkn8Yfi545/aE/bEf4J/EXx7f+CPBlhqjWSW8Mxt9yqRgs2RnfnGTxX6214V8ev2Mvgf+0Izah4v0B7PWeMarpz+RcnHTcw+8KzS5a8KslzRW6+7X5eZqpJ0Z00+WUtn2/4cytA/YM/ZUs9OjX/hXVnrBdQWu7y4e4eU/wB7cWPX2qxD+wh+zTYa7ZeI9C8ESaPfWM6TxtYXssSkqcgFQ2CK8ktv2N/2ofhXKZvgt+09qE2nQJtttG1hDJEAOg3H8q5K5/bl/aM/Zq8V2fhT9rT4d2NxZXsm2HWNHwsfl/3h2cgckVvGcXUXLK0ul9NfXb8TFwmoO6uuttfw3P0IjRYo1jQYVAFH0FVNX1vRtAtGv9c1W00+2QZaW5mWNB+LEVjaN8Q/DfiPwCnxG0C8F5pE1i1/FIv8SBS2D6HjFfkynx5079qT9oDUNW+P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b0Plub/goP8ADG9tpB4S8EeM9fv14Fnb6VIjlvQlgBXzz44+Bn7TP7efxK03XfiZ4Ub4f+ANJf8A0W0umzPJETywH98jg1+kyWdnGd0drCp9QgFTU4qCmqkldrVX2T72/wAxOU1Fwi7X3729TF8GeE9J8C+FdL8IaHF5djpNrHawg9SqqBk+5xW1RRVTk5ycpbsiEVCKjHZBRRRUlBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAH//2Q==" alt=""></span> <span id="brandLabel">Centro de Formación</span></div>
  <div class="steps" id="steps">
    <div class="step active" data-step="login">00 · Ingreso</div>
    <div class="step" data-step="home">01 · Pilares</div>
    <div class="step" data-step="pillar">02 · Módulos</div>
    <div class="step" data-step="content">03 · Lección</div>
    <div class="step" data-step="quiz">04 · Evaluación</div>
    <div class="step" data-step="result">05 · Resultado</div>
  </div>
  <div class="user-badge no-print" id="userBadge" style="display:none;">
    <span id="userBadgeName"></span>
    <button class="link-btn" id="logoutBtn">Cambiar de usuario</button>
  </div>
</div>

<main>

  <!-- ================= LOGIN ================= -->
  <section class="screen active" id="screen-login">
    <div class="login-wrap">
      <div class="login-card">
        <p class="eyebrow">Ingreso de empleados</p>
        <h1 class="login-title">Inicia sesión con tu cédula</h1>
        <p class="login-sub">Escribe tu número de cédula para identificarte. Debes estar inscrito por tu administrador de formación para poder ingresar.</p>

        <div class="field" style="margin-top:22px;">
          <label for="loginCedula">Número de cédula</label>
          <input type="text" id="loginCedula" inputmode="numeric" placeholder="Ej: 1017123456">
        </div>
        <button class="btn btn-accent" id="loginBtn" style="margin-top:14px; width:100%;">Ingresar</button>
        <div class="error-msg" id="loginError"></div>

        <div class="login-divider"><span></span></div>
        <button class="btn-link-toggle" id="openAdminBtn">Acceso administrador de formación</button>
      </div>
    </div>
  </section>

  <!-- ================= ADMIN: PANEL COMPLETO ================= -->
  <section class="screen" id="screen-admin">
    <div class="login-wrap">
      <div class="login-card" style="max-width:600px;">
        <p class="eyebrow">Panel del administrador</p>
        <h1 class="login-title">Administración del Centro de Formación</h1>
        <p class="login-sub">Desde aquí inscribes a los empleados, activas los pilares y generas el archivo que vas a publicar para compartir con tu equipo.</p>

        <div id="adminPinGate" style="margin-top: 20px; display: none;">
          <div class="field">
            <label for="adminPinInput">PIN de administrador</label>
            <input type="password" id="adminPinInput" inputmode="numeric" placeholder="PIN (por defecto: 1234)">
          </div>
          <button class="btn btn-accent" id="adminPinBtn" style="width:100%;">Entrar al panel</button>
          <div class="error-msg" id="adminPinError"></div>
        </div>

        <div id="adminPanelBody" style="display: block; margin-top: 8px;">

          <div class="login-divider"><span>1 · empresa cliente</span></div>
          <p class="card-sub" style="font-size:12.5px; color:var(--muted); margin:-4px 0 12px;">Estos datos reemplazan cualquier marca genérica en la aplicación: aparecen en el encabezado y en cada certificado que se genere. Configúralos antes de publicar para cada empresa que tome el curso.</p>
          <div class="logo-upload" style="display:flex; align-items:center; gap:16px; margin-bottom:14px;">
            <div class="logo-preview" id="brandLogoPreview" style="width:72px; height:72px; border-radius:10px; border:1.5px dashed var(--line-light); display:flex; align-items:center; justify-content:center; overflow:hidden; background:var(--paper); flex-shrink:0;"><img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAMCAgICAgMCAgIDAwMDBAYEBAQEBAgGBgUGCQgKCgkICQkKDA8MCgsOCwkJDRENDg8QEBEQCgwSExIQEw8QEBD/2wBDAQMDAwQDBAgEBAgQCwkLEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBD/wAARCALQA8ADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD9U6KKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAoor4k/4KPftdan8F/DUHwu+HepLb+LfEERa4uUP7yxtCMb19GbkA9qASufRnxC/aY+Bfwt+0L42+I+kWMlqu6aJZfNkT2Kpk59q47w9+3p+yl4oeePSPi1pzm3UNJ5kUkeAemNyjNfhfd3F1qF3LqGpXk93dzsXlnnkLvIx6liepqMop6igvlP6I/DXxi+Fni8R/8I54/wBDvXlAKRpexh2z6KTmuwBBAIOQehr+bLT7u90m8j1HSr24s7qI5jmgkKuh9Qa+mfgL/wAFCfjt8GLuCy1rWZvF/h8SAz2movvnC/7Ep5XHpQJxP21orhfgr8YPCnx0+HemfEXwfOWstQT5o3+/DKOGRvoa7qgkKKKr6hqFjpNjPqep3cVraWsbSzTSsFSNAMkknoKALFeOfFn9rj4BfBfMPjXx/YJd8gWtq/nybvQhM7T9a+Bv2yv+Cj3iPxjqGo/DX4E6hLpWgxM1vda5EdtxdkcHyj1RffvXwXcTXF5dS317cy3NzO2+WaVyzu3cknqaClG5+q/iT/gr38I9N1GWy0D4deItWhjI23ayRpHIO+AeaoWH/BYf4ayTrHqPwl8SxRswG+OeI7R3JFflpRQVyo/arwf/AMFK/wBlnxTLDaXvjCXRbqdwiRXkDYJPqyggV9C+FfiT4B8cRLL4T8YaTqm4Bglvdo7ge65yPyr+c8qDwRWj4f8AEfiTwjeNqXhPxDqOjXbDaZ7K4aJyPqKBcp/SHRX44/A//gp18b/hvLa6V4/WLxjocKrERNhLtVH8Rl6sa/SX4A/tb/Br9omxX/hC/ECw6sq5m0q8xFcocckKfvL7iglpo9pooooEFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQBU1fVLTRNLu9Yv5RHbWUDzysTgBVBJ/lX4AftHfFi7+Nvxo8TfEGeR2t7u7eKxRusVupwqD24r9V/+ClXxhb4Zfs8X2h6fdNFqXi6UaXEYnxJHGeXcenQD8a/F5QQoBOT3PqaC4rqLRRRQUFFFFAH6mf8ABHi91Sf4a+P7K7mmaztNathZowOxA0LFtn49a/Qevjn/AIJXaGun/sw2usBSDq2oTuSe+xitfY1Bm9xCQBknAFfln/wUi/bMPinUrr4BfDLVydLsn2a9fW8mBNKP+WCsOoHfHWvo3/gob+1j/wAKK8AjwP4PulPjDxNG0UZVubO2PDy/73oK/G6SSWaWSeeRpJZXaSR2OSzE5JP4mgcV1GABRgDApaKKCwopCcdiSTgADJJ9BXoPiz4BfFvwN4C0r4meKfB95Y+H9Ybbb3EiEFeMguP4Qe1AHn9FFFABWh4d8Q674R1u28SeF9VuNM1OzcSQ3Nu5VlIORnHUexrPooA/ZD9g39tiL9oLRj4E+IFxb2/jvTItx28LfwDjzR/teor7Dr+dH4a/EHxB8KvHmifEDwxdtb3+j3cc6kHCugPzK3quM8V/QR8M/HGl/ErwBoPjvRp0mtNaso7pHQ5GSPmA+jAigiSsdNRRRQSFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFc78Q/F9p4B8Da74zvSPK0awmvCD/EUQkD8SAKAPyR/4Kf/ABe/4T/4+r4KsZXNh4Nthb5DZjllk+ZiMdweK+PK1fF3iW58Z+LNZ8XXcskkms3017mQ5ZVdiwX8AayqDVaIKKKKACmTtshd/QZp9X/Dujr4i8R6T4ekDFdUvobNgv3iHYDj3oA/dr9jTwlF4L/Zt8E6PFbCAPp63ZUesvz5/HNdr8Y/ip4e+DHw61n4h+JbhI7bS7dnRGODNLj5Ix7k4Fa/gXRYfDPgjQdAiUxx6ZpltagMeQEiVefyr8of+CmX7TD/ABP+Ig+EXhfUWPh3wpKwvGif5Lq86EHH3lUYx70GaV2fK/xa+KXib4z/ABC1f4jeK7uWa81WcvHG7ZFvDn5I1HQADjiuQoooNApCcYABJYgKqjJYnoAO59qCcDNfop/wTu/YbXXJrP47/F/Rw9khEugaXOvDsDxPIp6j0HrQDdjR/YE/YBMn2D43fHHR+fluNE0O4T7o6rPMD39F/Ove/wDgp1BBF+yLr0ccKIsV1aBFVQAo39AO1fWaqqKERQqqMAAYAFfJ/wDwU9/5NI8Rf9fdp/6HQZ3uz8XaKKKDQKKKKAEYblK+oxX7H/8ABLXx+/i/9m6PQZiQ3ha/k01FJH+rwGBHtkmvxxr9FP8Agj54uuR4k8eeBpBi2W0h1CLnrIXw36UClsfp/RRRQZhRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABXxp/wVL+KCeCf2fF8I2moNbap4uvVtrfYfmaOPDSD6EGvsuvyJ/4KvfEaXxJ8b9K8AwSK9l4csBMSD924kJDD8sUDW58QgBQFAwB0paKKDQKKKKACvU/2WvB48c/tC+BtBZpFVNVhvD5fUiJg2PpXllfUX/BNfQZNU/ar0XV5RGthomn3l1dSOwAjxH8p57ZFAPY/Sr9uH9oe2/Z9+C2oahYXKDxFranT9Ji3DcHcEGTHXCjv71+Gs0891PLd3UrSz3EjSyuzElnY5JJPua+iv27P2hn/AGgPjbeS6ZM58PeGWfTdNQ9GKnEknuGYZBr5zoFFWQUUV1fws+GniP4v+PtH+Hnha3eW91a4WNnUZ8mLPzyH2Uc0DPf/ANgf9k2f9oXx+ninxTZyjwV4clWW5bGFvZwcrCD3Hc49K/aKxsbPTLKDTtPto7e2to1ihijXCogGAAPTFcb8FfhJ4b+CPw40f4d+F7dEttNhAlkVcGeYj55D9Tk13NBm3cK+Tf8Agp/Ii/sleIEZwGe8tQoJ6/PX1lXxh/wVYv7a2/ZtFlKW8271GNYgBwSuCc0Atz8e6KKKDQKKKKACvs3/AIJT6s1h+0Re2AIxqGluhy2Pugnp3r4yr6U/4JxySJ+2H4NRJGVXtr8MAeG/cHrQJ7H7f0UUUGYUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQBBe3UdjZz3sxAjt4mlYnsFBJ/lX8+Xx/8AHn/CzvjX4y8cx3bXEGp6rM9ux7Rg7QB6Div25/ax+IDfDL9nnxv4ugw1zbaXIlum7G+R/lxn6E1+AwYyFpSMGVmkP1Ykn+dBcULRRRQUFFFFABXXfD/4oeJvhnDrg8Kutvda7ZmxkuwxEkMJ4cL/ALwOK5GigBAMDGSfcnJNLRRQAjHaCx7V+r3/AAS2/ZvTwd4Im+OHiayA1fxKuzTBImDDZj+IZ5Bbp9BX5+fss/Ay/wD2hPjLo3gSFXXT45FvdUmXjyrZGBJz6kgCv3s0bSbHQdJs9F0yBIbSxhSCGNBgKqjA4oJk+hdooooICvz2/wCCwuv3dp8PPAegWtwUiv8AV53uo8DEiLENo/Ov0Jr8rv8Agr34wt7z4geDvAiysZrGxbUWTbwA7Fc59eOlA1ufn7RRRQaBRRRQAV9Kf8E40kb9sTwYyRuyrbX+4hSQv7g9T2r5rr7O/wCCU+lS337Q99fI2FsNLZ3G3Od2R+FAnsfsLRRRQZhRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAHw5/wVl8bXOg/AvSvC9jPsk1zVo0nX+9AoOR+ZFfkeAAMDtX3h/wAFcfF8uq/Fvwr4TgvG+z6RpkjzQBvlMjsCGI9cV8H0GkdgooooGFFFFABRRRQAUjMEUsxwByaWvVf2X/g5qfx0+NvhzwNZwk2n2lbzUZDHujW3jIZ1b03DIFAH6Wf8Exf2fj8M/hG/xF1+xMeveMGE6iRfmhtR9wA+jcNX2lVXS9MstF0210jTYFgtLKFLeCNRgIigBQPwFWqDJ6hRRRQAV+KP/BSvxjZ+Lf2p9XtbS4Ep8PWselzD+464bb+tftVcTLb28tw5wsSM5PsBmv57/wBoLxZD47+OXjfxhbyLJHqerzOrL0O07f6UFR3OAooooLCiiigAr9DP+CPnhm4fxn488XSBTbjT4LOLjkSCTLfpX55k4GTX61/8EkfC9zpXwL1zX7yDY2q63IYDj70SqMH8z+lApbH3RRRRQZhRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFUtb1KPRtHvtWlxssreSdsnjCqT/SgD8M/wBu3xRH4u/aq8a6pBdefBFJFaR4fcq+Uu0genSvBa3PHl+NV8feKNVVsi91m7uAc54aUnr+NYdBqtgooooAKKKKACiiigBGIVSx6AZr9X/+CUvwLPhL4daj8YtasTHqXip/JsmbvZIcqw+p/lX5k/C3wDqnxS+I3h74faOD9p1q/itw23cFXcCxI9MA1/Qd4G8I6X4D8H6P4N0W3WCy0i0jtYUXoAo5/M5NBMn0N2iiiggKKKKAOC+PXjCLwB8GvGPjCaURrpmkzy7vTK4/rX89csouLie6HS4mkm/76Yt/Wv2W/wCCn3xBfwV+zReaVbx+ZL4lvotMZd2MRtks34YFfjMi7EVR2AFBcRaKKKCgooooAa4JUqOrfKPqeBX7ufsN+D7jwV+y94F02+t/JvJ9PFzcJjkO7H+mK/D/AME+Gb3xp4z0LwjpxAutW1CG3iJGed4P8ga/ol8LaRFoHhrStEhjCJY2cNuFAwBtQA/qKCZGpRRRQQFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAV5Z+1Fr48N/s/8AjrUvMaNjotzAjKcEM6Ff616nXyZ/wU91+50T9lLWoLG7kt7i/vbWAMjYJTflh9CKAR+LVtu+zx72LMVGSTkk+tS0AADAGAKKDUKKKKACiiigAoopCJWwlvE0srnbHGgyzsegA7mgD7+/4JNfBhte8c658ZtUgY2mhxDT7EOnytO/zeYp9QMiv1Wrw39i74SwfBz9njwr4aEbLdXVquo3RkXD+ZMN+1voDivcqDNu7CiiigQUUUhIAyTgCgD8uf8Agr14+lu/Fvg74dWl0Db2ttJe3kQPSQkeWT+FfnnXt37anxHi+KP7S/jHxDbTO9taXI0uINwB5GUOB+FeI0GiVkFFFFAwooooA+lf+CdngC38fftTeHTdws8Xh2Nta6HaGj4Gfz6V+31fnV/wSG+G72nhfxZ8UL2BT/aVylnYyFeQij94AfqBX6K0GctwooooEFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAV+e//BX/AMWTad8PvBPhGFFZNY1Gd5yWIKLGgKkDvk5r9CK/Kv8A4K8+JYrz4ieD/CazAyafZNeNHnkByQD+lA1ufAFFFFBoFFFFABRRRQAV7J+x/wDDB/i5+0T4Q8LNG7W0F2NRuWAyAkGHIPscV43X6U/8Eh/hYfJ8V/GC9iysrjSrIsv3WTmQg+4IFAnoj9KI40hjSGJQqIoVVHQAdBTqKKDMKKKKACuA+Pfj21+Gnwf8V+Mrq4WE2Omz+SzNgecyFU/8eIrv6+D/APgrT8UF8P8Awf0j4Z2w3zeKr7dcYfBiii+ZSR3BbIoGtT8or7UbvWb+61m/bN1fzPczH1djk1DRRQaBRRRQAU6O3ubuWOzsoy9xcOIoUHVnbgD86bXuP7Fvwkl+Mf7RPhjQJbd307Tpxqd7IoyI1i+dQ3sSMUBsfsL+yf8ADC2+EfwD8JeEYrYQTCxS7ulxyJ5QHfP4nFeu01ESNFjjUKqgBQOgAp1BkFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFfi/wD8FQdXTV/2qboIwP2DSILQ47FSTj9a/aCvwW/bT8RXHiX9qb4iXEzK0dpq8lpblRj92oGM+9BUdzxWiiigsKKKKACiiigBCryYij+/IQif7xOB+pr95P2Lfhwfhh+zh4O0G5tVt7+4slvb5QMZnk5J/LFfiz8A/Aq/Ez41+DPAkscjRatqsMcmwchVO7PsPlr+g+ytYrGzgsoVCx28SxIB2CgAfyoJkT0UUUEBRRRQAdK/En/goz8U4/iX+0zrFnZTStZeFIxo8Y3Zjd1O5nUdOc4zX67/AB6+I9n8JfhB4p8fXbKP7K0+WSNScF5CMKB75P6V/Pnqep3et6nea1f3Ek9xf3ElxJJIcsS7E8n8aCoor0UUUFhRRRQAhIAJPQc1+qv/AASb+CjeG/Aes/GTVrMx3viZ/slk56NZochh9TX5m/DrwLrHxN8eaF4A0GIve65ex2qfLkKCfmJ9sA1/QX8M/Amj/DLwDoXgLQLZbex0SyjtYkXoMD5j+JJNBMmdNRRRQQFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUARXUnk20sxONiM35Cv57Pj1qQ1n43eONVVmYXWszPlup5x/Sv6BfE8/2bw1q1z5mzyrGd9393EbHNfzkarfXmp6xqOoahcNPc3F5O8krdXPmNyaColaiiigsKKKKACiiigD7W/4JS/D+XxH8edR8Z3Nqklh4f01gjsMlLliNuPwJr9fa+Dv+CSHgIaL8Htf8dSqS/iPUl8pj2SJSpA/HFfeNBnLcKKKKBBRRVbUtQs9I0+51XUJ1htbOF55pGOAiKCWJ/AUAfnn/wAFbvjEun+HfDvwY0y6YXGqS/2lfeW33Y04VH+uc1+YIGBgV6p+1D8W7v42/HPxP46mk3Wz3Js7IBtyfZ4sqjL9RXldBolZBRRRQMKKK6D4feBdc+J3jfRvh/4cgaXUNauUt4wvVVJ+Z/8AgI5oA+8v+CT/AMAX1PWNU+PmvWZ+z2YNho29eJHP35B7rjH41+oNcX8HPhlo3we+G2hfD3Q4Y0g0m1SORkGBLNj94/4tk12lBm3cKKKKBBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAHL/ABRvf7O+HHia98vf5WlXJ2+uYyP61/OtKc3Fw3rcSn/x81/QZ+0Rez6d8D/Gt7bMBLFpE5Un3GP61/PiTl5Cepkcn/vo0FxCiiigoKKKKACmTP5UTSf3Rmn1q+EdGXxH4v0Hw68YddV1KCzKnowdwMUAfuX+xN4Fg+Hv7M/gvQoIygls/tzZ6kzHfn9a9zrJ8I6Onh3wro2gRxhF02wt7QKOgEcarj9K1qDIKKKKACvkT/gpT8eH+EvwPfwto9yE1vxmz6fDg5KQYzISPQgkZr60vr600yyn1G+nSG3to2llkc4CqoySTX4T/tm/Hq7+P3xw1fXoLxpdB0qRrDR0z8ohU8tj1JzzQNK7PCY0WNFjQYVRgCnUUUGgUUUUAISACT0Ffpv/AMErf2aZNOsrr9oTxZZfvdQQ22gxSx8xx/xTqTz8w4r4j/Zd+AWsftGfFzS/AtnHPHpcci3Wr3cY4gtlOTz03HgY96/ebwz4c0nwj4f0/wAMaDaR2un6ZbpbW8SDAVFGOn60EyfQ06KKKCAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA8U/bS1e/0H9lf4latpkix3VvojmNmXIBLqDx9Ca/BWMlkDnqw3H6nk1+7X7d9xFB+yP8TBK20y6OY092MiYH6V+EkX+qT/dH8qC47D6KKKCgooooAK9i/Y+8HW3jr9pTwNoV3C0kcWoLf7VODmEhgfpXjtfW/wDwS98KHXf2orLXW5j0LTrmRlxwWdMKfwNAnsfs5RVHV9d0Tw/afb9f1ix022zt868uEhjz6bnIGar6T4t8Ka9j+wvE+k6ju6fZL2ObP/fLGgzNaiivHP2ov2jvC/7N3w3u/Fer3EMmqzo0WlWJYb7ifHBx12g8mgD5w/4Kd/tSJ4E8Hj4HeD9QI17xJFnUpYW5tbTuhI+6zcY9q/J1RtAGc+/rW/478c+JfiV4v1Txz4v1CS81TVp2nld2yEBPCL6KOgrBoNErBRRRQMKtaXpepa5qdpomjWj3V/fTLBbwoMs7scAcVV5yAoJLEAAdST0FfqR/wTn/AGJj4Tt7T47/ABT0of2zcx79EsZ1z9liYf61lPRiOlAm7H0B+xF+zFZfs3/CqC01GJZfFOthbvVrgrhlYj5Yh6BQcfWvouiigzCiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA+eP+CgH/JpXxA/68B/6GK/DGL/VJ/uiv3O/4KAf8mlfED/rwH/oYr8MYv8AVJ/uiguOw6iiigoK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RRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFfnv8Atpf8FBvir8BvjPN8MPAHhzRJbays4bma4v1ZnkZxnAxwBX6EV+Kn/BTX/k7fWf8AsFWf/oJoKirs7Qf8Fcf2iQAD4G8Fn3xP/wDFUv8Aw9y/aJ/6EXwV+U//AMVXxFRQVyo+3f8Ah7l+0T/0Ivgr8p//AIqtjwz/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/wCEE8FD/mVNK/8AARP8KClKx+D/AOzn8TPGfwD+L+hfEbTtA1dobaYW9/ELSXEts5w4xjk4r98dH1KLWdIsdXgRkjvraK5RXGGVXUMAR681nDwL4LBBHhXSsjkf6In+FbaIsaKiKFVQAABgAelAm7jqKKKBBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFRz3EFrE09zMkUSDLO7BVA9yaNgJKK4PWPjz8FfD9x9k1v4p+GLGb+5PqcSn8ia0fD3xX+Gfi1lTwz490LU2f7otb6OQn6YNC97YH7u51dFHWigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigBGJVSQM4Gcetfkn8Yfi545/aE/bEf4J/EXx7f+CPBlhqjWSW8Mxt9yqRgs2RnfnGTxX6214V8ev2Mvgf+0Izah4v0B7PWeMarpz+RcnHTcw+8KzS5a8KslzRW6+7X5eZqpJ0Z00+WUtn2/4cytA/YM/ZUs9OjX/hXVnrBdQWu7y4e4eU/wB7cWPX2qxD+wh+zTYa7ZeI9C8ESaPfWM6TxtYXssSkqcgFQ2CK8ktv2N/2ofhXKZvgt+09qE2nQJtttG1hDJEAOg3H8q5K5/bl/aM/Zq8V2fhT9rT4d2NxZXsm2HWNHwsfl/3h2cgckVvGcXUXLK0ul9NfXb8TFwmoO6uuttfw3P0IjRYo1jQYVAFH0FVNX1vRtAtGv9c1W00+2QZaW5mWNB+LEVjaN8Q/DfiPwCnxG0C8F5pE1i1/FIv8SBS2D6HjFfkynx5079qT9oDUNW+PWreKn+HukTO1l4e0K2knV9jYQSCPkZI5Pes/edf6vs0m3fol+r6IuCi6Ht1rHRK3Vva3l3fQ/SrW/wBr39nDw9OLfU/inpisW2AxRyzLn/eRCK6zwd8avhR4/k8jwh490fUZv+eMdwFk/wC+Gwf0r5t0D9oz9jfwxpqaRoXwh8RWtpGNojXwdKR+Zya+cf2tNV+BHjjR7fxn+zr4I8b+HfiJp1yklvLZaFPZxzKT8xc9MjtRKSg1dNq/Tf1t+eoRg6miaT89vv8A+AfqtVDWNd0Xw9ZtqGu6taafbIMmW5mWNfzY14P+yD8XvHHjb9nS28W/FPS7y11zR4JUu/tURjkmEakhyD3IHJr4W8A6j4x/4KIftPX+k+O/FF9aeBtHlknXSLaYxp5MbYVcD+IkHJrSdKf1r6rCzdrt9FHe/wA1sjOE4/V3iamiva3Vyva339T9BdV/bQ/Zg0a//sy++L+jfaN23bEJZQDnHVFIruPDvxl+Fni3TLnV/DnjrSb+2soWuLgxTjfHGoyWKH5sAD0rH8K/s1/ArwXpqaX4f+GOhQRKoUs1qru+O7M3JNeG/tdfss/DSy+FviT4jfD6ybwb4k0uxlmN5pDGEXMePnjlUcMCOK569VUKbm9bdf8Agf8ABNqNN1qijtf+t/8AgHvfww/aA+Dvxnub+0+GHjqw8QS6Wdt2tsH/AHR9DuUV0/jPxr4X+Hvh278W+MtYh0vSLFd1xdTZ2Rj1OATX52f8EdW8228ezFRukmgZjjkkrX1h+3YAf2X/ABkCMj7Ov/oVaZjfBUeeOr5U/mxYJLFYh0ntzW87afieh/Cr45fCj43WN7qXwr8a2PiK20+RYrmS1D4idhkA7gO1d3X53/8ABHVVXwB462qB/wATO36D/pma/RCurFUY0JqMesYv74p/qc9Ko6l79G0eW/EH9qD4C/CrxPD4N+IPxJ0zRdZuAhjtLgSb23HC/dUjnNenW9xDdW8d1byB4pUEiMOhUjINfkL/AMFMEU/tZ6IWUH5LLqP9pa/Wvw1/yLmmf9ecP/oArnw69tgliXu5yj5Wjax0YmKo4hUY7cqf3pP9Th/Df7SPwR8X+Pbv4YeHfiFp174osS4uNNQOJY9hw2cqBx9ag8b/ALUP7P3w51BdK8Z/FfQNNvHkEIha43tvJwFwgODmvyp12x8Uaz+3trPhPwdrr6He+JNYfTZL6H5ZIoXY7ipHQ4BFfph4N/Yi/Zu8J6db2918N9O16+iIkk1HVk+03EsvUuWbvnmlQTq4aliZaKS18+9uy9eoYlRo4iph46uO36X+fRdD3CxvrTU7KDUrGdZra6iWaKRejowyCPqDXIeMPjb8JfARK+LviDounOODHJdKzg+m1cn9K+TP+Ck37Sviz4I+GdA+FfwwuTo9/wCIYtpvIfla3tlIXZH6Hkc10X7Jf7Enww0jwHpXxD+JumL4x8Xa/Ct/c3WpuZkiZ+QEUnGfeimnXU6sNIRdrvdvsl8nd+RE/wBwoQqazkr2W1u9/ntvqetWH7av7L2pXp0+1+L+k+cuQRJHNGo/4EyAfrXqvhvxj4U8YWi33hbxFp+qwMNwe1uFk49wDkfjXM6v8Afgtr2nvperfDLw/cWsgw0bWaj9RzX5uftffDzWf2EPifoXxO+AviS/0nRtemYy6T9oZovMT5mTB/gI7UlUhGcYVNOZ2v5+aLVOU4ylT3Wtu/oz9YqK4v4NePj8UPhh4d8dvb+RLq9jFPLHjhZCo3Ae2c12laVacqU3TlutDGnUVWCnHZhRRRUFhRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAyZ2iheRIzIyKWCDqxA6CvlPXv25Nc8C6zf6d49/Zz8d2lrb3DRw3dnbCdHiB4cgV9X0x4opOJI1b6jNTaXNdPTsUnG1mj5H/4eV/CSdTFpfgDx9fXZ4S2j0WQO59ASMV4N8fdA/aO/b+8RaBoWifCO88F+C9KmaZdS1gBZGLjDFh1HA4Ar9LRY2SnctpAD6iMVMAFGAAB7U+SEpKU1e2tun9fMI1JwT9m7XVr9bPf+rHB/Cf4S6P8ADD4TaV8KoJWurOxsTaSu/wDy0LD5z+JJr4Ruf2Y/j5+xt8ar74q/A3wpD458H6nI5u9JAHnxwsckEH0ycEV+ldFVOc5V/rKfvu9/NPdNEU4whQ+rW9zTTs1s15nyLYft9fCu0jEPjz4TeLfDF6ow0VxopkUt32lAeK1F/be+FuqWyTeD/hX4t8QvI4RYrXRdjZ/4GBX1A9naSnMlrC5/2kBpY7W2i/1VvEn+6gFCabu1939Me2xm6aLLxD4ZieTSms4NTtAZbWRArRh15RgO4zg1+bevfsw/Hz9jb47y/Gb4EeHG8XeFrmaRp9OibEkcMh+ZHHfHOCK/TuvD/jP8ZvjJ8NvFEFt4U+BF54x8OyQq017Z3qpKj9xsIOcVHN7Ouq1N8stV3Vn0fl/XUuKc6MqM9Y6N9NV1Xmee+HP+CiXw5vnTS/FXw+8aeH9Z4R7OfS5GBfvtYDBFcd+0p8cPi98Yfg34q034afC3VPD3h6GzeTUdd15BEssAGSsCA5JI9a7OT9ti5Sf7Ncfsw/EP7YDjA0osm7/f24/GvO/jLr/7Y/7U3h9/hv4E+Dx8BeG9RYR6hf6reKJnh9hgYHqKjEU3iKbhGN2/lH1fl5XLw840ailJ2S+b+Xn8jh/+COaE2HjyWNGEXnQAH/gPSvvP42/DeL4t/C7xB8P5JxC2rWjxRSHokmPlJ9s4riP2Sv2YtE/Zf+HP/CKWV6NQ1S+cXGpXoXaJZAMAAdgBxXuFdeYKnif3W65Uvw1/HY5cHKdGTqrR811+n5H5Rfs56/8AHD/gnx4n8Q6B8SvhJreseEdRkV5L3S4TMzMnyrJGBnIx619Y6b+374f8X2ij4cfBrx/4hv5Tsjt104w4fsGL4wK+qXiilGJY1cejDNJHbW8PMMEaf7qgVDqTqRSqu7SSvs7LuaOMIycqatd3tuv6+Z+M/wC2v4b+OV98bvC/j/4p+Gjb3HiF4JLTTtNt5J/7PgjkUBJWUEbsda/Ynwyc+G9LIB5s4eowfuCr8lvBMQZYI3I6FlBxTwABgCinJU8MsMlopSl99tPw36hVbq1VWk9bW+7+tj8fdD0nWR/wUts7s6HqYtv+En3eebOTysfNzvxtx75r9g6i+zWwk80W8W/ru2DP51LSpv2eEpYX+RNX73HWftsTPEbc3Ttv/mfMX7cH7IKftP8AhKzudAv4dP8AFehbm0+eb/VyKeTG2OmSOteR/BH9oz48/s3+Gbb4ZftEfBPxHeWOir9mstb0uLzw8IPDMB2/WvvmmvHHIMSIrD0IzUUuajzRg/dk7tPa/ddn/mx1GqyjzrWOifW3b0Plub/goP8ADG9tpB4S8EeM9fv14Fnb6VIjlvQlgBXzz44+Bn7TP7efxK03XfiZ4Ub4f+ANJf8A0W0umzPJETywH98jg1+kyWdnGd0drCp9QgFTU4qCmqkldrVX2T72/wAxOU1Fwi7X3729TF8GeE9J8C+FdL8IaHF5djpNrHawg9SqqBk+5xW1RRVTk5ycpbsiEVCKjHZBRRRUlBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAH//2Q==" alt="" style="width:100%;height:100%;object-fit:contain;"></div>
            <div>
              <label class="upload-btn" for="brandLogoInput" style="display:inline-block; font-family:var(--body); font-weight:600; font-size:13.5px; padding:10px 16px; border-radius:8px; border:1px solid var(--line-light); background:#fff; color:var(--ink); cursor:pointer;">Subir logo (PNG/JPG)</label>
              <input type="file" id="brandLogoInput" accept="image/*" style="display:none;">
            </div>
          </div>
          <div class="field"><label>Nombre de la empresa</label><input type="text" id="brandName" placeholder="Ej: JM Estrada S.A.S."></div>
          <div class="field"><label>NIT</label><input type="text" id="brandNit" placeholder="Ej: 900.123.456-7"></div>
          <div class="hint-msg" id="brandHint"></div>

          <div class="login-divider"><span>2 · matrícula de empleados</span></div>
          <p class="card-sub" style="font-size:12.5px; color:var(--muted); margin:-4px 0 12px;">Sube el Excel o CSV con tus empleados (columnas: Cédula, Nombres y Apellidos, Cargo, Área, Sede, Correo).</p>
          <label class="upload-label" for="rosterFile">
            Cargar matrícula de empleados (.csv o .xlsx)
            <input type="file" id="rosterFile" accept=".csv,.xlsx,.xls" style="display:none;">
          </label>
          <div class="hint-msg" id="rosterHint" style="color: var(--accent-dim);">Matrícula cargada: 7 empleados. Recuerda generar el archivo para publicar para que quede incluida.</div>
          <div id="rosterCurrentCount" style="font-family:var(--mono); font-size:11.5px; color:var(--muted); margin-top:8px;">Matrícula actual en esta sesión: 7 empleado(s). Recuerda generar el archivo para publicar después de cualquier cambio.</div>

          <button class="btn-link-toggle" id="toggleManualAdd" style="margin-top:12px;">+ Agregar un empleado manualmente</button>
          <div id="manualAddBox" style="display:none; margin-top:10px;">
            <div class="field"><label>Nombre completo</label><input type="text" id="manualNombre" placeholder="Nombres y apellidos"></div>
            <div class="field"><label>Número de cédula</label><input type="text" id="manualCedula" inputmode="numeric" placeholder="Ej: 1017123456"></div>
            <div class="field"><label>Cargo</label><input type="text" id="manualCargo" placeholder="Ej: Auxiliar administrativo"></div>
            <button class="btn btn-outline-dark" id="manualAddBtn" style="width:100%; margin-top:6px;">Agregar a la matrícula</button>
          </div>

          <div class="login-divider"><span>3 · pilares disponibles</span></div>
          <p class="card-sub" style="font-size:12.5px; color:var(--muted); margin:-4px 0 12px;">Activa cada pilar cuando quieras habilitarlo. Dentro de un pilar activo, los módulos se desbloquean solos, uno a uno, a medida que el empleado aprueba la evaluación anterior.</p>
          <div id="courseLockList"><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M32 6l20 8v14c0 14-9 24-20 30-11-6-20-16-20-30V14l20-8Z"></path><path d="M23 32l6 6 12-14"></path></svg></span>Copasst <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(19 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="copasst" aria-label="Alternar disponibilidad de Copasst"></button>
      </div>
    </div><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M8 14h30v20H24l-8 8v-8H8z"></path><path d="M34 24h22v16h-6v8l-8-8h-8z"></path></svg></span>Comité de Convivencia Laboral <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(12 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="convivencia" aria-label="Alternar disponibilidad de Comité de Convivencia Laboral"></button>
      </div>
    </div><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M10 40c0-14 9-26 22-26s22 12 22 26"></path><path d="M8 40h48"></path><path d="M8 40v4a4 4 0 0 0 4 4h40a4 4 0 0 0 4-4v-4"></path><path d="M32 14V8"></path><path d="M22 40c0-8 4-14 10-14s10 6 10 14"></path></svg></span>Seguridad y Salud en el Trabajo <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(12 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="sst" aria-label="Alternar disponibilidad de Seguridad y Salud en el Trabajo"></button>
      </div>
    </div><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M32 8c4 8-4 10-4 18 0 5 3 8 4 8s4-3 4-8"></path><path d="M22 30c-4 5-6 10-6 16a16 16 0 0 0 32 0c0-8-4-13-8-18-1 6-4 9-6 9-3 0-4-4-3-9-4 0-7 1-9 2Z"></path></svg></span>Brigada de Emergencia <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(12 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="brigada" aria-label="Alternar disponibilidad de Brigada de Emergencia"></button>
      </div>
    </div><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 50C10 34 18 16 40 12c8 16 2 34-12 40-6 2.4-10.4 1.6-14-2Z"></path><path d="M14 50 40 14"></path></svg></span>Gestión Ambiental <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(12 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="ambiental" aria-label="Alternar disponibilidad de Gestión Ambiental"></button>
      </div>
    </div><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="32" cy="32" r="22"></circle><circle cx="32" cy="32" r="6"></circle><path d="M32 10v10M32 44v10M10 32h10M44 32h10M17 17l7 7M40 40l7 7M47 17l-7 7M24 40l-7 7"></path></svg></span>Plan Estratégico de Seguridad Vial <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(12 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="pesv" aria-label="Alternar disponibilidad de Plan Estratégico de Seguridad Vial"></button>
      </div>
    </div><div class="lock-row">
      <div class="lock-row-name"><span class="icon-sm"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="32" cy="32" r="22"></circle><path d="M22 33l7 7 14-15"></path></svg></span>Gestión de Calidad <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(12 módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">Habilitado</span>
        <button class="toggle on" data-key="calidad" aria-label="Alternar disponibilidad de Gestión de Calidad"></button>
      </div>
    </div></div>

          <div class="login-divider"><span>4 · publicar</span></div>
          <p class="card-sub" style="font-size:12.5px; color:var(--muted); margin:-4px 0 12px;">Genera el archivo final con la marca de la empresa y la matrícula ya incluidas. Sube ese archivo a tu servicio de hosting (o intranet) y comparte esa URL — cualquiera que la abra podrá ingresar solo con su cédula, y sus certificados saldrán con el logo, nombre y NIT de esta empresa.</p>
          <button class="btn btn-accent" id="generatePublishBtn" style="width:100%;">Generar archivo listo para publicar →</button>
          <div class="hint-msg" id="publishHint"></div>

          <div class="login-divider"><span>seguridad</span></div>
          <div class="field">
            <label for="newPinInput">Cambiar PIN de administrador</label>
            <input type="password" id="newPinInput" inputmode="numeric" placeholder="Nuevo PIN">
          </div>
          <button class="btn btn-outline-dark" id="savePinBtn" style="width:100%;">Guardar nuevo PIN</button>
          <div class="hint-msg" id="pinSavedHint"></div>
        </div>

        <div class="login-divider"><span></span></div>
        <button class="btn-link-toggle" id="backToLoginFromAdmin">← Volver al ingreso</button>
      </div>
    </div>
  </section>


  <!-- ================= HOME ================= -->
  <section class="screen" id="screen-home">
    <div class="hero">
      <p class="eyebrow">Centro de estudio · Copasst · Convivencia · SST · Brigada · Ambiental · PESV · Calidad</p>
      <h1>Escribe el tema que necesitas aprender</h1>
      <p>Escribe una palabra o frase relacionada con el pilar que buscas (por ejemplo "brigada", "seguridad vial" o "residuos"), o elige uno directamente abajo para ver su camino de módulos.</p>
      <div class="search-row">
        <input type="text" id="searchInput" placeholder="Ej: comité de convivencia, extintores, PHVA..." aria-label="Buscar pilar de formación">
        <button class="btn btn-accent" id="searchBtn">Buscar</button>
      </div>
      <div class="hint-msg" id="searchHint"></div>
    </div>

    <p class="section-label">Pilares de formación disponibles</p>
    <div class="topics-grid" id="topicsGrid"><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M32 6l20 8v14c0 14-9 24-20 30-11-6-20-16-20-30V14l20-8Z"></path><path d="M23 32l6 6 12-14"></path></svg></div>
      <div class="name">Copasst</div>
      <div class="desc">Comité Paritario de Seguridad y Salud en el Trabajo · 19 módulos</div>
      
    </button><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M8 14h30v20H24l-8 8v-8H8z"></path><path d="M34 24h22v16h-6v8l-8-8h-8z"></path></svg></div>
      <div class="name">Comité de Convivencia Laboral</div>
      <div class="desc">Prevención del acoso laboral y resolución de conflictos · 12 módulos</div>
      
    </button><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M10 40c0-14 9-26 22-26s22 12 22 26"></path><path d="M8 40h48"></path><path d="M8 40v4a4 4 0 0 0 4 4h40a4 4 0 0 0 4-4v-4"></path><path d="M32 14V8"></path><path d="M22 40c0-8 4-14 10-14s10 6 10 14"></path></svg></div>
      <div class="name">Seguridad y Salud en el Trabajo</div>
      <div class="desc">SG-SST, riesgos laborales y prevención · 12 módulos</div>
      
    </button><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M32 8c4 8-4 10-4 18 0 5 3 8 4 8s4-3 4-8"></path><path d="M22 30c-4 5-6 10-6 16a16 16 0 0 0 32 0c0-8-4-13-8-18-1 6-4 9-6 9-3 0-4-4-3-9-4 0-7 1-9 2Z"></path></svg></div>
      <div class="name">Brigada de Emergencia</div>
      <div class="desc">Respuesta ante emergencias y primeros auxilios · 12 módulos</div>
      
    </button><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 50C10 34 18 16 40 12c8 16 2 34-12 40-6 2.4-10.4 1.6-14-2Z"></path><path d="M14 50 40 14"></path></svg></div>
      <div class="name">Gestión Ambiental</div>
      <div class="desc">Cuidado ambiental, residuos y buenas prácticas · 12 módulos</div>
      
    </button><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="32" cy="32" r="22"></circle><circle cx="32" cy="32" r="6"></circle><path d="M32 10v10M32 44v10M10 32h10M44 32h10M17 17l7 7M40 40l7 7M47 17l-7 7M24 40l-7 7"></path></svg></div>
      <div class="name">Plan Estratégico de Seguridad Vial</div>
      <div class="desc">Prevención vial y conducción segura · 12 módulos</div>
      
    </button><button class="topic-tile" style="position: relative;">
      
      <div class="icon"><svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="32" cy="32" r="22"></circle><path d="M22 33l7 7 14-15"></path></svg></div>
      <div class="name">Gestión de Calidad</div>
      <div class="desc">SGC, no conformidades y mejora continua · 12 módulos</div>
      
    </button></div>
  </section>

  <!-- ================= PILAR: CAMINO DE MÓDULOS ================= -->
  <section class="screen" id="screen-pillar">
    <div class="content-header">
      <div>
        <span class="tag" id="pillarTag">Pilar</span>
        <h2 id="pillarTitle">Nombre del pilar</h2>
      </div>
    </div>
    <div class="pillar-progress-wrap">
      <div class="pillar-progress-bar"><div class="pillar-progress-fill" id="pillarProgressFill"></div></div>
      <div class="pillar-progress-label" id="pillarProgressLabel">0 de 0 módulos completados</div>
    </div>

    <div id="moduleList" class="module-list"></div>

    <div class="continue-row">
      <button class="btn btn-ghost" id="backHomeFromPillar">← Volver a los pilares</button>
    </div>
  </section>

  <!-- ================= MÓDULO: LECCIÓN ANIMADA ================= -->
  <section class="screen" id="screen-module">
    <div class="content-header">
      <div>
        <span class="tag" id="moduleTag">Pilar · Módulo 1 de 12</span>
        <h2 id="moduleTitle">Título del módulo</h2>
      </div>
      <button class="listen-btn no-print" id="listenBtn">
        <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 5 6 9H2v6h4l5 4V5Z"></path><path d="M19 5a11 11 0 0 1 0 14M15.5 8.5a6 6 0 0 1 0 7"></path></svg>
        <span id="listenLabel">Escuchar</span>
      </button>
    </div>

    <div class="deck" id="deck">
      <div class="deck-slide" id="deckSlide"></div>
      <div class="deck-controls">
        <div class="deck-dots" id="deckDots"></div>
        <div class="deck-nav-btns">
          <button class="btn-small" id="prevSlideBtn">← Anterior</button>
          <button class="btn-small" id="nextSlideBtn">Siguiente →</button>
        </div>
      </div>
    </div>

    <div class="continue-row">
      <button class="btn btn-ghost" id="backToPillarFromModule">← Volver al pilar</button>
      <button class="btn btn-accent" id="goToQuiz" disabled="">Continuar a la evaluación →</button>
    </div>
  </section>

  <!-- ================= QUIZ DEL MÓDULO ================= -->
  <section class="screen" id="screen-quiz">
    <div class="content-header">
      <div>
        <span class="tag" id="quizTag">Pilar · Módulo</span>
        <h2 id="quizTitle">Evaluación de conocimiento</h2>
      </div>
    </div>

    <div class="identity-card">
      <div class="field">
        <label for="participantName">Nombre completo del participante</label>
        <input type="text" id="participantName" placeholder="Escribe tu nombre y apellido">
      </div>
      <div class="field">
        <label for="participantDoc">Número de documento (opcional)</label>
        <input type="text" id="participantDoc" placeholder="Cédula / documento">
      </div>
    </div>

    <div id="quizQuestions"></div>

    <div class="quiz-footer">
      <div class="quiz-progress" id="quizProgress">0 de 2 preguntas respondidas</div>
      <div style="display:flex; gap:10px;">
        <button class="btn btn-ghost" id="backToContent">← Volver al módulo</button>
        <button class="btn btn-accent" id="submitQuiz">Enviar evaluación</button>
      </div>
    </div>
    <div class="error-msg" id="quizError"></div>
  </section>

  <!-- ================= RESULT ================= -->
  <section class="screen" id="screen-result">
    <div class="result-wrap">
      <div class="gauge" id="gauge">
        <div class="ring" id="gaugeRing"></div>
        <div class="center"><span id="gaugeScore">0.0</span><small>de 5.0</small></div>
      </div>
      <h2 class="result-title" id="resultTitle">Resultado</h2>
      <p class="result-msg" id="resultMsg"></p>
      <div class="result-actions" id="resultActions"></div>
    </div>
  </section>

  <!-- ================= CERTIFICATE ================= -->
  <section class="screen" id="screen-certificate">
    <div class="cert-stage">
      <div class="certificate" id="certificate-print">
        <div class="cert-inner">
          <div class="stamp">
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><path d="M20 6 9 17l-5-5"></path></svg>
          </div>
          <div class="cert-brand-row">
            <img id="certLogo" src="" alt="" style="display:none;">
            <div>
              <p class="cert-eyebrow">Certificado digital de formación</p>
              <p class="cert-org" id="certOrgName">Centro de Formación</p>
              <p class="cert-nit" id="certOrgNit"></p>
            </div>
          </div>
          <h2 class="cert-title">Certificado de Participación y Aprobación</h2>
          <p class="cert-sub">Se otorga el presente certificado a</p>
          <div class="cert-name-wrap">
            <div class="cert-name" id="certName">Nombre del Participante</div>
            <div class="cert-doc" id="certDoc"></div>
          </div>
          <p class="cert-body-text">Por haber participado en la lección y <b>aprobado la evaluación de conocimiento</b> del módulo <b id="certCourse">Módulo</b>, perteneciente al pilar <b id="certPillar">Pilar</b>, con una calificación de <b id="certScore">0.0 / 5.0</b>, cumpliendo el mínimo aprobatorio establecido.</p>
          <div class="cert-meta">
            <span id="certDate">Fecha: —</span>
            <span id="certId">ID: —</span>
          </div>
        </div>
      </div>
      <div class="cert-actions no-print">
        <button class="btn btn-outline" id="printCert">Imprimir / Descargar PDF</button>
        <button class="btn btn-outline" id="nextModuleFromCert" style="display:none;">Siguiente módulo →</button>
        <button class="btn btn-accent" id="backToPillarFromCert">Volver al pilar</button>
      </div>
    </div>
  </section>

</main>

<footer class="app-footer no-print">Centro de Formación — Herramienta interna de formación autoservicio. Calificación de aprobación: 3.0 / 5.0 o superior.</footer>

<script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
<script>
// ============================================================
// Contenido del Centro de Formación — Modelo por pilares y módulos
// Normatividad verificada vigente para Colombia — 2026
// ============================================================

// Matrícula incrustada: se reemplaza automáticamente al generar el archivo listo para publicar.
// No editar esta línea a mano — usar el botón "Generar archivo para publicar" del panel de administrador.
let EMBEDDED_ROSTER = [{"cedula":"71293479","name":"Andres Felipe Perez Zabala","cargo":"Profesional SST","area":"","sede":"Medellin","correo":"andresfelipeperezsst@gmail.com"},{"cedula":"43275566","name":"Sandra Yanet Duque Rios","cargo":"Ejecutiva Comercial","area":"","sede":"Medellin","correo":"ejecutivacomercial2@piensaseguros.com"},{"cedula":"1110495592","name":"Maira Alejandra Rivera Jimenez","cargo":"Directora Comercial","area":"","sede":"Medellin","correo":"directoracomercial@piensaseguros.com"},{"cedula":"79654720","name":"Alejandro Velez Ramos","cargo":"Director de Seguros","area":"","sede":"Medellin","correo":"directorseguros@piensaseguros.com"},{"cedula":"1216723430","name":"Santiago Correa Gomez","cargo":"Director general de Seguros","area":"","sede":"Medellin","correo":"directorgeneraseguros@piensaseguros.com"},{"cedula":"42693476","name":"Liliana Maria Cadavid Jaramillo","cargo":"Directora Administrativa","area":"","sede":"Medellin","correo":"administrativa@piensaseguros.com"},{"cedula":"43003947","name":"Gloria Patricia Cardona","cargo":"Gerente general","area":"","sede":"Medellin","correo":"gerentegenral@piensaseguros.com"}];
// Estado de pilares habilitados/bloqueados incrustado (mismo mecanismo que EMBEDDED_ROSTER).
let EMBEDDED_LOCKS = {"copasst":true,"convivencia":true,"sst":true,"brigada":true,"ambiental":true,"pesv":true,"calidad":true};
// Marca de la empresa cliente (logo, nombre, NIT) incrustada — se muestra en la interfaz y en los certificados.
let EMBEDDED_BRANDING = {"logo":"data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAMCAgICAgMCAgIDAwMDBAYEBAQEBAgGBgUGCQgKCgkICQkKDA8MCgsOCwkJDRENDg8QEBEQCgwSExIQEw8QEBD/2wBDAQMDAwQDBAgEBAgQCwkLEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBD/wAARCALQA8ADASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD9U6KKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAoor4k/4KPftdan8F/DUHwu+HepLb+LfEERa4uUP7yxtCMb19GbkA9qASufRnxC/aY+Bfwt+0L42+I+kWMlqu6aJZfNkT2Kpk59q47w9+3p+yl4oeePSPi1pzm3UNJ5kUkeAemNyjNfhfd3F1qF3L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EyfQ06KKKCAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA8U/bS1e/0H9lf4latpkix3VvojmNmXIBLqDx9Ca/BWMlkDnqw3H6nk1+7X7d9xFB+yP8TBK20y6OY092MiYH6V+EkX+qT/dH8qC47D6KKKCgooooAK9i/Y+8HW3jr9pTwNoV3C0kcWoLf7VODmEhgfpXjtfW/wDwS98KHXf2orLXW5j0LTrmRlxwWdMKfwNAnsfs5RVHV9d0Tw/afb9f1ix022zt868uEhjz6bnIGar6T4t8Ka9j+wvE+k6ju6fZL2ObP/fLGgzNaiivHP2ov2jvC/7N3w3u/Fer3EMmqzo0WlWJYb7ifHBx12g8mgD5w/4Kd/tSJ4E8Hj4HeD9QI17xJFnUpYW5tbTuhI+6zcY9q/J1RtAGc+/rW/478c+JfiV4v1Txz4v1CS81TVp2nld2yEBPCL6KOgrBoNErBRRRQMKtaXpepa5qdpomjWj3V/fTLBbwoMs7scAcVV5yAoJLEAAdST0FfqR/wTn/AGJj4Tt7T47/ABT0of2zcx79EsZ1z9liYf61lPRiOlAm7H0B+xF+zFZfs3/CqC01GJZfFOthbvVrgrhlYj5Yh6BQcfWvouiigzCiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA+eP+CgH/JpXxA/68B/6GK/DGL/VJ/uiv3O/4KAf8mlfED/rwH/oYr8MYv8AVJ/uiguOw6iiigoK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RRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFfnv8Atpf8FBvir8BvjPN8MPAHhzRJbays4bma4v1ZnkZxnAxwBX6EV+Kn/BTX/k7fWf8AsFWf/oJoKirs7Qf8Fcf2iQAD4G8Fn3xP/wDFUv8Aw9y/aJ/6EXwV+U//AMVXxFRQVyo+3f8Ah7l+0T/0Ivgr8p//AIqtjwz/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/wCEE8FD/mVNK/8AARP8KClKx+D/AOzn8TPGfwD+L+hfEbTtA1dobaYW9/ELSXEts5w4xjk4r98dH1KLWdIsdXgRkjvraK5RXGGVXUMAR681nDwL4LBBHhXSsjkf6In+FbaIsaKiKFVQAABgAelAm7jqKKKBBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFRz3EFrE09zMkUSDLO7BVA9yaNgJKK4PWPjz8FfD9x9k1v4p+GLGb+5PqcSn8ia0fD3xX+Gfi1lTwz490LU2f7otb6OQn6YNC97YH7u51dFHWigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigBGJVSQM4Gcetfkn8Yfi545/aE/bEf4J/EXx7f+CPBlhqjWSW8Mxt9yqRgs2RnfnGTxX6214V8ev2Mvgf+0Izah4v0B7PWeMarpz+RcnHTcw+8KzS5a8KslzRW6+7X5eZqpJ0Z00+WUtn2/4cytA/YM/ZUs9OjX/hXVnrBdQWu7y4e4eU/wB7cWPX2qxD+wh+zTYa7ZeI9C8ESaPfWM6TxtYXssSkqcgFQ2CK8ktv2N/2ofhXKZvgt+09qE2nQJtttG1hDJEAOg3H8q5K5/bl/aM/Zq8V2fhT9rT4d2NxZXsm2HWNHwsfl/3h2cgckVvGcXUXLK0ul9NfXb8TFwmoO6uuttfw3P0IjRYo1jQYVAFH0FVNX1vRtAtGv9c1W00+2QZaW5mWNB+LEVjaN8Q/DfiPwCnxG0C8F5pE1i1/FIv8SBS2D6HjFfkynx5079qT9oDUNW+P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b0Plub/goP8ADG9tpB4S8EeM9fv14Fnb6VIjlvQlgBXzz44+Bn7TP7efxK03XfiZ4Ub4f+ANJf8A0W0umzPJETywH98jg1+kyWdnGd0drCp9QgFTU4qCmqkldrVX2T72/wAxOU1Fwi7X3729TF8GeE9J8C+FdL8IaHF5djpNrHawg9SqqBk+5xW1RRVTk5ycpbsiEVCKjHZBRRRUlBRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFAH//2Q==","name":"Piensa Seguro Ltda.","nit":"901580775-5"};

const ICONS = {
  helmet: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M10 40c0-14 9-26 22-26s22 12 22 26"/><path d="M8 40h48"/><path d="M8 40v4a4 4 0 0 0 4 4h40a4 4 0 0 0 4-4v-4"/><path d="M32 14V8"/><path d="M22 40c0-8 4-14 10-14s10 6 10 14"/></svg>`,
  leaf: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M14 50C10 34 18 16 40 12c8 16 2 34-12 40-6 2.4-10.4 1.6-14-2Z"/><path d="M14 50 40 14"/></svg>`,
  wheel: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="32" cy="32" r="22"/><circle cx="32" cy="32" r="6"/><path d="M32 10v10M32 44v10M10 32h10M44 32h10M17 17l7 7M40 40l7 7M47 17l-7 7M24 40l-7 7"/></svg>`,
  check: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="32" cy="32" r="22"/><path d="M22 33l7 7 14-15"/></svg>`,
  fire: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M32 8c4 8-4 10-4 18 0 5 3 8 4 8s4-3 4-8"/><path d="M22 30c-4 5-6 10-6 16a16 16 0 0 0 32 0c0-8-4-13-8-18-1 6-4 9-6 9-3 0-4-4-3-9-4 0-7 1-9 2Z"/></svg>`,
  shield: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M32 6l20 8v14c0 14-9 24-20 30-11-6-20-16-20-30V14l20-8Z"/><path d="M23 32l6 6 12-14"/></svg>`,
  dialogue: `<svg viewBox="0 0 64 64" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M8 14h30v20H24l-8 8v-8H8z"/><path d="M34 24h22v16h-6v8l-8-8h-8z"/></svg>`,
  lock: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="11" width="16" height="10" rx="2"/><path d="M7 11V8a5 5 0 0 1 10 0v3"/></svg>`,
  unlock: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><rect x="4" y="11" width="16" height="10" rx="2"/><path d="M7 11V8a5 5 0 0 1 9-3"/></svg>`,
  check_circle: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="9"/><path d="M8 12.5l2.5 2.5L16 9.5"/></svg>`,
  play_circle: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="9"/><path d="M10 8.5l6 3.5-6 3.5v-7Z"/></svg>`,
  idea: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 18h6M10 21h4"/><path d="M12 3a6 6 0 0 0-4 10.5c.6.6 1 1.4 1 2.5h6c0-1.1.4-1.9 1-2.5A6 6 0 0 0 12 3Z"/></svg>`,
  star: `<svg viewBox="0 0 24 24" fill="currentColor" stroke="none"><path d="M12 2.5c.6 3 1.6 5.3 3 6.7 1.4 1.4 3.7 2.4 6.7 3-3 .6-5.3 1.6-6.7 3-1.4 1.4-2.4 3.7-3 6.7-.6-3-1.6-5.3-3-6.7-1.4-1.4-3.7-2.4-6.7-3 3-.6 5.3-1.6 6.7-3 1.4-1.4 2.4-3.7 3-6.7Z"/></svg>`,
  spark: `<svg viewBox="0 0 24 24" fill="currentColor" stroke="none"><path d="M13 2 4 14h6l-1 8 9-12h-6l1-8Z"/></svg>`,
  target: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><circle cx="12" cy="12" r="9"/><circle cx="12" cy="12" r="5"/><circle cx="12" cy="12" r="1.2" fill="currentColor" stroke="none"/></svg>`,
  flag: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 21V4"/><path d="M5 4h13l-3 4 3 4H5"/></svg>`,
  trophy: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 4h10v5a5 5 0 0 1-10 0V4Z"/><path d="M7 5H4a3 3 0 0 0 3 3M17 5h3a3 3 0 0 1-3 3"/><path d="M12 14v3M9 21h6M10 17h4v2.5a1.5 1.5 0 0 1-1.5 1.5h-1a1.5 1.5 0 0 1-1.5-1.5V17Z"/></svg>`,
  upload: `<svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 16V4M7 9l5-5 5 5"/><path d="M4 16v3a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-3"/></svg>`,
};

// Íconos "sticker" decorativos que acompañan al ícono principal en la portada de cada pilar
const PILLAR_ACCENTS = {
  copasst: ["target", "flag"],
  convivencia: ["idea", "star"],
  sst: ["target", "spark"],
  brigada: ["spark", "flag"],
  ambiental: ["star", "idea"],
  pesv: ["flag", "target"],
  calidad: ["star", "spark"],
};

const PILLARS = {
  "copasst": {
    "label": "Copasst",
    "icon": "shield",
    "desc": "Comité Paritario de Seguridad y Salud en el Trabajo",
    "keywords": [
      "copasst",
      "comite paritario",
      "comité paritario",
      "vigia",
      "vigía"
    ],
    "modules": [
      {
        "key": "plan_capacitaciones",
        "title": "Plan de capacitaciones",
        "intro": "El plan de capacitaciones del Copasst organiza, año a año, los temas que sus integrantes deben conocer para cumplir su función.",
        "points": [
          "Se construye para toda la vigencia anual",
          "Incluye normatividad, investigación de accidentes e inspecciones",
          "Debe quedar documentado dentro del SG-SST"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué exige el Decreto 1072 de 2015 respecto a la capacitación de los miembros del Copasst?",
            "options": [
              "Que se capaciten solo si lo solicitan",
              "Que participen en las capacitaciones programadas por la ARL y que queden documentadas",
              "Que se capaciten únicamente el primer año de gestión",
              "Que la capacitación sea opcional para los suplentes"
            ],
            "correct": 1
          },
          {
            "q": "¿Con qué frecuencia se construye el plan de capacitaciones del Copasst?",
            "options": [
              "Una sola vez, al conformarse el comité",
              "Cada cinco años",
              "Año a año, para cada vigencia",
              "Solo cuando ocurre un accidente grave"
            ],
            "correct": 2
          }
        ],
        "apply": "Antes de terminar el año, siéntate con tu Copasst y define juntos los 3 temas que más necesitan reforzar para el próximo periodo. Escríbelos en un cronograma simple con fechas — eso ya es tu plan de capacitaciones."
      },
      {
        "key": "politicas_objetivos_sgsst",
        "title": "Políticas y objetivos del SG-SST",
        "intro": "La política de SST expresa el compromiso de la alta dirección con la seguridad de los trabajadores, y los objetivos la traducen en metas medibles.",
        "points": [
          "Debe estar firmada por la representación legal",
          "El Copasst la recibe directamente de la alta dirección",
          "Debe ser coherente con los riesgos reales de la empresa"
        ],
        "norm": "Decreto 1072 de 2015, art. 2.2.4.6.5",
        "questions": [
          {
            "q": "¿De quién debe recibir el Copasst la comunicación de la política de SST?",
            "options": [
              "De la ARL únicamente",
              "De la alta dirección de la empresa",
              "Del Ministerio del Trabajo",
              "De cualquier trabajador que la redacte"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué convierte una política de SST en algo más que una declaración de buenas intenciones?",
            "options": [
              "Que esté enmarcada en la oficina",
              "Que se traduzca en objetivos medibles y sea coherente con los riesgos reales",
              "Que la conozca solo la gerencia",
              "Que se actualice cada diez años"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que leas la política de SST de tu empresa, pregúntate: ¿realmente refleja los riesgos que veo a diario en mi área? Si no, coméntalo en la próxima reunión del Copasst."
      },
      {
        "key": "intervencion_riesgos_prioritarios",
        "title": "Intervención de riesgos prioritarios",
        "intro": "No todos los riesgos se atienden al mismo tiempo: los riesgos prioritarios requieren intervención inmediata por su nivel de exposición o gravedad.",
        "points": [
          "Se priorizan según exposición y gravedad",
          "El Copasst participa en la priorización",
          "Se hace seguimiento a que los controles realmente se implementen"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué define que un riesgo sea considerado prioritario?",
            "options": [
              "Que lo mencione un solo trabajador",
              "Su nivel de exposición y gravedad",
              "Que aparezca primero en la matriz",
              "El presupuesto disponible ese año"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuál es el rol del Copasst frente a un riesgo prioritario ya identificado?",
            "options": [
              "Ignorarlo hasta la próxima auditoría",
              "Hacer seguimiento a que las medidas de control se implementen realmente",
              "Delegarlo por completo a la ARL",
              "Esperar a que ocurra un accidente para actuar"
            ],
            "correct": 1
          }
        ],
        "apply": "Haz una lista mental de los 3 riesgos que más te preocupan de tu puesto de trabajo. Llévala a la próxima reunión del Copasst: así empieza la priorización real."
      },
      {
        "key": "matriz_peligros",
        "title": "Matriz de peligros",
        "intro": "La matriz de peligros identifica, por área y por cargo, los riesgos a los que está expuesto cada trabajador y su nivel.",
        "points": [
          "Es la base técnica del SG-SST",
          "El Copasst debe conocerla y participar en su actualización",
          "Sustenta las recomendaciones e inspecciones del comité"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué identifica la matriz de peligros?",
            "options": [
              "Únicamente los accidentes ya ocurridos",
              "Los riesgos por área y cargo, y su nivel de exposición",
              "El organigrama de la empresa",
              "El presupuesto del área de SST"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué papel cumple el Copasst frente a la matriz de peligros?",
            "options": [
              "Ninguno, es responsabilidad exclusiva del profesional SST",
              "Conocerla y participar en su actualización periódica",
              "Elaborarla sin apoyo de nadie más",
              "Aprobarla solo si hay accidentes reportados"
            ],
            "correct": 1
          }
        ],
        "apply": "Busca la matriz de peligros de tu área y revisa si de verdad describe lo que haces día a día. Si algo cambió y no está reflejado, repórtalo."
      },
      {
        "key": "trabajo_equipo",
        "title": "Trabajo en equipo",
        "intro": "El Copasst está conformado por igual número de representantes del empleador y de los trabajadores; su eficacia depende de que ambas partes trabajen coordinadas.",
        "points": [
          "Roles claros evitan duplicidad o vacíos de gestión",
          "La comunicación abierta sostiene la confianza del comité",
          "Un comité dividido pierde credibilidad ante los trabajadores"
        ],
        "norm": "Resolución 2013 de 1986",
        "questions": [
          {
            "q": "¿De qué depende principalmente la eficacia del Copasst como equipo?",
            "options": [
              "Del número de reuniones que realice",
              "De que empleador y trabajadores trabajen coordinados, con roles claros",
              "De que siempre esté de acuerdo con la gerencia",
              "De que el presidente tome todas las decisiones solo"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué consecuencia tiene un Copasst internamente dividido?",
            "options": [
              "Ninguna, sigue funcionando igual",
              "Pierde la confianza de los trabajadores en el comité",
              "Obtiene más presupuesto de la empresa",
              "Se disuelve automáticamente por ley"
            ],
            "correct": 1
          }
        ],
        "apply": "Si eres miembro del Copasst, en la próxima reunión pregúntate: ¿estoy aportando información real de mi área, o solo asistiendo?"
      },
      {
        "key": "evaluaciones_ambientales",
        "title": "Evaluaciones ambientales",
        "intro": "Las evaluaciones ambientales de puesto de trabajo miden factores como ruido, iluminación, temperatura o calidad del aire, para verificar que estén dentro de límites seguros.",
        "points": [
          "Miden condiciones físicas del entorno de trabajo",
          "El Copasst puede solicitarlas ante molestias o riesgos",
          "Sus resultados alimentan la matriz de peligros"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué mide una evaluación ambiental de puesto de trabajo?",
            "options": [
              "El desempeño individual del trabajador",
              "Factores como ruido, iluminación, temperatura o calidad del aire",
              "Las ventas del área evaluada",
              "La antigüedad de los equipos"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuándo puede el Copasst solicitar una evaluación ambiental?",
            "options": [
              "Nunca, es una decisión exclusiva de la ARL",
              "Cuando identifique condiciones que generan molestia o riesgo",
              "Solo una vez al conformarse el comité",
              "Únicamente si lo pide un cliente externo"
            ],
            "correct": 1
          }
        ],
        "apply": "Si notas que un área siempre está muy ruidosa, mal iluminada o con mala ventilación, no lo des por normal: repórtalo al Copasst."
      },
      {
        "key": "ambiente_trabajo",
        "title": "Ambiente de trabajo",
        "intro": "Un ambiente de trabajo seguro no es solo la ausencia de peligros físicos: incluye orden, iluminación adecuada, ventilación y un clima laboral sano.",
        "points": [
          "Va más allá de la seguridad física",
          "Incluye orden, iluminación, ventilación y clima laboral",
          "El Copasst lo verifica en sus visitas periódicas"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué elementos componen un ambiente de trabajo seguro, además de la ausencia de peligros físicos?",
            "options": [
              "Solo el salario de los trabajadores",
              "Orden, iluminación adecuada, ventilación y un clima laboral sano",
              "El logo y los colores corporativos",
              "El número de años de la empresa"
            ],
            "correct": 1
          },
          {
            "q": "¿Cómo verifica el Copasst las condiciones del ambiente de trabajo?",
            "options": [
              "Con encuestas de clima laboral externas contratadas anualmente",
              "Mediante visitas periódicas a los lugares de trabajo",
              "No es función del Copasst verificarlo",
              "Solo cuando el gerente lo solicita"
            ],
            "correct": 1
          }
        ],
        "apply": "En tu próxima recorrida por la empresa, fíjate en algo simple: ¿el pasillo está despejado? ¿hay buena luz? Eso es justo lo que revisa un buen inspector del Copasst."
      },
      {
        "key": "gestion_del_cambio",
        "title": "Gestión del cambio",
        "intro": "Cada vez que la empresa cambia un proceso, una máquina, una instalación o un método de trabajo, pueden aparecer riesgos nuevos.",
        "points": [
          "Evalúa riesgos nuevos antes de implementar un cambio",
          "Aplica a procesos, máquinas, instalaciones y métodos",
          "El Copasst debe ser informado de cambios que afecten la seguridad"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Para qué sirve la gestión del cambio dentro del SG-SST?",
            "options": [
              "Para cambiar de ARL cada año",
              "Para evaluar los riesgos nuevos antes de implementar un cambio",
              "Para rotar al personal del Copasst",
              "Para actualizar el logo de la empresa"
            ],
            "correct": 1
          },
          {
            "q": "¿Debe el Copasst ser informado de un cambio de maquinaria en la empresa?",
            "options": [
              "No, es un tema exclusivamente técnico",
              "Sí, si ese cambio puede afectar la seguridad de los trabajadores",
              "Solo si la maquinaria es importada",
              "Solo si el cambio cuesta más de mil salarios mínimos"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que se anuncie un cambio de máquina o proceso en tu área, pregunta si ya se evaluaron los riesgos nuevos antes de arrancar."
      },
      {
        "key": "indicadores",
        "title": "Indicadores",
        "intro": "Los indicadores del SG-SST, de estructura, proceso y resultado, permiten medir si el sistema está funcionando realmente.",
        "points": [
          "Existen indicadores de estructura, proceso y resultado",
          "El índice de accidentalidad es uno de los más usados",
          "Orientan las recomendaciones del Copasst"
        ],
        "norm": "Resolución 0312 de 2019",
        "questions": [
          {
            "q": "¿Para qué recibe y analiza el Copasst los indicadores del SG-SST?",
            "options": [
              "Solo para archivarlos",
              "Para orientar sus recomendaciones y verificar el impacto real de las medidas",
              "Para calcular el salario de los trabajadores",
              "Para definir el organigrama de la empresa"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué tipo de indicador es el índice de accidentalidad?",
            "options": [
              "Un indicador de resultado",
              "Un indicador financiero",
              "Un indicador de mercadeo",
              "Un indicador de nómina"
            ],
            "correct": 0
          }
        ],
        "apply": "Pide ver el índice de accidentalidad de tu empresa del último trimestre. Compararlo con el anterior te dice, en segundos, si las medidas están funcionando."
      },
      {
        "key": "planes_accion",
        "title": "Planes de acción",
        "intro": "Un plan de acción define qué se va a hacer frente a un riesgo o hallazgo, quién lo hará y para cuándo.",
        "points": [
          "Define responsable y fecha de cumplimiento",
          "El Copasst hace seguimiento a su cumplimiento",
          "Se reportan los retrasos a la alta dirección"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué elementos debe tener todo plan de acción frente a un riesgo?",
            "options": [
              "Solo una descripción general del problema",
              "Qué se hará, quién lo hará y para cuándo",
              "El nombre del proveedor de EPP",
              "Una foto del lugar de trabajo"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué debe hacer el Copasst si un plan de acción se atrasa?",
            "options": [
              "Nada, no es su función",
              "Reportarlo a la alta dirección",
              "Cancelarlo automáticamente",
              "Esperar el siguiente año para revisarlo"
            ],
            "correct": 1
          }
        ],
        "apply": "Si el Copasst propuso una acción hace meses y no ves avances, pregunta en la próxima reunión quién es el responsable y para cuándo estaba comprometida."
      },
      {
        "key": "investigacion_atel",
        "title": "Investigación de ATEL",
        "intro": "ATEL significa Accidentes de Trabajo y Enfermedad Laboral. El Copasst participa activamente en la investigación de estos eventos.",
        "points": [
          "El Copasst ayuda a identificar las causas reales, no solo la inmediata",
          "Propone medidas correctivas para evitar repetición",
          "Su participación es activa, no solo formal"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué significa la sigla ATEL?",
            "options": [
              "Auditoría Técnica de Elementos Laborales",
              "Accidentes de Trabajo y Enfermedad Laboral",
              "Área de Trabajo en Espacios Limitados",
              "Actividades de Terreno y Logística"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué busca el Copasst al investigar un accidente, más allá de la causa inmediata?",
            "options": [
              "Encontrar un culpable para sancionarlo",
              "Identificar las causas reales y proponer medidas correctivas",
              "Cerrar el caso lo más rápido posible",
              "Determinar el costo del accidente"
            ],
            "correct": 1
          }
        ],
        "apply": "Si presencias o eres parte de un incidente, por menor que parezca, repórtalo formalmente. Sin ese reporte, el Copasst no puede investigar."
      },
      {
        "key": "roles_responsabilidades",
        "title": "Roles y responsabilidades del Copasst",
        "intro": "El Copasst tiene presidente, secretario y miembros principales y suplentes, con roles definidos en la Resolución 2013 de 1986.",
        "points": [
          "Presidente, secretario, principales y suplentes",
          "Conocer los roles evita que las funciones queden en el papel",
          "Está conformado por igual número de representantes del empleador y de los trabajadores"
        ],
        "norm": "Resolución 2013 de 1986",
        "questions": [
          {
            "q": "¿Cómo está conformado el Copasst?",
            "options": [
              "Solo por representantes del empleador",
              "Solo por representantes de los trabajadores",
              "Por igual número de representantes del empleador y de los trabajadores",
              "Por un único representante externo"
            ],
            "correct": 2
          },
          {
            "q": "¿Qué roles existen dentro del Copasst según la Resolución 2013 de 1986?",
            "options": [
              "Solo un coordinador general",
              "Presidente, secretario y miembros principales y suplentes",
              "Gerente y subgerente",
              "Auditor externo únicamente"
            ],
            "correct": 1
          }
        ],
        "apply": "Si no sabes quién es el presidente o el secretario actual del Copasst de tu empresa, pregúntalo — saber a quién dirigirte agiliza cualquier reporte."
      },
      {
        "key": "normatividad_copasst",
        "title": "Normatividad Copasst",
        "intro": "El marco legal del Copasst se compone principalmente de la Resolución 2013 de 1986, el Decreto 1295 de 1994 y el Decreto 1072 de 2015.",
        "points": [
          "Resolución 2013 de 1986: organización y funciones",
          "Decreto 1295 de 1994: exige Vigía en empresas de menos de 10 trabajadores",
          "Decreto 1072 de 2015: añade funciones relacionadas con el SG-SST"
        ],
        "norm": "Resolución 2013 de 1986, Decreto 1295 de 1994, Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Cuál es la norma que regula específicamente la organización y funcionamiento del Copasst?",
            "options": [
              "Resolución 0312 de 2019",
              "Resolución 2013 de 1986",
              "Ley 2466 de 2025",
              "Decreto 1076 de 2015"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué establece el Decreto 1295 de 1994 para empresas de menos de 10 trabajadores?",
            "options": [
              "Que no requieren ningún tipo de gestión de SST",
              "Que deben nombrar un Vigía de SST en lugar de un Copasst completo",
              "Que el Copasst debe tener 20 integrantes",
              "Que deben afiliarse a dos ARL distintas"
            ],
            "correct": 1
          }
        ],
        "apply": "Guarda en tus favoritos la Resolución 2013 de 1986: es corta y te da claridad inmediata sobre qué puede y debe hacer el Copasst."
      },
      {
        "key": "como_identificar_agresor",
        "title": "Cómo identificar un agresor",
        "intro": "Reconocer señales de una persona con conducta agresiva o de riesgo dentro de la empresa permite actuar a tiempo, antes de que la situación escale.",
        "points": [
          "Lenguaje amenazante o aislamiento súbito son señales de alerta",
          "También lo son las conductas de control o intimidación",
          "El Copasst y el Comité de Convivencia deben coordinar la ruta de atención"
        ],
        "norm": "Ley 1010 de 2006 (marco de referencia)",
        "questions": [
          {
            "q": "¿Cuál de las siguientes es una señal de alerta de una posible conducta agresiva en el trabajo?",
            "options": [
              "Puntualidad en las reuniones",
              "Lenguaje amenazante o conductas de control e intimidación",
              "Participar activamente en capacitaciones",
              "Tomar vacaciones programadas"
            ],
            "correct": 1
          },
          {
            "q": "¿Con quién debe coordinar el Copasst la ruta de atención ante señales de un posible agresor?",
            "options": [
              "Con ningún otro comité, actúa solo",
              "Con el Comité de Convivencia Laboral",
              "Directamente con un juzgado",
              "Con la competencia de la empresa"
            ],
            "correct": 1
          }
        ],
        "apply": "Si notas en un compañero un cambio repentino de comportamiento —aislamiento, lenguaje amenazante— coméntalo con discreción al Copasst o al Comité de Convivencia."
      },
      {
        "key": "inspecciones_vehiculos",
        "title": "Inspecciones a vehículos",
        "intro": "Cuando la empresa opera vehículos, el Copasst puede participar en las inspecciones preoperacionales que verifican su estado antes de cada uso.",
        "points": [
          "Verifican el estado mecánico y de seguridad",
          "Se realizan antes de cada uso del vehículo",
          "Se articulan con el control de riesgos del PESV"
        ],
        "norm": "Resolución 40595 de 2022 (PESV)",
        "questions": [
          {
            "q": "¿Qué verifica una inspección preoperacional a un vehículo?",
            "options": [
              "Solo la limpieza exterior",
              "El estado mecánico y de seguridad antes de cada uso",
              "El precio de reventa del vehículo",
              "El color de la pintura"
            ],
            "correct": 1
          },
          {
            "q": "¿Con qué otro instrumento se articula la inspección de vehículos que puede acompañar el Copasst?",
            "options": [
              "El plan estratégico comercial",
              "El Plan Estratégico de Seguridad Vial (PESV)",
              "El manual de marketing",
              "El reglamento de propiedad horizontal"
            ],
            "correct": 1
          }
        ],
        "apply": "Si tu empresa usa vehículos, pregunta si existe un formato de inspección preoperacional y si realmente se diligencia antes de cada salida."
      },
      {
        "key": "inspecciones_seguridad",
        "title": "Inspecciones de seguridad",
        "intro": "Las inspecciones planeadas son recorridos programados por los lugares de trabajo para identificar condiciones inseguras antes de que causen un accidente.",
        "points": [
          "Deben ser periódicas, no improvisadas",
          "El Copasst deja constancia escrita de los hallazgos",
          "Se hace seguimiento a la corrección de cada hallazgo"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué debe hacer el Copasst al encontrar condiciones inseguras en una inspección?",
            "options": [
              "Ignorarlas si no son graves",
              "Dejar constancia escrita y hacer seguimiento a su corrección",
              "Sancionar directamente al trabajador responsable",
              "Esperar a la siguiente auditoría externa"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué diferencia a una inspección planeada de una revisión improvisada?",
            "options": [
              "Ninguna, son lo mismo",
              "Que está programada y tiene un propósito definido de identificar riesgos",
              "Que la hace solo el gerente general",
              "Que no requiere registro alguno"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que veas un cable suelto o una salida obstruida, no esperes a la inspección formal: repórtalo de inmediato."
      },
      {
        "key": "eliminacion_sustitucion_mitigacion",
        "title": "Eliminación, sustitución y mitigación",
        "intro": "Ante un riesgo, la jerarquía de controles prioriza primero eliminarlo, luego sustituirlo, y solo al final mitigar sus efectos.",
        "points": [
          "Eliminar el riesgo es siempre la primera opción",
          "Sustituir por algo menos peligroso es la segunda",
          "El EPP es el último recurso, no el primero"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "Ante un riesgo identificado, ¿cuál debe ser la primera opción según la jerarquía de controles?",
            "options": [
              "Entregar EPP",
              "Eliminar el riesgo",
              "Capacitar al trabajador",
              "Señalizar la zona"
            ],
            "correct": 1
          },
          {
            "q": "¿En qué lugar de la jerarquía de controles se ubica el uso de EPP?",
            "options": [
              "Es siempre la primera opción",
              "Es la segunda opción, antes que eliminar el riesgo",
              "Es el último recurso, cuando no se pudo eliminar ni sustituir el riesgo",
              "No forma parte de la jerarquía de controles"
            ],
            "correct": 2
          }
        ],
        "apply": "Antes de pedir más EPP para un riesgo, pregúntate: ¿ya se intentó eliminar o sustituir ese riesgo? El EPP es el último recurso."
      },
      {
        "key": "orden_limpieza",
        "title": "Orden y limpieza",
        "intro": "Un lugar de trabajo desordenado multiplica el riesgo de caídas, golpes e incendios. No es un tema estético, es una condición básica de seguridad.",
        "points": [
          "El desorden aumenta el riesgo de caídas y golpes",
          "También incrementa el riesgo de incendio",
          "El Copasst lo verifica en cada inspección"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Por qué el orden y la limpieza se consideran una condición de seguridad y no solo un tema estético?",
            "options": [
              "Porque mejoran la imagen ante visitantes únicamente",
              "Porque el desorden multiplica el riesgo de caídas, golpes e incendios",
              "Porque lo exige el área de mercadeo",
              "Porque reduce el consumo de energía"
            ],
            "correct": 1
          },
          {
            "q": "¿En qué actividad del Copasst se verifica el orden y la limpieza del lugar de trabajo?",
            "options": [
              "En las inspecciones periódicas",
              "Solo en la evaluación de fin de año",
              "Nunca, es responsabilidad exclusiva de aseo general",
              "En la revisión de nómina"
            ],
            "correct": 0
          }
        ],
        "apply": "Dedica dos minutos al final de tu jornada a dejar tu puesto ordenado. Es la medida de seguridad más simple y la que más rápido se olvida."
      },
      {
        "key": "auditoria",
        "title": "Auditoría",
        "intro": "La auditoría del SG-SST verifica, con evidencia, si lo documentado realmente se cumple en la práctica, no busca culpables sino oportunidades de mejora.",
        "points": [
          "Verifica con evidencia, no con suposiciones",
          "El Copasst puede participar como observador o insumo",
          "Aporta lo identificado durante el año de gestión"
        ],
        "norm": "Resolución 0312 de 2019",
        "questions": [
          {
            "q": "¿Qué verifica principalmente una auditoría del SG-SST?",
            "options": [
              "El salario de los trabajadores",
              "Si lo documentado realmente se cumple en la práctica",
              "El logo de la empresa",
              "Las ventas del último trimestre"
            ],
            "correct": 1
          },
          {
            "q": "¿Cómo puede participar el Copasst en la auditoría interna del SG-SST?",
            "options": [
              "No puede participar bajo ninguna circunstancia",
              "Como observador o insumo, aportando lo identificado durante el año",
              "Solo si es contratado como auditor externo",
              "Firmando el informe sin revisarlo"
            ],
            "correct": 1
          }
        ],
        "apply": "Si el Copasst participa como observador de una auditoría, prepárate llevando por escrito los hallazgos que has identificado en el año."
      }
    ]
  },
  "convivencia": {
    "label": "Comité de Convivencia Laboral",
    "icon": "dialogue",
    "desc": "Prevención del acoso laboral y resolución de conflictos",
    "keywords": [
      "comite de convivencia",
      "comité de convivencia",
      "cocola",
      "convivencia laboral",
      "acoso laboral"
    ],
    "modules": [
      {
        "key": "funciones_comite",
        "title": "Funciones del Comité de Convivencia Laboral",
        "intro": "El Comité de Convivencia Laboral previene el acoso laboral y contribuye a un ambiente de trabajo sano, mediante la recepción y trámite de quejas.",
        "points": [
          "Previene el acoso laboral de forma activa",
          "Recibe y tramita quejas de los trabajadores",
          "Su marco vigente es la Resolución 3461 de 2025"
        ],
        "norm": "Resolución 3461 de 2025",
        "questions": [
          {
            "q": "¿Cuál es la norma vigente que regula la conformación del Comité de Convivencia Laboral?",
            "options": [
              "Resolución 652 de 2012",
              "Resolución 1356 de 2012",
              "Resolución 3461 de 2025",
              "Resolución 0312 de 2019"
            ],
            "correct": 2
          },
          {
            "q": "¿Cuál es una de las funciones principales del Comité de Convivencia Laboral?",
            "options": [
              "Definir los salarios de la empresa",
              "Recibir y tramitar quejas relacionadas con acoso laboral",
              "Aprobar el presupuesto anual",
              "Contratar y despedir personal"
            ],
            "correct": 1
          }
        ],
        "apply": "Si no sabes quiénes son los integrantes actuales del Comité de Convivencia de tu empresa, pregúntalo. Saber a quién acudir es el primer paso."
      },
      {
        "key": "riesgo_psicosocial",
        "title": "Riesgo psicosocial",
        "intro": "El riesgo psicosocial incluye factores como la carga de trabajo, las relaciones interpersonales y el estilo de liderazgo, que pueden afectar la salud mental.",
        "points": [
          "Incluye carga laboral, relaciones y liderazgo",
          "Se mide con la batería de riesgo psicosocial",
          "Su intervención es tarea conjunta del SG-SST y el comité"
        ],
        "norm": "Resolución 2764 de 2022",
        "questions": [
          {
            "q": "¿Qué es el riesgo psicosocial?",
            "options": [
              "Un riesgo exclusivo de cargos administrativos",
              "Factores del trabajo, como la carga laboral o el liderazgo, que pueden afectar la salud mental",
              "Un tipo de riesgo físico relacionado con maquinaria",
              "Un riesgo que solo aplica a empresas grandes"
            ],
            "correct": 1
          },
          {
            "q": "¿Con qué instrumento se identifica el riesgo psicosocial en la empresa?",
            "options": [
              "Con la nómina mensual",
              "Con la batería de riesgo psicosocial (Resolución 2764 de 2022)",
              "Con el manual de funciones",
              "Con el estado de resultados"
            ],
            "correct": 1
          }
        ],
        "apply": "Si sientes que la carga de trabajo te está afectando, no esperes a la próxima batería de riesgo psicosocial: coméntalo con SST o con tu jefe."
      },
      {
        "key": "comunicacion_asertiva",
        "title": "Comunicación asertiva",
        "intro": "Comunicarse de forma asertiva es expresar lo que se piensa o siente con claridad y respeto, sin agredir ni callar.",
        "points": [
          "Es clara y respetuosa a la vez",
          "Evita tanto la agresión como el silencio pasivo",
          "Permite al comité mediar sin tomar partido"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué caracteriza a la comunicación asertiva?",
            "options": [
              "Evitar siempre el conflicto callando la opinión propia",
              "Expresar lo que se piensa o siente con claridad y respeto, sin agredir ni callar",
              "Imponer la propia posición sin escuchar",
              "Comunicarse únicamente por escrito"
            ],
            "correct": 1
          },
          {
            "q": "¿Por qué es útil la comunicación asertiva para el Comité de Convivencia?",
            "options": [
              "Porque le permite mediar sin tomar partido por ninguna de las partes",
              "Porque acelera los despidos",
              "Porque reemplaza la necesidad de escuchar a las partes",
              "Porque evita tener que documentar las quejas"
            ],
            "correct": 0
          }
        ],
        "apply": "La próxima vez que algo te moleste en el trabajo, practica decirlo con una frase clara y respetuosa en el momento, en lugar de callarlo."
      },
      {
        "key": "trabajo_equipo_conv",
        "title": "Trabajo en equipo",
        "intro": "Un equipo que confía entre sí y comparte información abiertamente reduce la probabilidad de malentendidos que escalan a conflictos.",
        "points": [
          "La confianza reduce los malentendidos",
          "El comité también debe funcionar como equipo",
          "Requiere coordinación entre representantes del empleador y de los trabajadores"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué reduce la probabilidad de que un malentendido escale a un conflicto mayor?",
            "options": [
              "Un equipo que confía entre sí y comparte información abiertamente",
              "Evitar cualquier tipo de comunicación",
              "Cambiar de personal constantemente",
              "Reducir las reuniones del equipo"
            ],
            "correct": 0
          },
          {
            "q": "¿Cómo debe funcionar internamente el Comité de Convivencia Laboral?",
            "options": [
              "Cada representante decide por su cuenta",
              "Como un equipo coordinado entre representantes del empleador y de los trabajadores",
              "Solo el presidente toma decisiones",
              "No requiere coordinación interna"
            ],
            "correct": 1
          }
        ],
        "apply": "Si formas parte del Comité de Convivencia, comparte con tus compañeros de comité lo que has escuchado en el área, aunque parezca menor."
      },
      {
        "key": "violencia_lugar_trabajo",
        "title": "Violencia en el lugar de trabajo",
        "intro": "La violencia laboral puede ser física, verbal o psicológica, y provenir de compañeros, jefes o incluso de terceros como clientes o proveedores.",
        "points": [
          "Puede ser física, verbal o psicológica",
          "Puede provenir también de terceros externos",
          "Identificarla a tiempo evita que se vuelva un patrón sostenido"
        ],
        "norm": "Ley 1010 de 2006",
        "questions": [
          {
            "q": "¿De quién puede provenir la violencia laboral, además de compañeros o jefes?",
            "options": [
              "Únicamente de la alta dirección",
              "También de terceros, como clientes o proveedores",
              "Solo de personas ajenas a la empresa",
              "No puede provenir de terceros"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué tipos de violencia laboral existen?",
            "options": [
              "Solo la física",
              "Física, verbal y psicológica",
              "Solo la que ocurre por escrito",
              "Únicamente la que involucra a un superior jerárquico"
            ],
            "correct": 1
          }
        ],
        "apply": "Si un cliente o proveedor externo te trata de forma agresiva, repórtalo igual que reportarías una agresión de un compañero."
      },
      {
        "key": "discriminacion_laboral",
        "title": "Discriminación laboral",
        "intro": "Discriminar es dar un trato desigual e injustificado a una persona por su género, edad, origen, discapacidad u otra condición.",
        "points": [
          "Es un trato desigual e injustificado",
          "El comité debe identificarla y atenderla",
          "Puede articularse con la Ley 1010 de 2006 si configura acoso laboral"
        ],
        "norm": "Ley 1010 de 2006",
        "questions": [
          {
            "q": "¿Qué es la discriminación laboral?",
            "options": [
              "Cualquier evaluación de desempeño",
              "Un trato desigual e injustificado por género, edad, origen, discapacidad u otra condición",
              "Un tipo de contrato laboral",
              "Un beneficio adicional al salario"
            ],
            "correct": 1
          },
          {
            "q": "¿Con qué ley se articula la discriminación laboral cuando configura una conducta persistente?",
            "options": [
              "Ley 1010 de 2006, sobre acoso laboral",
              "Ley 100 de 1993, sobre seguridad social",
              "Ley 1562 de 2012, sobre riesgos laborales",
              "Ley 2191 de 2022, sobre desconexión laboral"
            ],
            "correct": 0
          }
        ],
        "apply": "Si presencias que a un compañero lo tratan distinto por su edad, género u origen, no lo normalices como 'una broma'."
      },
      {
        "key": "negociacion_conflictos",
        "title": "Negociación de conflictos",
        "intro": "Negociar un conflicto no es imponer una posición, sino buscar una solución donde ambas partes ganen algo.",
        "points": [
          "Escuchar activamente es clave",
          "Se separa a la persona del problema",
          "Se buscan intereses comunes, no solo posiciones"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué busca la negociación de un conflicto, según un enfoque constructivo?",
            "options": [
              "Imponer la posición de una de las partes",
              "Una solución donde ambas partes ganen algo",
              "Que una parte ceda totalmente ante la otra",
              "Evitar cualquier tipo de diálogo"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué habilidad es clave para mediar con eficacia en un conflicto?",
            "options": [
              "Interrumpir a las partes para agilizar la conversación",
              "Escuchar activamente y separar a la persona del problema",
              "Tomar partido rápidamente por quien se queja primero",
              "Evitar cualquier reunión entre las partes"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que medies un conflicto entre compañeros, empieza preguntando qué necesita cada uno, no quién tiene la razón."
      },
      {
        "key": "desconexion_laboral",
        "title": "Desconexión laboral",
        "intro": "La Ley 2191 de 2022 garantiza el derecho de todo trabajador a desconectarse de sus labores fuera de la jornada laboral.",
        "points": [
          "Aplica fuera de la jornada laboral",
          "Incluye llamadas, correos y mensajes de trabajo",
          "Su incumplimiento reiterado puede constituir acoso laboral"
        ],
        "norm": "Ley 2191 de 2022",
        "questions": [
          {
            "q": "¿Qué garantiza la Ley 2191 de 2022?",
            "options": [
              "El pago de horas extra automáticas",
              "El derecho a la desconexión laboral fuera de la jornada de trabajo",
              "La estabilidad laboral reforzada",
              "La reducción de la jornada semanal"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué puede constituir el incumplimiento reiterado del derecho a la desconexión laboral?",
            "options": [
              "Una falta administrativa menor sin consecuencias",
              "Una conducta de acoso laboral, según la propia Ley 2191 de 2022",
              "Un beneficio adicional para el trabajador",
              "Un motivo automático de despido"
            ],
            "correct": 1
          }
        ],
        "apply": "Si tu jefe te escribe fuera de horario por temas no urgentes, es válido responder al día siguiente. La Ley 2191 de 2022 respalda ese derecho."
      },
      {
        "key": "acoso_laboral",
        "title": "Acoso laboral",
        "intro": "El acoso laboral, definido por la Ley 1010 de 2006, es toda conducta persistente y demostrable ejercida sobre un trabajador para infundir miedo o desmotivarlo.",
        "points": [
          "Debe ser persistente y demostrable",
          "Busca infundir miedo, intimidación o desmotivación",
          "El comité es el primer canal interno de atención"
        ],
        "norm": "Ley 1010 de 2006",
        "questions": [
          {
            "q": "¿Qué ley define el acoso laboral en Colombia?",
            "options": [
              "Ley 1010 de 2006",
              "Ley 2191 de 2022",
              "Ley 1562 de 2012",
              "Ley 2466 de 2025"
            ],
            "correct": 0
          },
          {
            "q": "¿Qué característica debe tener una conducta para considerarse acoso laboral?",
            "options": [
              "Que ocurra una sola vez, sin importar la gravedad",
              "Que sea persistente y demostrable",
              "Que la denuncie un tercero ajeno a la empresa",
              "Que ocurra fuera del horario laboral"
            ],
            "correct": 1
          }
        ],
        "apply": "Si una conducta incómoda se repite semana tras semana con la misma persona, empieza a dejarla por escrito (fechas, hechos)."
      },
      {
        "key": "resolucion_conflictos",
        "title": "Resolución de conflictos",
        "intro": "No todo conflicto es acoso laboral: muchas veces es una diferencia normal que se resuelve con diálogo directo.",
        "points": [
          "No todo conflicto constituye acoso laboral",
          "El comité distingue entre conflicto puntual y conducta reiterada",
          "Cada caso requiere el mecanismo adecuado"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Todo conflicto laboral constituye acoso laboral?",
            "options": [
              "Sí, siempre que involucre a un jefe",
              "No, el acoso requiere una conducta persistente y demostrable",
              "Sí, según cualquier queja presentada",
              "No, el acoso laboral no existe legalmente en Colombia"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué debe distinguir el comité al recibir un caso?",
            "options": [
              "Nada, todos los casos se tratan igual",
              "Si es un conflicto puntual o una conducta reiterada",
              "El cargo de quien presenta la queja",
              "El género de las personas involucradas"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de escalar un roce con un compañero al Comité de Convivencia, intenta primero una conversación directa y respetuosa."
      },
      {
        "key": "violencia_genero_acoso_sexual",
        "title": "Violencia basada en género y acoso sexual laboral",
        "intro": "La violencia basada en género y el acoso sexual laboral son conductas graves que la empresa debe prevenir con protocolos claros.",
        "points": [
          "Requieren protocolos claros de prevención",
          "Los canales de denuncia deben proteger frente a represalias",
          "La Resolución 3461 y el Decreto 405 de 2025 refuerzan esta protección"
        ],
        "norm": "Resolución 3461 de 2025 y Decreto 405 de 2025",
        "questions": [
          {
            "q": "¿Qué debe garantizar la empresa a quien denuncia acoso sexual laboral?",
            "options": [
              "Confidencialidad únicamente si el denunciante lo solicita por escrito",
              "Protección frente a represalias",
              "Ninguna garantía adicional a la de cualquier queja",
              "Solo protección si la denuncia se comprueba"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué normas refuerzan la protección frente a represalias en casos de acoso sexual laboral?",
            "options": [
              "La Resolución 0312 de 2019 únicamente",
              "La Resolución 3461 de 2025 y el Decreto 405 de 2025",
              "La Ley 100 de 1993",
              "El Código de Comercio"
            ],
            "correct": 1
          }
        ],
        "apply": "Si conoces el protocolo de tu empresa contra el acoso sexual laboral, compártelo con quien lo necesite."
      },
      {
        "key": "ruta_atencion_quejas",
        "title": "Ruta de atención y trámite de quejas",
        "intro": "Toda queja que llega al comité debe seguir una ruta definida: recepción confidencial, escucha a las partes, búsqueda de solución y seguimiento.",
        "points": [
          "Recepción confidencial es el primer paso",
          "Se escucha a ambas partes antes de concluir",
          "Un trámite mal documentado debilita la confianza en el mecanismo"
        ],
        "norm": "Resolución 3461 de 2025",
        "questions": [
          {
            "q": "¿Cuál es el primer paso ante una queja que llega al Comité de Convivencia?",
            "options": [
              "Notificar de inmediato a toda la empresa",
              "Recibirla de forma confidencial y escuchar a las partes",
              "Rechazarla si no tiene pruebas documentales",
              "Remitirla directamente a un juzgado"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué debilita la confianza de los trabajadores en el mecanismo de quejas?",
            "options": [
              "Un trámite confidencial y bien documentado",
              "Un trámite mal documentado o sin confidencialidad",
              "Que el comité haga seguimiento a los casos",
              "Que existan actas de cada reunión"
            ],
            "correct": 1
          }
        ],
        "apply": "Si vas a presentar una queja al Comité de Convivencia, hazlo por el canal formal establecido, no de forma verbal e informal."
      }
    ]
  },
  "sst": {
    "label": "Seguridad y Salud en el Trabajo",
    "icon": "helmet",
    "desc": "SG-SST, riesgos laborales y prevención",
    "keywords": [
      "sst",
      "seguridad y salud en el trabajo",
      "seguridad y salud",
      "sgsst",
      "sg-sst",
      "sg sst",
      "salud ocupacional",
      "riesgos laborales",
      "seguridad laboral"
    ],
    "modules": [
      {
        "key": "epp",
        "title": "Qué son los EPP",
        "intro": "Los Elementos de Protección Personal (EPP) son la última barrera de defensa frente a un riesgo que no se pudo eliminar ni controlar de otra forma.",
        "points": [
          "Casco, guantes, gafas y protección auditiva, entre otros",
          "El empleador los suministra sin costo para el trabajador",
          "Son la última barrera, no la primera medida de control"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Quién debe asumir el costo de los EPP?",
            "options": [
              "El trabajador",
              "El empleador",
              "Únicamente la ARL",
              "Se divide entre trabajador y empleador"
            ],
            "correct": 1
          },
          {
            "q": "¿En qué lugar de la jerarquía de controles se ubican los EPP?",
            "options": [
              "Son la primera medida a aplicar",
              "Son la última barrera, cuando no se pudo eliminar ni controlar el riesgo de otra forma",
              "No forman parte de la jerarquía de controles",
              "Solo aplican en trabajos administrativos"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de empezar tu turno, revisa que tu EPP esté completo y en buen estado — un guante roto ya no te protege como debería."
      },
      {
        "key": "levantamiento_objetos",
        "title": "Levantamiento de objetos",
        "intro": "Levantar un objeto pesado con la técnica incorrecta es una de las principales causas de lesiones osteomusculares en el trabajo.",
        "points": [
          "Acercar la carga al cuerpo antes de levantarla",
          "Flexionar las piernas, no doblar la espalda",
          "Mantener la espalda recta durante todo el movimiento"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es la técnica correcta para levantar un objeto pesado?",
            "options": [
              "Doblar la espalda manteniendo las piernas rectas",
              "Acercar la carga al cuerpo, flexionar las piernas y mantener la espalda recta",
              "Levantar el objeto lo más rápido posible",
              "Girar el torso mientras se levanta la carga"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué causa frecuentemente el levantamiento incorrecto de cargas?",
            "options": [
              "Mejora en el rendimiento físico",
              "Lesiones osteomusculares",
              "Ahorro de tiempo sin ningún riesgo",
              "Ningún efecto relevante en el cuerpo"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que levantes algo pesado, detente un segundo: pies firmes, espalda recta, flexiona las piernas."
      },
      {
        "key": "estilos_vida_saludable",
        "title": "Estilos de vida saludable",
        "intro": "Una alimentación balanceada, actividad física regular, buen descanso y control del estrés reducen el riesgo de enfermedades y mejoran el desempeño laboral.",
        "points": [
          "Alimentación balanceada y actividad física regular",
          "Buen descanso y control del estrés",
          "El SG-SST promueve estos hábitos activamente"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué elementos hacen parte de un estilo de vida saludable en el trabajo?",
            "options": [
              "Solo dormir muchas horas",
              "Alimentación balanceada, actividad física, buen descanso y control del estrés",
              "Trabajar sin pausas para rendir más",
              "Evitar cualquier tipo de ejercicio"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué promueve el SG-SST respecto a los hábitos de vida de los trabajadores?",
            "options": [
              "No tiene relación con este tema",
              "Programas de estilo de vida y trabajo saludable",
              "Solo la reducción de personal",
              "Exclusivamente incentivos económicos"
            ],
            "correct": 1
          }
        ],
        "apply": "Elige hoy un solo hábito para mejorar —tomar más agua, caminar en el descanso— y sostenlo una semana."
      },
      {
        "key": "pausas_activas",
        "title": "Importancia de las pausas activas",
        "intro": "Las pausas activas son breves interrupciones de la jornada para estirar, cambiar de postura y descansar la vista.",
        "points": [
          "Duran pocos minutos pero se hacen con frecuencia",
          "Previenen la fatiga física y visual",
          "Reducen los desórdenes musculoesqueléticos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué previenen las pausas activas durante la jornada laboral?",
            "options": [
              "El aumento de salario",
              "La fatiga física y los desórdenes musculoesqueléticos",
              "Las reuniones de trabajo",
              "El uso del computador"
            ],
            "correct": 1
          },
          {
            "q": "¿En qué consisten las pausas activas?",
            "options": [
              "En dejar de trabajar toda la tarde",
              "En breves interrupciones para estirar, cambiar de postura y descansar la vista",
              "En cambiar de oficina cada hora",
              "En reuniones de retroalimentación"
            ],
            "correct": 1
          }
        ],
        "apply": "Programa una alarma cada dos horas para hacer una pausa activa de dos minutos. Tu cuerpo lo va a notar al final del día."
      },
      {
        "key": "caidas_niveles_alturas",
        "title": "Caídas a nivel, a diferente nivel y en alturas",
        "intro": "Una caída a nivel ocurre en el mismo plano; una a diferente nivel implica un desnivel; y el trabajo en alturas exige medidas específicas de protección.",
        "points": [
          "Caída a nivel: resbalones y tropiezos en el mismo plano",
          "Caída a diferente nivel: escaleras y rampas",
          "Trabajo en alturas desde 1.5 metros exige arnés y línea de vida"
        ],
        "norm": "Resolución 4272 de 2021 (trabajo seguro en alturas)",
        "questions": [
          {
            "q": "¿A partir de qué altura se considera trabajo en alturas en Colombia?",
            "options": [
              "1.0 metro",
              "1.5 metros",
              "3 metros",
              "5 metros"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué diferencia una caída a nivel de una caída a diferente nivel?",
            "options": [
              "No existe ninguna diferencia",
              "La caída a nivel ocurre en el mismo plano; la de diferente nivel implica un desnivel",
              "La caída a nivel es siempre más grave",
              "Solo la de diferente nivel requiere reporte"
            ],
            "correct": 1
          }
        ],
        "apply": "Si vas a subir una escalera o trabajar en un lugar elevado, revisa primero si el área está despejada y si tienes el equipo adecuado."
      },
      {
        "key": "primeros_auxilios_psicologicos",
        "title": "Primeros auxilios psicológicos",
        "intro": "Los primeros auxilios psicológicos son el apoyo inmediato que se brinda a una persona que atraviesa una crisis o un evento perturbador.",
        "points": [
          "Escuchar sin juzgar es el primer paso",
          "Brindar contención, no un diagnóstico",
          "Orientar hacia ayuda profesional si es necesario"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué son los primeros auxilios psicológicos?",
            "options": [
              "Un diagnóstico clínico inmediato",
              "Apoyo inmediato de escucha y contención a alguien en crisis, sin intentar diagnosticar",
              "Medicación de emergencia",
              "Una evaluación de desempeño laboral"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué NO debe hacer quien brinda primeros auxilios psicológicos?",
            "options": [
              "Escuchar sin juzgar",
              "Intentar dar un diagnóstico clínico",
              "Brindar contención",
              "Orientar hacia ayuda profesional"
            ],
            "correct": 1
          }
        ],
        "apply": "Si un compañero está pasando por un mal momento, a veces lo más útil es simplemente escuchar sin juzgar."
      },
      {
        "key": "riesgo_publico_agresion",
        "title": "Prevención del riesgo público y agresión en el trabajo",
        "intro": "El riesgo público incluye eventos como robos, atracos o agresiones de terceros durante la actividad laboral.",
        "points": [
          "Incluye robos, atracos y agresiones de terceros",
          "Evitar la confrontación directa es clave",
          "Reportar de inmediato protege la integridad de todos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué incluye el riesgo público en el ámbito laboral?",
            "options": [
              "Solo accidentes de tránsito",
              "Eventos como robos, atracos o agresiones de terceros",
              "Únicamente riesgos ambientales",
              "Solo riesgos relacionados con maquinaria"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué se recomienda evitar ante una situación de riesgo público?",
            "options": [
              "Reportar el incidente",
              "La confrontación directa",
              "Seguir el protocolo de la empresa",
              "Proteger la propia integridad"
            ],
            "correct": 1
          }
        ],
        "apply": "Si tu trabajo te expone a zonas de riesgo público, ten siempre presente la ruta de salida más cercana y evita confrontar directamente."
      },
      {
        "key": "identificacion_evaluacion_riesgos",
        "title": "Identificación y evaluación de riesgos",
        "intro": "Identificar un riesgo es reconocer una fuente de daño potencial; evaluarlo es determinar qué tan probable y grave sería ese daño.",
        "points": [
          "Identificar: reconocer la fuente de daño",
          "Evaluar: medir probabilidad y gravedad",
          "Debe involucrar a los propios trabajadores del puesto"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué es evaluar un riesgo?",
            "options": [
              "Eliminarlo por completo de inmediato",
              "Determinar qué tan probable y grave sería el daño que ese riesgo podría causar",
              "Reportarlo a la ARL sin más análisis",
              "Ignorarlo si nunca antes causó un accidente"
            ],
            "correct": 1
          },
          {
            "q": "¿Por qué es importante involucrar a los propios trabajadores en la identificación de riesgos?",
            "options": [
              "No es necesario involucrarlos",
              "Porque conocen su puesto de trabajo mejor que nadie",
              "Porque así se reduce el número de inspecciones",
              "Porque lo exige únicamente el área comercial"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que notes algo que 'siempre ha sido así' en tu puesto, pregúntate si realmente es seguro o si te acostumbraste al riesgo."
      },
      {
        "key": "prevencion_atel_sst",
        "title": "Estrategias para la prevención de ATEL",
        "intro": "Prevenir accidentes de trabajo y enfermedad laboral exige combinar inspecciones periódicas, reporte oportuno y capacitación constante.",
        "points": [
          "Inspecciones periódicas y mantenimiento de equipos",
          "Reporte oportuno de condiciones inseguras",
          "La prevención rara vez depende de una sola medida"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué combina una estrategia efectiva de prevención de ATEL?",
            "options": [
              "Solo el uso de EPP",
              "Inspecciones periódicas, reporte oportuno, mantenimiento y capacitación",
              "Únicamente sanciones a los trabajadores",
              "Solo la reducción de personal"
            ],
            "correct": 1
          },
          {
            "q": "¿La prevención efectiva de accidentes suele depender de una sola medida?",
            "options": [
              "Sí, basta con entregar EPP",
              "No, rara vez depende de una sola medida",
              "Sí, basta con una capacitación anual",
              "No es posible prevenir accidentes"
            ],
            "correct": 1
          }
        ],
        "apply": "Elige hoy una condición insegura que llevas tiempo posponiendo reportar, y repórtala."
      },
      {
        "key": "bienestar_emocional",
        "title": "Buenas prácticas para el bienestar emocional",
        "intro": "El bienestar emocional en el trabajo se fortalece con límites claros entre la vida laboral y personal, y relaciones respetuosas.",
        "points": [
          "Límites claros entre vida laboral y personal",
          "Reconocimiento del trabajo bien hecho",
          "Espacios para expresarse sin estigmatizar a quien pide ayuda"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué fortalece el bienestar emocional en el trabajo?",
            "options": [
              "Eliminar cualquier límite entre vida laboral y personal",
              "Límites claros, relaciones respetuosas y reconocimiento del trabajo bien hecho",
              "Evitar cualquier retroalimentación",
              "Aumentar la carga laboral sin pausas"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué actitud debe evitarse frente a alguien que pide ayuda emocional en el trabajo?",
            "options": [
              "Escucharlo con respeto",
              "Estigmatizarlo",
              "Orientarlo a un profesional si es necesario",
              "Ofrecer un espacio de conversación"
            ],
            "correct": 1
          }
        ],
        "apply": "Al final del día, pregúntate honestamente cómo te sientes, no solo qué tareas cumpliste."
      },
      {
        "key": "maquinas_herramientas",
        "title": "Utilización de máquinas y herramientas",
        "intro": "Usar una máquina o herramienta sin conocer sus riesgos o sin la capacitación adecuada es una de las causas más frecuentes de accidentes graves.",
        "points": [
          "Verificar siempre el buen estado antes de usarla",
          "Las guardas de seguridad deben estar instaladas",
          "Requiere capacitación específica para cada equipo"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué se debe verificar antes de operar una máquina o herramienta?",
            "options": [
              "Solo que esté encendida",
              "Que esté en buen estado y contar con la capacitación adecuada",
              "Que otro compañero la haya usado antes",
              "Nada, si la tarea es urgente"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué elemento de seguridad debe estar siempre instalado en una máquina?",
            "options": [
              "Las guardas de seguridad",
              "Un adhesivo publicitario",
              "Un contador de horas de uso únicamente",
              "Ninguno, basta con la experiencia del operario"
            ],
            "correct": 0
          }
        ],
        "apply": "Antes de usar una herramienta que no manejas seguido, revisa que tenga sus guardas de seguridad puestas."
      },
      {
        "key": "sustancias_psicoactivas",
        "title": "Consumo de sustancias psicoactivas",
        "intro": "El consumo de alcohol o sustancias psicoactivas afecta la atención, el equilibrio y el tiempo de reacción, elevando drásticamente el riesgo de accidente.",
        "points": [
          "Afecta atención, equilibrio y tiempo de reacción",
          "La empresa debe tener una política clara al respecto",
          "El enfoque debe ser preventivo, no estigmatizante"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué efecto tiene el consumo de sustancias psicoactivas en el trabajo?",
            "options": [
              "Ningún efecto relevante en tareas de oficina",
              "Afecta la atención, el equilibrio y el tiempo de reacción, aumentando el riesgo de accidente",
              "Solo afecta el rendimiento, no la seguridad",
              "Mejora la concentración a corto plazo"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuál debe ser el enfoque de la política empresarial frente al consumo de sustancias psicoactivas?",
            "options": [
              "Estigmatizar a quien consume",
              "Prevención, sin estigmatizar a quien busca ayuda",
              "Ignorar el tema por completo",
              "Sancionar sin ofrecer ningún apoyo"
            ],
            "correct": 1
          }
        ],
        "apply": "Si sabes que un compañero está lidiando con un problema de consumo, la mejor ayuda es orientarlo hacia los canales de apoyo de la empresa."
      }
    ]
  },
  "brigada": {
    "label": "Brigada de Emergencia",
    "icon": "fire",
    "desc": "Respuesta ante emergencias y primeros auxilios",
    "keywords": [
      "brigada",
      "brigada de emergencia",
      "emergencia",
      "primeros auxilios",
      "evacuacion",
      "evacuación",
      "incendio",
      "extintor"
    ],
    "modules": [
      {
        "key": "plan_emergencia",
        "title": "Plan de emergencia",
        "intro": "El plan de emergencia define cómo debe actuar la empresa ante un evento que ponga en riesgo a las personas o las instalaciones.",
        "points": [
          "Define qué hacer, quién lo hace y en qué orden",
          "Es obligatorio para toda empresa",
          "Incluye prevención, preparación y respuesta"
        ],
        "norm": "Decreto 1072 de 2015",
        "questions": [
          {
            "q": "¿Qué documento define cómo debe actuar la empresa ante una emergencia?",
            "options": [
              "El reglamento interno de trabajo",
              "El plan de emergencia",
              "La matriz de peligros",
              "El manual de funciones"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué exige el Decreto 1072 de 2015 en materia de emergencias?",
            "options": [
              "Nada, es opcional",
              "Que toda empresa cuente con un plan de prevención, preparación y respuesta",
              "Que solo las empresas grandes tengan un plan",
              "Que el plan lo diseñe exclusivamente la ARL"
            ],
            "correct": 1
          }
        ],
        "apply": "Ubica hoy mismo dónde está publicado el plan de emergencia de tu área y revisa cuál es tu punto de encuentro asignado."
      },
      {
        "key": "roles_brigada",
        "title": "Roles y responsabilidades de la brigada",
        "intro": "Cada brigadista tiene un rol definido según su formación: control de incendios, primeros auxilios, evacuación o comunicaciones.",
        "points": [
          "Cada rol requiere formación específica",
          "Roles claros evitan tareas duplicadas o descubiertas",
          "La coordinación es clave en una emergencia real"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Por qué es importante que cada brigadista tenga un rol claramente definido?",
            "options": [
              "Para que todos hagan exactamente lo mismo",
              "Para evitar que dos personas hagan lo mismo mientras otra tarea queda sin cubrir",
              "Porque lo exige el área de recursos humanos",
              "No es importante, cualquiera puede hacer cualquier tarea"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuáles son ejemplos de roles dentro de una brigada de emergencia?",
            "options": [
              "Solo el rol de vocero de prensa",
              "Control de incendios, primeros auxilios, evacuación y comunicaciones",
              "Únicamente contabilidad",
              "Solo atención al cliente"
            ],
            "correct": 1
          }
        ],
        "apply": "Si eres brigadista, ten claro tu rol específico y practica mentalmente qué harías en los primeros 60 segundos de una emergencia."
      },
      {
        "key": "cadena_supervivencia",
        "title": "Cadena de supervivencia y primer respondiente",
        "intro": "La cadena de supervivencia describe los pasos que aumentan la posibilidad de que una persona sobreviva a una emergencia médica.",
        "points": [
          "Reconocimiento temprano y alerta oportuna",
          "Reanimación básica antes de la atención especializada",
          "El primer respondiente actúa en los primeros minutos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué es el primer respondiente en una emergencia médica?",
            "options": [
              "El paramédico que llega al final",
              "Quien actúa en los primeros minutos, antes de que lleguen los organismos de socorro",
              "Solo el médico de la EPS",
              "Un cargo administrativo de la empresa"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuáles son pasos de la cadena de supervivencia?",
            "options": [
              "Solo llamar a la EPS",
              "Reconocimiento temprano, alerta oportuna, reanimación básica y atención especializada",
              "Esperar sin actuar hasta que llegue una ambulancia",
              "Documentar el incidente únicamente"
            ],
            "correct": 1
          }
        ],
        "apply": "Aprende a reconocer las señales básicas de una emergencia médica — ser el primero en notarlo puede ganar minutos que salvan una vida."
      },
      {
        "key": "extintores_camilla_botiquin",
        "title": "Manejo de extintores, camilla y botiquín",
        "intro": "Usar un extintor sigue el método PASS. Movilizar a un lesionado en camilla exige inmovilización previa y coordinación entre brigadistas.",
        "points": [
          "PASS: halar, apuntar, presionar y mover en zigzag",
          "La camilla requiere inmovilización previa",
          "El botiquín debe estar dotado, vigente y accesible"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué significa la sigla PASS para el uso de extintores?",
            "options": [
              "Prevenir, Actuar, Salir, Señalizar",
              "Halar el pasador, Apuntar a la base del fuego, presionar la palanca (Squeeze) y mover en zigzag (Sweep)",
              "Parar, Alertar, Suspender, Salir",
              "Preparar, Asegurar, Supervisar, Sofocar"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué se requiere antes de movilizar a un lesionado en camilla?",
            "options": [
              "Nada, se puede mover de inmediato",
              "Inmovilización previa y coordinación entre varios brigadistas",
              "Solo la autorización del jefe de área",
              "Esperar 24 horas"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que pases cerca de un extintor, ubica su ficha técnica y confirma para qué tipo de fuego sirve."
      },
      {
        "key": "evacuacion",
        "title": "Evacuación",
        "intro": "Evacuar es desplazar de forma ordenada a las personas de una zona de riesgo hacia un lugar seguro.",
        "points": [
          "Requiere rutas señalizadas y puntos de encuentro definidos",
          "Se debe verificar que nadie quede atrás",
          "Atención especial a personas con movilidad reducida"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué se requiere para una evacuación ordenada?",
            "options": [
              "Solo correr hacia la salida más cercana",
              "Rutas señalizadas, puntos de encuentro definidos y verificación de que nadie quede atrás",
              "Usar siempre el ascensor",
              "No es necesario ningún tipo de organización"
            ],
            "correct": 1
          },
          {
            "q": "¿A quién se debe prestar especial atención durante una evacuación?",
            "options": [
              "A nadie en particular",
              "A las personas con movilidad reducida",
              "Solo a los visitantes",
              "Solo al personal directivo"
            ],
            "correct": 1
          }
        ],
        "apply": "Camina hoy, aunque sea mentalmente, la ruta de evacuación más cercana a tu puesto hasta el punto de encuentro."
      },
      {
        "key": "alerta_alarma",
        "title": "Sistema de alerta y alarma",
        "intro": "La alerta informa que existe una situación de riesgo; la alarma indica que se debe actuar de inmediato, generalmente iniciando la evacuación.",
        "points": [
          "La alerta informa del riesgo",
          "La alarma exige actuar de inmediato",
          "Todos deben reconocer la señal de su empresa"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es la diferencia entre alerta y alarma?",
            "options": [
              "Son sinónimos, no hay diferencia",
              "La alerta informa del riesgo; la alarma indica que se debe actuar de inmediato",
              "La alarma es solo sonora y la alerta solo visual",
              "La alerta la activa el brigadista y la alarma el trabajador"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué debe saber todo trabajador respecto a la alarma de su empresa?",
            "options": [
              "No necesita reconocerla",
              "Reconocer la señal y saber qué hacer al escucharla",
              "Solo el personal de seguridad debe conocerla",
              "Es información confidencial"
            ],
            "correct": 1
          }
        ],
        "apply": "Asegúrate de reconocer el sonido exacto de la alarma de tu empresa antes de que ocurra una emergencia real."
      },
      {
        "key": "incendios",
        "title": "Incendios",
        "intro": "El fuego necesita tres elementos para existir: combustible, oxígeno y calor. Eliminar cualquiera de los tres lo apaga.",
        "points": [
          "Combustible, oxígeno y calor: el triángulo del fuego",
          "Eliminar un elemento apaga el fuego",
          "Conocer el tipo de fuego evita elegir el extintor equivocado"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuáles son los tres elementos del triángulo del fuego?",
            "options": [
              "Agua, tierra y aire",
              "Combustible, oxígeno y calor",
              "Humo, calor y presión",
              "Chispa, viento y madera"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué ocurre si se elimina uno de los tres elementos del triángulo del fuego?",
            "options": [
              "El fuego se intensifica",
              "El fuego se apaga",
              "No pasa nada",
              "El fuego cambia de color únicamente"
            ],
            "correct": 1
          }
        ],
        "apply": "Si ves un principio de incendio pequeño, usa el extintor correcto de inmediato; si crece rápido, evacúa y da la alerta."
      },
      {
        "key": "analisis_vulnerabilidad",
        "title": "Análisis de vulnerabilidad",
        "intro": "El análisis de vulnerabilidad identifica qué tan expuesta está la empresa ante distintas amenazas y qué tan preparada está para responder.",
        "points": [
          "Evalúa amenazas como incendio, sismo o inundación",
          "Mide el nivel de preparación de la empresa",
          "Es la base técnica del plan de emergencias"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué evalúa el análisis de vulnerabilidad?",
            "options": [
              "El presupuesto anual de la brigada",
              "Qué tan expuesta está la empresa ante distintas amenazas y qué tan preparada está para responder",
              "El número de extintores instalados únicamente",
              "La antigüedad de la infraestructura"
            ],
            "correct": 1
          },
          {
            "q": "¿Sobre qué se construye el plan de emergencias de una empresa?",
            "options": [
              "Sobre el análisis de vulnerabilidad",
              "Sobre el presupuesto de marketing",
              "Sobre el manual de calidad",
              "Sobre la política de vacaciones"
            ],
            "correct": 0
          }
        ],
        "apply": "Piensa en la amenaza más probable para tu sede y pregúntate si sabes cómo debe actuar tu área frente a ella."
      },
      {
        "key": "primeros_auxilios_brigada",
        "title": "Primeros auxilios",
        "intro": "Los primeros auxilios son la atención inmediata que se brinda a una persona lesionada o enferma antes de que llegue ayuda profesional.",
        "points": [
          "Su objetivo es preservar la vida",
          "Buscan evitar que la condición empeore",
          "Se aplican dentro de los límites de la formación del brigadista"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es el objetivo principal de los primeros auxilios?",
            "options": [
              "Reemplazar la atención médica profesional",
              "Preservar la vida y evitar que la condición del lesionado empeore",
              "Diagnosticar la lesión con precisión",
              "Trasladar siempre al lesionado por cuenta propia"
            ],
            "correct": 1
          },
          {
            "q": "¿Dentro de qué límites debe actuar un brigadista al dar primeros auxilios?",
            "options": [
              "Sin ningún límite, puede actuar como médico",
              "Dentro de los límites de su propia formación",
              "Solo si tiene autorización escrita de la gerencia",
              "Únicamente si hay un médico presente"
            ],
            "correct": 1
          }
        ],
        "apply": "Si presencias una lesión: garantiza tu propia seguridad, actúa dentro de lo que sabes hacer, y activa la cadena de ayuda de inmediato."
      },
      {
        "key": "simulacros",
        "title": "Simulacros",
        "intro": "Un simulacro pone a prueba, en condiciones controladas, si el plan de emergencias realmente funciona.",
        "points": [
          "Evalúa si las rutas de evacuación son suficientes",
          "Verifica que la alarma se escuche en todas las áreas",
          "Sin simulacros periódicos, el plan es solo teoría"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Para qué sirve un simulacro?",
            "options": [
              "Para cumplir un requisito sin analizar resultados",
              "Para poner a prueba si el plan de emergencias realmente funciona en la práctica",
              "Para evaluar el desempeño individual de cada empleado",
              "Para reemplazar la señalización de evacuación"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué ocurre con un plan de emergencias que nunca se pone a prueba con simulacros?",
            "options": [
              "Sigue siendo igual de efectivo",
              "Se queda solo en teoría, sin saber si realmente funciona",
              "Mejora automáticamente con el tiempo",
              "No requiere ningún ajuste"
            ],
            "correct": 1
          }
        ],
        "apply": "En el próximo simulacro, participa como si fuera real — cronometra tu propio tiempo hasta el punto de encuentro."
      },
      {
        "key": "pon",
        "title": "Procedimientos Operativos Normalizados (PON)",
        "intro": "Los Procedimientos Operativos Normalizados son instrucciones paso a paso para actuar frente a un tipo específico de emergencia.",
        "points": [
          "Existe uno para cada tipo de emergencia",
          "Evitan que la respuesta dependa de la improvisación",
          "Deben ser conocidos por todos los brigadistas"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué son los Procedimientos Operativos Normalizados (PON)?",
            "options": [
              "Los turnos de trabajo de la brigada",
              "Instrucciones paso a paso para actuar frente a un tipo específico de emergencia",
              "El inventario de equipos contra incendio",
              "El acta de conformación de la brigada"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué evitan los PON en una emergencia real?",
            "options": [
              "Que la respuesta dependa de la improvisación de quien esté presente",
              "Que se necesite un plan de emergencias",
              "La necesidad de brigadistas capacitados",
              "El uso de extintores"
            ],
            "correct": 0
          }
        ],
        "apply": "Pregunta si existe un Procedimiento Operativo Normalizado para el tipo de emergencia más probable en tu área."
      },
      {
        "key": "clasificacion_niveles_emergencia",
        "title": "Clasificación y niveles de emergencia",
        "intro": "No todas las emergencias tienen la misma magnitud: se clasifican según su gravedad y el alcance de la respuesta que requieren.",
        "points": [
          "Van desde un conato hasta una emergencia mayor",
          "El nivel determina el alcance de la respuesta",
          "Una emergencia mayor exige apoyo de organismos externos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Según qué se clasifican los niveles de una emergencia?",
            "options": [
              "Según el número de brigadistas disponibles ese día",
              "Según su gravedad y el alcance de la respuesta que requieren",
              "Según la hora del día en que ocurre",
              "Según el clima"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué tipo de emergencia exige la intervención de organismos externos de socorro?",
            "options": [
              "Un conato controlable por la propia brigada",
              "Una emergencia mayor",
              "Ninguna emergencia requiere apoyo externo",
              "Solo las emergencias nocturnas"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de reaccionar, evalúa rápido la magnitud: ¿la puede controlar la brigada, o requiere ayuda externa de inmediato?"
      }
    ]
  },
  "ambiental": {
    "label": "Gestión Ambiental",
    "icon": "leaf",
    "desc": "Cuidado ambiental, residuos y buenas prácticas",
    "keywords": [
      "ambiental",
      "medio ambiente",
      "ambiente",
      "sga",
      "gestion ambiental",
      "gestión ambiental",
      "residuos",
      "reciclaje"
    ],
    "modules": [
      {
        "key": "aspectos_impactos",
        "title": "Aspectos e impactos ambientales",
        "intro": "Un aspecto ambiental es cualquier elemento de las actividades de la empresa que puede interactuar con el entorno; el impacto es el cambio que produce.",
        "points": [
          "El aspecto es la actividad; el impacto es el efecto",
          "Puede ser positivo o negativo",
          "Es el punto de partida de toda gestión ambiental"
        ],
        "norm": "Ley 99 de 1993 y Decreto 1076 de 2015",
        "questions": [
          {
            "q": "¿Qué es un aspecto ambiental?",
            "options": [
              "Una sanción de la autoridad ambiental",
              "Un elemento de las actividades de la empresa que puede interactuar con el ambiente",
              "El logotipo del sistema de gestión ambiental",
              "Un tipo específico de residuo peligroso"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué es un impacto ambiental?",
            "options": [
              "Un tipo de multa que impone la autoridad ambiental",
              "El cambio que se produce en el ambiente como resultado de un aspecto ambiental",
              "El nombre del comité ambiental de la empresa",
              "Un documento exigido únicamente a la industria pesada"
            ],
            "correct": 1
          }
        ],
        "apply": "Identifica un aspecto ambiental de tu propio puesto (el papel que usas, la energía que consumes) y piensa en una acción para reducir su impacto."
      },
      {
        "key": "ahorro_energia",
        "title": "Ahorro de energía",
        "intro": "Apagar luces y equipos que no se están usando, y aprovechar la luz natural, son medidas simples que reducen el consumo energético.",
        "points": [
          "Apagar lo que no se está usando",
          "Aprovechar la luz natural cuando sea posible",
          "Mantener los equipos en buen estado"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es una buena práctica de ahorro de energía?",
            "options": [
              "Dejar los equipos encendidos por si se necesitan luego",
              "Apagar luces y equipos que no se están usando",
              "Usar siempre luz artificial, incluso de día",
              "Aumentar la potencia de todos los equipos"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué relación existe entre el ahorro de energía y el impacto ambiental?",
            "options": [
              "Ninguna relación",
              "Reducir el consumo energético reduce el impacto ambiental de la operación",
              "El ahorro de energía aumenta el impacto ambiental",
              "Solo aplica a empresas industriales"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de salir de tu puesto hoy, revisa: ¿dejaste encendido algo que no necesitas?"
      },
      {
        "key": "fuentes_hidricas",
        "title": "Cuidado y protección de las fuentes hídricas",
        "intro": "Ríos, quebradas y nacimientos de agua son ecosistemas frágiles que la actividad empresarial puede afectar mediante vertimientos o consumo excesivo.",
        "points": [
          "Evitar el vertimiento de sustancias no autorizadas",
          "Usar el agua de forma responsable",
          "Son ecosistemas frágiles ante la actividad empresarial"
        ],
        "norm": "Decreto 1076 de 2015",
        "questions": [
          {
            "q": "¿Cómo puede afectar una empresa a una fuente hídrica?",
            "options": [
              "Solo mediante publicidad",
              "Mediante vertimientos no autorizados o consumo excesivo de agua",
              "No es posible que una empresa afecte una fuente hídrica",
              "Únicamente a través de sus proveedores"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué norma enmarca la protección de las fuentes hídricas en Colombia?",
            "options": [
              "El Código Sustantivo del Trabajo",
              "El Decreto 1076 de 2015",
              "La Ley 1010 de 2006",
              "La Resolución 40595 de 2022"
            ],
            "correct": 1
          }
        ],
        "apply": "Si tu trabajo involucra líquidos o químicos, verifica siempre dónde y cómo se desechan — nunca por un desagüe común sin autorización."
      },
      {
        "key": "importancia_cuidado_ambiente",
        "title": "Importancia y cuidado del medio ambiente",
        "intro": "El cuidado del medio ambiente no es solo una obligación legal: garantiza recursos naturales para las generaciones futuras.",
        "points": [
          "Garantiza recursos para el futuro",
          "Reduce riesgos sanitarios y económicos",
          "Es un derecho reconocido por la Constitución de 1991"
        ],
        "norm": "Constitución Política de 1991",
        "questions": [
          {
            "q": "¿Qué reconoce la Constitución Política de 1991 en materia ambiental?",
            "options": [
              "Ningún derecho relacionado con el ambiente",
              "El derecho de toda persona a gozar de un ambiente sano",
              "Solo obligaciones para las empresas grandes",
              "El derecho exclusivo del Estado sobre los recursos naturales"
            ],
            "correct": 1
          },
          {
            "q": "¿Por qué cuidar el medio ambiente no es solo una obligación legal para una empresa?",
            "options": [
              "Porque no tiene ningún beneficio adicional",
              "Porque también reduce riesgos sanitarios y económicos para la propia empresa",
              "Porque solo aplica a empresas exportadoras",
              "Porque es un tema exclusivamente publicitario"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que evalúes una decisión operativa, pregúntate no solo si es rentable, sino si es ambientalmente responsable."
      },
      {
        "key": "inventario_quimicos",
        "title": "Inventario de productos químicos",
        "intro": "Tener un inventario actualizado de todos los productos químicos que entran a la empresa permite conocer sus riesgos y planear su almacenamiento.",
        "points": [
          "Debe incluir la ficha de datos de seguridad (FDS)",
          "Permite planear el almacenamiento correcto",
          "Facilita la reacción ante una emergencia con químicos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué documento describe los riesgos de un producto químico?",
            "options": [
              "El manual de funciones",
              "La ficha de datos de seguridad (FDS)",
              "El plan de saneamiento básico",
              "El certificado de calidad del proveedor"
            ],
            "correct": 1
          },
          {
            "q": "¿Para qué sirve un inventario actualizado de productos químicos?",
            "options": [
              "Solo para fines contables",
              "Para conocer sus riesgos y planear su almacenamiento correcto",
              "Para calcular el precio de venta",
              "No tiene ninguna utilidad práctica"
            ],
            "correct": 1
          }
        ],
        "apply": "Si usas algún producto químico en tu labor, confirma que tienes acceso a su ficha de datos de seguridad."
      },
      {
        "key": "manejo_desechos",
        "title": "Manejo de desechos",
        "intro": "El manejo adecuado de los desechos incluye su clasificación, almacenamiento temporal correcto y disposición final por gestores autorizados.",
        "points": [
          "Clasificación, almacenamiento y disposición final",
          "Los residuos peligrosos requieren gestores autorizados",
          "No deben mezclarse con los residuos comunes"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué incluye el manejo adecuado de desechos?",
            "options": [
              "Solo botarlos en cualquier caneca",
              "Clasificación, almacenamiento temporal correcto y disposición final por gestores autorizados",
              "Quemarlos dentro de la empresa",
              "Ignorarlos si son en pequeña cantidad"
            ],
            "correct": 1
          },
          {
            "q": "¿Pueden mezclarse los residuos peligrosos con los residuos comunes?",
            "options": [
              "Sí, siempre que sea poca cantidad",
              "No, requieren manejo y disposición separados",
              "Sí, no hay ninguna restricción",
              "Solo si el residuo es líquido"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de botar un residuo, pregúntate: ¿es peligroso? Si no estás seguro, no lo mezcles con la basura común."
      },
      {
        "key": "saneamiento_basico",
        "title": "Plan de saneamiento básico",
        "intro": "El plan de saneamiento básico organiza las actividades de limpieza, control de plagas y manejo de residuos de un lugar de trabajo.",
        "points": [
          "Incluye limpieza y desinfección",
          "Incluye control de plagas",
          "Previene riesgos sanitarios para empleados y visitantes"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué busca un plan de saneamiento básico?",
            "options": [
              "Aumentar la producción de la empresa",
              "Prevenir riesgos sanitarios mediante limpieza, control de plagas y manejo de residuos",
              "Reemplazar el sistema de gestión ambiental",
              "Certificar la calidad del producto final"
            ],
            "correct": 1
          },
          {
            "q": "¿A quiénes protege el plan de saneamiento básico?",
            "options": [
              "Solo a los directivos de la empresa",
              "A empleados y visitantes",
              "Únicamente a los proveedores",
              "A nadie en particular"
            ],
            "correct": 1
          }
        ],
        "apply": "Si notas una condición de aseo deficiente en tu área, repórtala — el saneamiento básico previene enfermedades."
      },
      {
        "key": "programa_plagas",
        "title": "Programa integral de plagas",
        "intro": "Un programa integral de manejo de plagas combina medidas preventivas con controles químicos o biológicos aplicados por personal autorizado.",
        "points": [
          "Combina prevención con control químico o biológico",
          "El control lo aplica personal autorizado",
          "Evita el uso indiscriminado de plaguicidas"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué combina un programa integral de manejo de plagas?",
            "options": [
              "Solo el uso constante de plaguicidas",
              "Medidas preventivas con controles químicos o biológicos aplicados por personal autorizado",
              "Únicamente trampas mecánicas",
              "No requiere ninguna planificación"
            ],
            "correct": 1
          },
          {
            "q": "¿Quién debe aplicar los controles químicos o biológicos de un programa de plagas?",
            "options": [
              "Cualquier trabajador disponible",
              "Personal autorizado",
              "Solo el gerente general",
              "No requiere ninguna autorización"
            ],
            "correct": 1
          }
        ],
        "apply": "Si detectas señales de plagas en tu área, repórtalo de inmediato en lugar de intentar resolverlo con productos caseros."
      },
      {
        "key": "rotulacion_quimicos",
        "title": "Rotulación de productos químicos",
        "intro": "Todo producto químico debe estar correctamente rotulado, indicando su identidad, los pictogramas de peligro y las precauciones de manejo.",
        "points": [
          "Debe indicar identidad y pictogramas de peligro",
          "Incluye precauciones de manejo",
          "Un envase sin rótulo es un riesgo oculto"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué debe tener todo envase de producto químico?",
            "options": [
              "Solo el nombre comercial del producto",
              "Un rótulo con su identidad, pictogramas de peligro y precauciones de manejo",
              "Ninguna identificación si el envase es pequeño",
              "Solo el color del líquido que contiene"
            ],
            "correct": 1
          },
          {
            "q": "¿Por qué un envase sin rótulo es un riesgo oculto?",
            "options": [
              "Porque no afecta la seguridad en ningún caso",
              "Porque no permite conocer sus riesgos ni actuar correctamente ante una emergencia",
              "Porque solo afecta la estética del lugar",
              "Porque encarece el producto"
            ],
            "correct": 1
          }
        ],
        "apply": "Si encuentras un envase con líquido sin etiqueta, no asumas qué contiene ni lo uses — repórtalo."
      },
      {
        "key": "sensibilizacion_ambiental",
        "title": "Sensibilización ambiental",
        "intro": "Sensibilizar es generar conciencia sobre el impacto que las actividades diarias tienen en el entorno.",
        "points": [
          "Busca generar conciencia real, no solo cumplir una norma",
          "Convierte el cuidado ambiental en un hábito genuino",
          "Es una tarea continua, no un evento único"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es el objetivo de la sensibilización ambiental?",
            "options": [
              "Cumplir un indicador sin cambiar comportamientos",
              "Generar conciencia para que el cuidado ambiental se vuelva un hábito genuino",
              "Reducir el personal del área ambiental",
              "Aumentar el consumo de recursos naturales"
            ],
            "correct": 1
          },
          {
            "q": "¿La sensibilización ambiental debe ser un evento único o un proceso continuo?",
            "options": [
              "Un evento único al año",
              "Un proceso continuo",
              "No es necesaria en ningún caso",
              "Solo aplica una vez en la vida de la empresa"
            ],
            "correct": 1
          }
        ],
        "apply": "Elige un hábito ambiental que puedas mantener esta semana y compártelo con un compañero."
      },
      {
        "key": "separacion_residuos",
        "title": "Separación de residuos",
        "intro": "En Colombia, el código de colores nacional establece: blanco para aprovechables, verde para orgánicos aprovechables, y negro para no aprovechables.",
        "points": [
          "Blanco: plástico, papel, cartón, vidrio, metal",
          "Verde: residuos orgánicos aprovechables",
          "Negro: residuos no aprovechables"
        ],
        "norm": "Resolución 2184 de 2019",
        "questions": [
          {
            "q": "Según la Resolución 2184 de 2019, ¿qué color corresponde a los residuos orgánicos aprovechables?",
            "options": [
              "Blanco",
              "Verde",
              "Negro",
              "Rojo"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué color corresponde a los residuos aprovechables como plástico, papel y vidrio?",
            "options": [
              "Blanco",
              "Verde",
              "Negro",
              "Azul"
            ],
            "correct": 0
          }
        ],
        "apply": "La próxima vez que vayas a botar algo, tómate tres segundos para pensar en qué caneca va: blanca, verde o negra."
      },
      {
        "key": "uso_eficiente_agua",
        "title": "Uso eficiente del agua",
        "intro": "Cerrar la llave mientras se enjabona las manos y reportar de inmediato cualquier fuga son acciones simples que generan un ahorro real.",
        "points": [
          "Cerrar la llave mientras se enjabona las manos",
          "Reportar de inmediato cualquier fuga",
          "Multiplicado por todos, el ahorro es real"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es una buena práctica para el uso eficiente del agua?",
            "options": [
              "Dejar las llaves abiertas mientras se enjabona las manos",
              "Cerrar la llave mientras se enjabona las manos y reportar fugas",
              "Usar agua embotellada para todas las tareas de aseo",
              "No es necesario cuidar el agua en oficinas"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué se debe hacer al detectar una fuga de agua?",
            "options": [
              "Ignorarla si es pequeña",
              "Reportarla de inmediato",
              "Esperar a que alguien más la reporte",
              "Repararla sin avisar a nadie"
            ],
            "correct": 1
          }
        ],
        "apply": "Si ves una llave goteando, repórtala el mismo día — una fuga pequeña ignorada por meses representa un desperdicio enorme."
      }
    ]
  },
  "pesv": {
    "label": "Plan Estratégico de Seguridad Vial",
    "icon": "wheel",
    "desc": "Prevención vial y conducción segura",
    "keywords": [
      "pesv",
      "seguridad vial",
      "plan estrategico de seguridad vial",
      "plan estratégico de seguridad vial",
      "plan de seguridad vial",
      "transito",
      "tránsito",
      "conduccion",
      "conducción"
    ],
    "modules": [
      {
        "key": "peatones_motociclistas",
        "title": "Seguridad vial para peatones y motociclistas",
        "intro": "El peatón debe cruzar por zonas señalizadas y mantenerse visible; el motociclista debe usar casco certificado y chaleco reflectivo.",
        "points": [
          "El peatón cruza por zonas señalizadas",
          "El motociclista usa casco certificado y chaleco reflectivo",
          "Ambos son actores viales vulnerables"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué debe usar siempre un motociclista, además del casco certificado?",
            "options": [
              "Guantes de cuero exclusivamente",
              "Chaleco reflectivo",
              "Gafas de sol oscuras",
              "Ninguna otra protección es necesaria"
            ],
            "correct": 1
          },
          {
            "q": "¿Por qué se considera al peatón y al motociclista actores viales vulnerables?",
            "options": [
              "Porque tienen mayor riesgo de lesión grave frente a un vehículo más grande",
              "Porque no deben respetar las señales de tránsito",
              "Porque no pueden circular por la vía pública",
              "Porque no aplican normas de seguridad vial para ellos"
            ],
            "correct": 0
          }
        ],
        "apply": "Si eres motociclista, revisa hoy mismo que tu casco esté certificado y en buen estado."
      },
      {
        "key": "prevencion_at",
        "title": "Prevención de accidentes de tránsito",
        "intro": "La mayoría de los accidentes de tránsito son evitables con revisión del vehículo, respeto a las normas y planeación del recorrido.",
        "points": [
          "Revisar el vehículo antes de salir",
          "Respetar las normas de tránsito",
          "Planear el recorrido con tiempo suficiente"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué reduce significativamente la probabilidad de un siniestro vial?",
            "options": [
              "Conducir sin revisar el vehículo",
              "Revisar el vehículo, respetar las normas y planear el recorrido con tiempo",
              "Salir siempre con prisa",
              "Ignorar las señales de tránsito"
            ],
            "correct": 1
          },
          {
            "q": "¿La mayoría de los accidentes de tránsito son evitables?",
            "options": [
              "No, son siempre impredecibles",
              "Sí, la mayoría son evitables con medidas de prevención básicas",
              "Solo los que ocurren de noche son evitables",
              "Solo aplica a conductores profesionales"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de salir a manejar, dedica un minuto a revisar tu vehículo (luces, llantas, espejos)."
      },
      {
        "key": "actuacion_accidente",
        "title": "Actuación ante un accidente de tránsito",
        "intro": "Ante un accidente, la prioridad es garantizar la propia seguridad, señalizar la zona y alertar a las líneas de emergencia.",
        "points": [
          "Garantizar la propia seguridad primero",
          "Señalizar la zona para evitar un segundo accidente",
          "No mover a un lesionado salvo riesgo inminente"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué se debe hacer primero al presenciar un accidente de tránsito?",
            "options": [
              "Mover a los heridos de inmediato",
              "Señalizar la zona, garantizar la propia seguridad y alertar a las líneas de emergencia",
              "Retirarse del lugar",
              "Discutir la responsabilidad con la otra parte"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuándo se debe mover a una persona lesionada en un accidente de tránsito?",
            "options": [
              "Siempre, de inmediato",
              "Solo si existe un riesgo inminente para su vida",
              "Nunca, bajo ninguna circunstancia",
              "Solo si lo pide la persona lesionada"
            ],
            "correct": 1
          }
        ],
        "apply": "Guarda en tu vehículo, de forma visible, los números de las líneas de emergencia."
      },
      {
        "key": "socializacion_pesv",
        "title": "Socialización del PESV y sus pasos",
        "intro": "El PESV se construye siguiendo la metodología definida por el Ministerio de Transporte, y debe socializarse con todos los trabajadores.",
        "points": [
          "Sigue una metodología oficial de pasos",
          "Debe socializarse con todos los trabajadores",
          "No es solo un requisito documental"
        ],
        "norm": "Resolución 40595 de 2022",
        "questions": [
          {
            "q": "¿Por qué es importante socializar el PESV con todos los trabajadores?",
            "options": [
              "Para que lo conozcan y lo apliquen, no solo para cumplir un requisito documental",
              "No es necesario socializarlo",
              "Solo deben conocerlo los conductores",
              "Es un documento confidencial de la gerencia"
            ],
            "correct": 0
          },
          {
            "q": "¿Quién define la metodología oficial para construir el PESV?",
            "options": [
              "Cada empresa la define libremente sin ningún criterio",
              "El Ministerio de Transporte, mediante la Resolución 40595 de 2022",
              "La ARL exclusivamente",
              "El Ministerio del Trabajo"
            ],
            "correct": 1
          }
        ],
        "apply": "Pregunta si tu empresa ya socializó el PESV contigo. Si no lo conoces, pídelo."
      },
      {
        "key": "normatividad_pesv",
        "title": "Normatividad PESV",
        "intro": "El PESV está regulado principalmente por la Ley 1503 de 2011 y por la Resolución 40595 de 2022, que define su metodología oficial.",
        "points": [
          "Ley 1503 de 2011: modificada por el Decreto Ley 2106 de 2019",
          "Resolución 40595 de 2022: metodología oficial",
          "Aplica a quien posea, contrate o administre flotas o transporte de personal"
        ],
        "norm": "Ley 1503 de 2011 y Resolución 40595 de 2022",
        "questions": [
          {
            "q": "¿Qué norma define la metodología oficial del PESV en Colombia?",
            "options": [
              "Resolución 0312 de 2019",
              "Ley 1010 de 2006",
              "Resolución 40595 de 2022",
              "Decreto 1076 de 2015"
            ],
            "correct": 2
          },
          {
            "q": "¿A qué tipo de organizaciones aplica el PESV?",
            "options": [
              "Solo a las empresas de transporte público de pasajeros",
              "A quienes posean, contraten o administren flotas de vehículos o transporte de personal",
              "Únicamente a conductores particulares",
              "Solo a empresas con más de 500 empleados"
            ],
            "correct": 1
          }
        ],
        "apply": "Si conduces para tu empresa, pregunta si aplicas al alcance del PESV vigente."
      },
      {
        "key": "inspeccion_vehiculos_pesv",
        "title": "Inspección a vehículos",
        "intro": "La inspección preoperacional verifica, antes de cada uso, el estado de frenos, luces, llantas y niveles de fluidos del vehículo.",
        "points": [
          "Se realiza antes de cada uso del vehículo",
          "Verifica frenos, luces, llantas y fluidos",
          "Detectar una falla a tiempo es más seguro y económico"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué verifica la inspección preoperacional de un vehículo?",
            "options": [
              "Solo el nivel de combustible",
              "El estado de frenos, luces, llantas y niveles de fluidos antes de cada uso",
              "Únicamente la vigencia del SOAT",
              "El color y la estética del vehículo"
            ],
            "correct": 1
          },
          {
            "q": "¿Por qué es preferible detectar una falla en la inspección y no en movimiento?",
            "options": [
              "Porque es más barato y más seguro",
              "No hay ninguna diferencia",
              "Porque así se evita pagar el SOAT",
              "Porque acelera el viaje"
            ],
            "correct": 0
          }
        ],
        "apply": "No firmes una inspección preoperacional 'de memoria': revisa realmente cada punto antes de arrancar."
      },
      {
        "key": "beber_conducir",
        "title": "Beber y conducir",
        "intro": "Conducir bajo efectos del alcohol reduce los reflejos, la percepción de riesgo y la coordinación motriz, incluso en niveles bajos.",
        "points": [
          "Afecta reflejos y percepción del riesgo",
          "El efecto ocurre incluso con niveles bajos de alcohol",
          "No existe una cantidad completamente segura"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuánto alcohol es seguro para conducir?",
            "options": [
              "Una copa de vino",
              "Una cerveza pequeña",
              "Ninguna cantidad es completamente segura",
              "Depende del peso del conductor"
            ],
            "correct": 2
          },
          {
            "q": "¿Qué capacidades afecta el alcohol al conducir?",
            "options": [
              "Ninguna si la cantidad es baja",
              "Los reflejos, la percepción de riesgo y la coordinación motriz",
              "Solo la visión nocturna",
              "Solo la audición"
            ],
            "correct": 1
          }
        ],
        "apply": "Si vas a consumir alcohol, decide desde antes cómo vas a volver a casa sin conducir."
      },
      {
        "key": "conducir_bicicleta",
        "title": "Conducir bicicleta",
        "intro": "El ciclista debe usar casco, mantenerse en los carriles o ciclorrutas destinados, y respetar las señales de tránsito.",
        "points": [
          "Casco y elementos reflectivos",
          "Circular por carriles o ciclorrutas destinados",
          "Respetar las señales igual que cualquier vehículo"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué elemento de protección debe usar siempre un ciclista?",
            "options": [
              "Ningún elemento es obligatorio",
              "Casco",
              "Solo guantes",
              "Solo gafas de sol"
            ],
            "correct": 1
          },
          {
            "q": "¿Debe el ciclista respetar las señales de tránsito?",
            "options": [
              "No, solo aplican a los vehículos motorizados",
              "Sí, tiene las mismas obligaciones que cualquier otro actor vial",
              "Solo en las ciclorrutas",
              "Solo de noche"
            ],
            "correct": 1
          }
        ],
        "apply": "Si te mueves en bicicleta, usa siempre casco y elementos reflectivos, incluso en trayectos cortos."
      },
      {
        "key": "cortesia_conducir",
        "title": "Cortesía común al conducir",
        "intro": "Ceder el paso, no usar innecesariamente el pito y mantener la distancia de seguridad reduce la tensión en las vías.",
        "points": [
          "Ceder el paso cuando corresponde",
          "Mantener la distancia de seguridad",
          "Evitar gestos agresivos ante otros conductores"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué previene la cortesía al conducir?",
            "options": [
              "Comportamientos de riesgo derivados de la frustración al conducir",
              "El pago de multas por exceso de velocidad",
              "El desgaste de las llantas",
              "El consumo de combustible"
            ],
            "correct": 0
          },
          {
            "q": "¿Cuál es un ejemplo de cortesía al conducir?",
            "options": [
              "Usar el pito de forma constante",
              "Mantener la distancia de seguridad y ceder el paso cuando corresponde",
              "Acelerar al ver a otro conductor querer adelantar",
              "Ignorar a los peatones"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que otro conductor te cierre el paso, resiste el impulso de reaccionar con agresividad."
      },
      {
        "key": "implementos_alerta",
        "title": "Implementos de alerta de emergencia en el vehículo",
        "intro": "Todo vehículo debe contar con triángulo o señal reflectiva, chaleco reflectivo y botiquín básico, listos para usarse.",
        "points": [
          "Triángulo o señal de carretera reflectiva",
          "Chaleco reflectivo",
          "Botiquín básico"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué elementos de alerta debe llevar todo vehículo?",
            "options": [
              "Solo el botiquín básico",
              "Triángulo o señal reflectiva, chaleco reflectivo y botiquín básico",
              "Únicamente un extintor",
              "Ningún elemento es obligatorio"
            ],
            "correct": 1
          },
          {
            "q": "¿Para qué se usan los implementos de alerta del vehículo?",
            "options": [
              "Para decorar el vehículo",
              "Para usarse en caso de una falla mecánica o un incidente en la vía",
              "Solo para viajes largos",
              "No tienen ninguna utilidad real"
            ],
            "correct": 1
          }
        ],
        "apply": "Revisa hoy que tu vehículo tenga el triángulo, el chaleco reflectivo y el botiquín, y que estén donde los puedas alcanzar rápido."
      },
      {
        "key": "senales_transito",
        "title": "Señales de tránsito",
        "intro": "Las señales de tránsito se clasifican en reglamentarias, preventivas e informativas, y su respeto es responsabilidad de todos los actores viales.",
        "points": [
          "Reglamentarias: obligan o prohíben",
          "Preventivas: advierten un peligro",
          "Informativas: orientan al conductor"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué tipo de señal de tránsito advierte sobre un peligro en la vía?",
            "options": [
              "Señal reglamentaria",
              "Señal preventiva",
              "Señal informativa",
              "Señal publicitaria"
            ],
            "correct": 1
          },
          {
            "q": "¿Quién es responsable de conocer y respetar las señales de tránsito?",
            "options": [
              "Solo los conductores de vehículos pesados",
              "Conductores, ciclistas y peatones por igual",
              "Únicamente el conductor del vehículo",
              "Solo las autoridades de tránsito"
            ],
            "correct": 1
          }
        ],
        "apply": "La próxima vez que veas una señal que no recuerdas bien, búscala — conocerlas es protección real todos los días."
      },
      {
        "key": "distraccion_fatiga",
        "title": "Factores de riesgo vial: distracción y fatiga",
        "intro": "El uso del celular al conducir y la fatiga por falta de descanso reducen drásticamente el tiempo de reacción ante un imprevisto.",
        "points": [
          "El celular reduce el tiempo de reacción",
          "La fatiga afecta igual que el alcohol o la velocidad",
          "Ambos factores suelen subestimarse"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuáles son dos factores de riesgo vial frecuentemente subestimados?",
            "options": [
              "El exceso de velocidad y el clima",
              "La distracción (uso del celular) y la fatiga al conducir",
              "El color del vehículo y la hora del día",
              "El tipo de combustible y la marca del vehículo"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué efecto tiene la fatiga en la capacidad de conducción?",
            "options": [
              "Ningún efecto relevante",
              "Reduce drásticamente el tiempo de reacción ante un imprevisto",
              "Mejora la concentración",
              "Solo afecta en trayectos cortos"
            ],
            "correct": 1
          }
        ],
        "apply": "Si sientes sueño o llevas rato mirando el celular mientras conduces, para el vehículo en un lugar seguro."
      }
    ]
  },
  "calidad": {
    "label": "Gestión de Calidad",
    "icon": "check",
    "desc": "SGC, no conformidades y mejora continua",
    "keywords": [
      "calidad",
      "gestion de calidad",
      "gestión de calidad",
      "sgc",
      "iso 9001",
      "sistema de gestion de calidad",
      "sistema de gestión de calidad",
      "no conformidad"
    ],
    "modules": [
      {
        "key": "que_es_sgc",
        "title": "¿Qué es un Sistema de Gestión de Calidad?",
        "intro": "Un SGC organiza los procesos de una empresa para asegurar, de forma consistente, que sus productos o servicios cumplan los requisitos del cliente.",
        "points": [
          "Busca consistencia, no un logro aislado",
          "Aplica a productos y servicios por igual",
          "Su referencia internacional más usada es la NTC-ISO 9001"
        ],
        "norm": "NTC-ISO 9001",
        "questions": [
          {
            "q": "¿Qué busca principalmente un Sistema de Gestión de Calidad?",
            "options": [
              "Aumentar el número de empleados de la empresa",
              "Asegurar que los productos o servicios cumplan consistentemente los requisitos del cliente",
              "Reducir el precio de los productos sin importar la calidad",
              "Eliminar por completo la necesidad de auditorías"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuál es la referencia internacional más usada para un SGC?",
            "options": [
              "La norma NTC-ISO 9001",
              "El Código Sustantivo del Trabajo",
              "El Decreto 1072 de 2015",
              "La Ley 99 de 1993"
            ],
            "correct": 0
          }
        ],
        "apply": "La próxima vez que entregues un trabajo, pregúntate: ¿esto cumple exactamente lo que el cliente pidió?"
      },
      {
        "key": "enfoque_cliente",
        "title": "Enfoque al cliente",
        "intro": "Todo SGC parte de entender lo que el cliente necesita y esperar superarlo, no solo cumplirlo.",
        "points": [
          "Escuchar quejas y sugerencias activamente",
          "Medir la satisfacción del cliente",
          "Usar esa información para ajustar procesos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué implica el enfoque al cliente en un SGC?",
            "options": [
              "Ignorar las quejas si son pocas",
              "Escuchar, medir la satisfacción y usar esa información para ajustar procesos",
              "Solo cumplir el contrato firmado",
              "Enfocarse únicamente en el precio"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué busca un SGC frente a las expectativas del cliente?",
            "options": [
              "Cumplirlas exactamente, ni más ni menos",
              "Entenderlas y esperar superarlas",
              "Ignorarlas si no están por escrito",
              "Reducirlas para facilitar su cumplimiento"
            ],
            "correct": 1
          }
        ],
        "apply": "Si un cliente te da una queja, no la veas como un problema: es información gratuita sobre qué mejorar."
      },
      {
        "key": "liderazgo_compromiso",
        "title": "Liderazgo y compromiso de la dirección",
        "intro": "Un sistema de calidad no funciona si la alta dirección no lo respalda de forma visible, asignando recursos y participando activamente.",
        "points": [
          "La dirección debe asignar recursos reales",
          "Debe participar en la revisión del sistema",
          "Debe exigirse el mismo estándar que al resto de la organización"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué necesita un SGC para funcionar realmente, más allá de la documentación?",
            "options": [
              "Que la alta dirección lo respalde de forma visible",
              "Que solo el área de calidad lo conozca",
              "Que se revise una sola vez al certificarse",
              "Que no involucre a la dirección"
            ],
            "correct": 0
          },
          {
            "q": "¿De qué forma se manifiesta el compromiso de la alta dirección con el SGC?",
            "options": [
              "Firmando el certificado únicamente",
              "Asignando recursos y participando en la revisión del sistema",
              "Delegando el tema por completo sin seguimiento",
              "Solo mencionándolo en reuniones anuales"
            ],
            "correct": 1
          }
        ],
        "apply": "Si eres líder de un equipo, muestra compromiso con la calidad aplicando tú mismo el estándar que le exiges a los demás."
      },
      {
        "key": "planificacion_riesgos",
        "title": "Planificación de riesgos y oportunidades",
        "intro": "Antes de que un problema ocurra, un SGC maduro ya lo anticipó, identificando riesgos y oportunidades de mejora.",
        "points": [
          "Anticipa problemas antes de que ocurran",
          "Identifica también oportunidades de mejora",
          "Planifica acciones con anticipación"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué caracteriza a un SGC maduro frente a los riesgos?",
            "options": [
              "Espera a que el problema ocurra para actuar",
              "Anticipa los riesgos y planifica acciones antes de que ocurran",
              "Ignora los riesgos menores",
              "Solo actúa ante auditorías externas"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué identifica la planificación de riesgos y oportunidades en un SGC?",
            "options": [
              "Solo los riesgos financieros",
              "Riesgos que podrían afectar la calidad y oportunidades de mejora",
              "Únicamente el desempeño de un empleado",
              "El presupuesto de marketing"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de iniciar una tarea importante, pregúntate: ¿qué podría salir mal aquí, y qué haría si pasa?"
      },
      {
        "key": "contexto_organizacion",
        "title": "Contexto de la organización",
        "intro": "Entender el contexto significa identificar los factores internos y externos que pueden afectar la capacidad de la empresa de lograr sus resultados.",
        "points": [
          "Incluye competencia y regulación externa",
          "Incluye también las expectativas de las partes interesadas",
          "Afecta directamente el logro de los resultados esperados"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué significa \"contexto de la organización\" en un SGC?",
            "options": [
              "El horario de atención de la empresa",
              "Los factores internos y externos que pueden afectar el logro de los resultados esperados",
              "El organigrama de la compañía",
              "El manual de bienvenida para nuevos empleados"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué tipo de factores se consideran al analizar el contexto de la organización?",
            "options": [
              "Solo factores internos",
              "Factores internos y externos, como competencia y regulación",
              "Solo el clima laboral",
              "Solo las ventas del último mes"
            ],
            "correct": 1
          }
        ],
        "apply": "Piensa en un cambio reciente del entorno (un competidor, una norma nueva) y en cómo podría afectar tu proceso."
      },
      {
        "key": "documentacion_control",
        "title": "Documentación y control de la información",
        "intro": "La información documentada debe estar actualizada, ser de fácil acceso y estar protegida frente a cambios no autorizados.",
        "points": [
          "Debe estar siempre actualizada",
          "Debe ser de fácil acceso para quien la necesita",
          "Debe protegerse frente a cambios no autorizados"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué riesgo representa un documento desactualizado en un SGC?",
            "options": [
              "Ninguno, siempre es mejor tener algo documentado",
              "Puede ser más riesgoso que no tener documento",
              "Solo afecta la estética de los archivos",
              "No tiene ninguna relevancia legal"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué características debe tener la información documentada de un SGC?",
            "options": [
              "Estar actualizada, ser accesible y estar protegida ante cambios no autorizados",
              "Ser secreta para todos los empleados",
              "Cambiarse libremente por cualquier persona",
              "No requiere actualización periódica"
            ],
            "correct": 0
          }
        ],
        "apply": "La próxima vez que uses un formato, verifica que sea la versión más reciente antes de diligenciarlo."
      },
      {
        "key": "competencia_conciencia",
        "title": "Competencia y toma de conciencia",
        "intro": "La empresa debe asegurar que cada persona tenga la formación necesaria para su función, y sea consciente de su aporte a la calidad final.",
        "points": [
          "Formación y experiencia adecuadas al cargo",
          "Conciencia de cómo el propio trabajo aporta al resultado final",
          "Contribuye directamente a la satisfacción del cliente"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué debe garantizar la empresa respecto a la competencia del personal?",
            "options": [
              "Que tenga la formación y experiencia necesarias para su función",
              "Que todos tengan el mismo cargo",
              "Que roten de área cada mes",
              "Que trabajen sin supervisión"
            ],
            "correct": 0
          },
          {
            "q": "¿Por qué es importante la toma de conciencia del personal en un SGC?",
            "options": [
              "Porque no tiene relación con la calidad final",
              "Porque ayuda a entender cómo su trabajo contribuye a la calidad y satisfacción del cliente",
              "Porque es un requisito solo para los directivos",
              "Porque reemplaza la necesidad de capacitación"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de asumir una tarea nueva, sé honesto contigo mismo: ¿tienes la formación necesaria, o deberías pedir capacitación primero?"
      },
      {
        "key": "control_operacional",
        "title": "Control operacional de procesos",
        "intro": "Controlar un proceso significa definir de antemano cómo debe ejecutarse y qué hacer si el resultado no es el esperado.",
        "points": [
          "Se define antes de ejecutar el proceso",
          "Incluye criterios de aceptación claros",
          "Anticipa qué hacer si algo sale mal"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué implica controlar un proceso en un SGC?",
            "options": [
              "Descubrir el problema cuando el producto ya llegó al cliente",
              "Definir de antemano cómo debe ejecutarse y qué hacer si el resultado no es el esperado",
              "No definir ningún criterio de aceptación",
              "Delegar el control únicamente al cliente final"
            ],
            "correct": 1
          },
          {
            "q": "¿Cuándo es preferible detectar una desviación en un proceso controlado?",
            "options": [
              "Después de que el producto llegue al cliente",
              "Antes de que el producto llegue al cliente, mediante criterios definidos de antemano",
              "Nunca es posible detectarla a tiempo",
              "Solo durante auditorías externas"
            ],
            "correct": 1
          }
        ],
        "apply": "Antes de ejecutar un proceso, revisa si existen criterios claros de aceptación para saber si el resultado quedó bien."
      },
      {
        "key": "no_conformidades",
        "title": "No conformidades y acciones correctivas",
        "intro": "Una no conformidad es el incumplimiento de un requisito establecido. Frente a ella, se implementa una acción correctiva.",
        "points": [
          "No conformidad: incumplimiento de un requisito",
          "Acción correctiva: elimina la causa raíz",
          "El objetivo es que el problema no se repita"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Qué es una no conformidad?",
            "options": [
              "Un elogio recibido de un cliente",
              "El incumplimiento de un requisito establecido",
              "Un tipo de indicador de gestión",
              "Un modelo de certificado de calidad"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué es una acción correctiva?",
            "options": [
              "Una acción tomada para eliminar la causa de una no conformidad y evitar que se repita",
              "Una sanción dirigida al responsable del error",
              "Un cambio estético en un producto",
              "Una acción que se toma antes de que ocurra el problema"
            ],
            "correct": 0
          }
        ],
        "apply": "La próxima vez que algo salga mal, pregúntate por qué pasó, para atacar la causa real y no solo el síntoma."
      },
      {
        "key": "auditorias_internas",
        "title": "Auditorías internas de calidad",
        "intro": "La auditoría interna verifica, con evidencia objetiva, si el SGC se aplica tal como está documentado y si es eficaz.",
        "points": [
          "Se basa en evidencia objetiva, no en opiniones",
          "No busca culpables, busca oportunidades de mejora",
          "Verifica tanto la aplicación como la eficacia del sistema"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Cuál es el propósito de una auditoría interna de calidad?",
            "options": [
              "Encontrar y sancionar culpables",
              "Verificar con evidencia si el sistema se aplica y es eficaz, buscando oportunidades de mejora",
              "Reemplazar la certificación externa",
              "Medir únicamente la satisfacción del cliente"
            ],
            "correct": 1
          },
          {
            "q": "¿En qué se basa una auditoría interna para sus conclusiones?",
            "options": [
              "En opiniones personales del auditor",
              "En evidencia objetiva",
              "En rumores dentro de la empresa",
              "En el desempeño financiero únicamente"
            ],
            "correct": 1
          }
        ],
        "apply": "Si te toca una auditoría interna, no la veas como una evaluación personal: es una oportunidad de mejora."
      },
      {
        "key": "indicadores_calidad",
        "title": "Indicadores y seguimiento de procesos",
        "intro": "Los indicadores de calidad permiten medir el desempeño real de los procesos con datos, no con percepciones.",
        "points": [
          "Se basan en datos, no en percepciones",
          "Sin medición no hay evidencia de mejora real",
          "Permiten hacer seguimiento objetivo a los procesos"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿Para qué sirven los indicadores de calidad?",
            "options": [
              "Para decorar los informes de gestión",
              "Para medir el desempeño real de los procesos con datos",
              "Únicamente para cumplir un requisito de auditoría externa",
              "Para calificar el desempeño de un solo empleado"
            ],
            "correct": 1
          },
          {
            "q": "¿Qué ocurre con la mejora continua si no hay indicadores que la midan?",
            "options": [
              "Se vuelve una intención sin evidencia de si realmente funciona",
              "No afecta en nada a la mejora continua",
              "Mejora automáticamente sin necesidad de medición",
              "Solo afecta al área financiera"
            ],
            "correct": 0
          }
        ],
        "apply": "Antes de decir que un proceso 'va bien', pregúntate si tienes un dato que lo respalde."
      },
      {
        "key": "mejora_continua",
        "title": "Mejora continua",
        "intro": "La mejora continua es el compromiso permanente de optimizar procesos, productos y servicios, apoyado en el ciclo PHVA.",
        "points": [
          "Es un compromiso permanente, no un evento único",
          "Se apoya en el ciclo PHVA",
          "No espera a que algo falle para actuar"
        ],
        "norm": "",
        "questions": [
          {
            "q": "¿En qué ciclo se apoya la mejora continua?",
            "options": [
              "El ciclo de ventas",
              "El ciclo PHVA (Planear-Hacer-Verificar-Actuar)",
              "El ciclo de vida del producto únicamente",
              "El ciclo contable anual"
            ],
            "correct": 1
          },
          {
            "q": "¿La mejora continua espera a que algo falle para actuar?",
            "options": [
              "Sí, siempre reacciona después de una falla",
              "No, revisa constantemente qué se puede hacer mejor",
              "Solo actúa una vez al año",
              "Solo aplica después de una auditoría externa"
            ],
            "correct": 1
          }
        ],
        "apply": "Elige hoy una tarea repetitiva de tu trabajo y pregúntate: ¿hay una forma de hacerla mejor?"
      }
    ]
  }
};

const PASSING_SCORE = 3.0; // escala 0.0 - 5.0

</script>
<script>
// ============================================================
// Centro de Formación — lógica de la aplicación (modelo por pilares y módulos)
// ============================================================

const state = {
  pillarKey: null,
  moduleIndex: 0,
  score: 0,
  approved: false,
  participant: { name: "", doc: "" },
  certId: null,
};

const session = {
  user: null,       // { cedula, name, cargo }
  roster: [],        // [{cedula, name, cargo, area, sede, correo}]
  branding: { logo: "", name: "", nit: "" },
};

// ============================================================
// Marca de la empresa cliente (logo, nombre, NIT) — reemplaza cualquier
// marca genérica en la interfaz y en los certificados generados.
// ============================================================
function renderBrand() {
  const mark = document.getElementById("brandMark");
  const label = document.getElementById("brandLabel");
  if (session.branding.logo) {
    mark.innerHTML = `<img src="${session.branding.logo}" alt="">`;
  } else {
    mark.textContent = "CF";
  }
  label.textContent = "Centro de Formación";
  document.title = session.branding.name ? `Centro de Formación · ${session.branding.name}` : "Centro de Formación";
}
function renderBrandLogoPreview() {
  const wrap = document.getElementById("brandLogoPreview");
  wrap.innerHTML = session.branding.logo
    ? `<img src="${session.branding.logo}" alt="" style="width:100%;height:100%;object-fit:contain;">`
    : ICONS.upload;
}

// ============================================================
// Bloqueo / desbloqueo de PILARES (estilo Moodle) — persistente
// ============================================================
const LOCKS_KEY = "ps_pillar_locks_v1";
const PIN_KEY = "ps_admin_pin_v1";
const DEFAULT_PIN = "1234";

function getLockState() {
  try {
    const raw = localStorage.getItem(LOCKS_KEY);
    if (raw) return JSON.parse(raw);
  } catch (e) {}
  if (EMBEDDED_LOCKS && typeof EMBEDDED_LOCKS === "object") {
    const merged = {};
    Object.keys(PILLARS).forEach((k) => (merged[k] = !!EMBEDDED_LOCKS[k]));
    return merged;
  }
  const initial = {};
  Object.keys(PILLARS).forEach((k) => (initial[k] = false));
  return initial;
}
function saveLockState(locks) {
  try { localStorage.setItem(LOCKS_KEY, JSON.stringify(locks)); } catch (e) {}
}
function isPillarUnlocked(key) {
  const locks = getLockState();
  return !!locks[key];
}
function setPillarUnlocked(key, unlocked) {
  const locks = getLockState();
  locks[key] = unlocked;
  saveLockState(locks);
}
function getAdminPin() {
  try { return localStorage.getItem(PIN_KEY) || DEFAULT_PIN; } catch (e) { return DEFAULT_PIN; }
}
function setAdminPin(pin) {
  try { localStorage.setItem(PIN_KEY, pin); } catch (e) {}
}

// ============================================================
// Progreso por empleado (módulos aprobados) — persistente por cédula
// ============================================================
const PROGRESS_KEY = "ps_progress_v1";

function getAllProgress() {
  try {
    const raw = localStorage.getItem(PROGRESS_KEY);
    if (raw) return JSON.parse(raw);
  } catch (e) {}
  return {};
}
function saveAllProgress(all) {
  try { localStorage.setItem(PROGRESS_KEY, JSON.stringify(all)); } catch (e) {}
}
function getModuleRecord(cedula, pillarKey, moduleKey) {
  const all = getAllProgress();
  return (all[cedula] && all[cedula][pillarKey] && all[cedula][pillarKey][moduleKey]) || null;
}
function setModuleRecord(cedula, pillarKey, moduleKey, record) {
  const all = getAllProgress();
  if (!all[cedula]) all[cedula] = {};
  if (!all[cedula][pillarKey]) all[cedula][pillarKey] = {};
  all[cedula][pillarKey][moduleKey] = Object.assign({}, all[cedula][pillarKey][moduleKey], record);
  saveAllProgress(all);
}
function isModulePassed(pillarKey, moduleKey) {
  if (!session.user) return false;
  const rec = getModuleRecord(session.user.cedula, pillarKey, moduleKey);
  return !!(rec && rec.passed);
}
function isModuleUnlocked(pillarKey, moduleIndex) {
  if (moduleIndex === 0) return true;
  const pillar = PILLARS[pillarKey];
  const prevModule = pillar.modules[moduleIndex - 1];
  return isModulePassed(pillarKey, prevModule.key);
}

// ---------- Utilidades ----------
function normalize(str) {
  return str.toLowerCase().normalize("NFD").replace(/[\u0300-\u036f]/g, "").replace(/[^a-z0-9\s]/g, "").trim();
}
function findPillarByQuery(query) {
  const q = normalize(query);
  if (!q) return null;
  let bestKey = null, bestScore = 0;
  Object.entries(PILLARS).forEach(([key, pillar]) => {
    let score = 0;
    pillar.keywords.forEach((kw) => {
      const nkw = normalize(kw);
      if (q === nkw) score += 5;
      else if (q.includes(nkw) || nkw.includes(q)) score += 2;
    });
    if (score > bestScore) { bestScore = score; bestKey = key; }
  });
  return bestScore > 0 ? bestKey : null;
}

function showScreen(id) {
  document.querySelectorAll(".screen").forEach((s) => s.classList.remove("active"));
  document.getElementById(id).classList.add("active");
  window.scrollTo({ top: 0, behavior: "smooth" });
  updateSteps(id);
}
function updateSteps(screenId) {
  const map = {
    "screen-login": "login", "screen-admin": "login",
    "screen-home": "home",
    "screen-pillar": "pillar",
    "screen-module": "content",
    "screen-quiz": "quiz",
    "screen-result": "result", "screen-certificate": "result",
  };
  const current = map[screenId] || "home";
  const order = ["login", "home", "pillar", "content", "quiz", "result"];
  const currentIdx = order.indexOf(current);
  document.querySelectorAll(".step").forEach((el) => {
    const idx = order.indexOf(el.dataset.step);
    el.classList.remove("active", "done");
    if (idx < currentIdx) el.classList.add("done");
    else if (idx === currentIdx) el.classList.add("active");
  });
}

// ---------- Grilla de pilares (Home) ----------
function renderTopicsGrid() {
  const grid = document.getElementById("topicsGrid");
  grid.innerHTML = "";
  const locks = getLockState();
  Object.entries(PILLARS).forEach(([key, pillar]) => {
    const isUnlocked = !!locks[key];
    const btn = document.createElement("button");
    btn.className = "topic-tile" + (isUnlocked ? "" : " locked");
    btn.style.position = "relative";
    const doneCount = isUnlocked && session.user ? countDoneModules(key) : 0;
    btn.innerHTML = `
      ${isUnlocked ? "" : `<div class="tile-lock-badge">${ICONS.lock} Bloqueado</div>`}
      <div class="icon">${ICONS[pillar.icon]}</div>
      <div class="name">${pillar.label}</div>
      <div class="desc">${pillar.desc} · ${pillar.modules.length} módulos</div>
      ${isUnlocked && session.user ? `<div class="desc" style="margin-top:6px; color:${doneCount === pillar.modules.length ? "var(--green)" : "rgba(255,255,255,0.5)"};">${doneCount} de ${pillar.modules.length} completados</div>` : ""}
    `;
    btn.addEventListener("click", () => {
      if (isUnlocked) openPillar(key);
      else showHomeHint(`El pilar "${pillar.label}" aún no está habilitado. Pídele a tu administrador de formación que lo active.`);
    });
    grid.appendChild(btn);
  });
}
function countDoneModules(pillarKey) {
  if (!session.user) return 0;
  let n = 0;
  PILLARS[pillarKey].modules.forEach((m) => { if (isModulePassed(pillarKey, m.key)) n++; });
  return n;
}
function showHomeHint(msg) {
  const hint = document.getElementById("searchHint");
  hint.textContent = msg;
  hint.style.color = "var(--accent-dim)";
}

// ---------- Buscar por palabra/frase ----------
function handleSearch() {
  const input = document.getElementById("searchInput");
  const hint = document.getElementById("searchHint");
  const pillarKey = findPillarByQuery(input.value);
  const pillar = pillarKey ? PILLARS[pillarKey] : null;
  if (pillar) {
    if (!isPillarUnlocked(pillarKey)) {
      hint.textContent = `El pilar "${pillar.label}" existe pero aún no está habilitado. Pídele a tu administrador de formación que lo active.`;
      hint.style.color = "var(--accent-dim)";
      return;
    }
    hint.textContent = `Encontramos el pilar "${pillar.label}". Abriendo su camino de módulos...`;
    hint.style.color = "var(--accent)";
    setTimeout(() => openPillar(pillarKey), 400);
  } else if (input.value.trim() === "") {
    hint.textContent = "Escribe una palabra o frase, por ejemplo: \"extintores\", \"reciclaje\" o \"PHVA\".";
    hint.style.color = "var(--accent)";
  } else {
    hint.textContent = "No encontramos un pilar exacto para esa palabra. Elige uno de los disponibles abajo.";
    hint.style.color = "var(--accent-dim)";
  }
}

// ============================================================
// Pantalla de PILAR — camino de módulos
// ============================================================
function openPillar(pillarKey) {
  state.pillarKey = pillarKey;
  const pillar = PILLARS[pillarKey];
  document.getElementById("pillarTag").textContent = "Pilar";
  document.getElementById("pillarTitle").textContent = pillar.label;
  renderModuleList();
  showScreen("screen-pillar");
}

function renderModuleList() {
  const pillar = PILLARS[state.pillarKey];
  const wrap = document.getElementById("moduleList");
  wrap.innerHTML = "";
  let doneCount = 0;

  pillar.modules.forEach((m, i) => {
    const done = isModulePassed(state.pillarKey, m.key);
    const unlocked = isModuleUnlocked(state.pillarKey, i);
    if (done) doneCount++;
    const status = done ? "done" : unlocked ? "available" : "locked";
    const row = document.createElement("div");
    row.className = `module-row ${status}`;
    row.style.animationDelay = `${i * 0.03}s`;

    let numHtml = String(i + 1).padStart(2, "0");
    if (done) numHtml = ICONS.check_circle;
    else if (!unlocked) numHtml = ICONS.lock;

    let statusText = "Bloqueado";
    if (done) {
      const rec = getModuleRecord(session.user.cedula, state.pillarKey, m.key);
      statusText = `Aprobado · ${rec.score.toFixed(1)} / 5.0`;
    } else if (unlocked) {
      statusText = "Disponible";
    }

    let actionHtml = "";
    if (done) {
      actionHtml = `<button class="btn-module secondary" data-action="cert" data-i="${i}">Ver certificado</button>`;
    } else if (unlocked) {
      actionHtml = `<button class="btn-module" data-action="start" data-i="${i}">Iniciar módulo</button>`;
    } else {
      actionHtml = `<button class="btn-module" disabled>Bloqueado</button>`;
    }

    row.innerHTML = `
      <div class="module-num">${numHtml}</div>
      <div class="module-info">
        <div class="m-title">${m.title}</div>
        <div class="m-status">${statusText}</div>
      </div>
      <div class="module-row-action">${actionHtml}</div>
    `;
    wrap.appendChild(row);
  });

  wrap.querySelectorAll('[data-action="start"]').forEach((btn) => {
    btn.addEventListener("click", () => startModule(state.pillarKey, parseInt(btn.dataset.i, 10)));
  });
  wrap.querySelectorAll('[data-action="cert"]').forEach((btn) => {
    btn.addEventListener("click", () => {
      const i = parseInt(btn.dataset.i, 10);
      const m = pillar.modules[i];
      const rec = getModuleRecord(session.user.cedula, state.pillarKey, m.key);
      state.moduleIndex = i;
      state.score = rec.score;
      state.certId = rec.certId || null;
      showCertificate();
    });
  });

  const pct = Math.round((doneCount / pillar.modules.length) * 100);
  document.getElementById("pillarProgressFill").style.width = pct + "%";
  document.getElementById("pillarProgressLabel").textContent = `${doneCount} de ${pillar.modules.length} módulos completados`;
}

document.getElementById("backHomeFromPillar").addEventListener("click", () => {
  renderTopicsGrid();
  showScreen("screen-home");
});

// ============================================================
// Pantalla de MÓDULO — presentación animada (carrusel, mínimo 6 diapositivas)
// ============================================================
function startModule(pillarKey, moduleIndex) {
  state.pillarKey = pillarKey;
  state.moduleIndex = moduleIndex;
  state.slideIndex = 0;
  state.seenSlides = new Set([0]);
  stopSpeech();
  buildSlideDeck();
  renderModuleSlide();
  showScreen("screen-module");
}

// Construye la secuencia de diapositivas del módulo actual a partir de su contenido
function buildSlideDeck() {
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];
  const deck = [];

  deck.push({ type: "hook", icon: pillar.icon, title: m.title, sub: `${pillar.label} · Módulo ${state.moduleIndex + 1} de ${pillar.modules.length}` });
  deck.push({ type: "concept", text: m.intro });
  m.points.forEach((p, i) => deck.push({ type: "point", num: i + 1, text: p }));
  if (m.apply) deck.push({ type: "apply", text: m.apply });
  deck.push({ type: "recap", points: m.points, norm: m.norm, title: m.title });

  state.deck = deck;
}

function renderModuleSlide() {
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];
  const total = state.deck.length;
  const slide = state.deck[state.slideIndex];

  document.getElementById("moduleTag").textContent = `${pillar.label} · Módulo ${state.moduleIndex + 1} de ${pillar.modules.length}`;
  document.getElementById("moduleTitle").textContent = m.title;

  const wrap = document.getElementById("deckSlide");
  const bgClass = slide.type === "point" ? "bg-paper" : slide.type === "concept" ? "bg-paper" : slide.type === "apply" ? "bg-tint" : "bg-dark";
  wrap.className = "deck-slide " + bgClass;
  wrap.innerHTML = renderSlideHtml(slide, pillar);

  // Puntos: animar en cascada según el índice (para que no reaparezcan todos de golpe)
  wrap.querySelectorAll("[data-stagger]").forEach((el, i) => {
    el.style.animationDelay = `${0.15 + i * 0.12}s`;
  });

  const dotsWrap = document.getElementById("deckDots");
  dotsWrap.innerHTML = "";
  state.deck.forEach((_, i) => {
    const dot = document.createElement("div");
    dot.className = "deck-dot" + (i === state.slideIndex ? " on" : state.seenSlides.has(i) ? " seen" : "");
    dot.addEventListener("click", () => { state.slideIndex = i; state.seenSlides.add(i); renderModuleSlide(); });
    dotsWrap.appendChild(dot);
  });

  document.getElementById("prevSlideBtn").disabled = state.slideIndex === 0;
  const isLast = state.slideIndex === total - 1;
  document.getElementById("nextSlideBtn").textContent = isLast ? "Finalizar presentación" : "Siguiente →";
  document.getElementById("nextSlideBtn").disabled = false;

  const allSeen = state.seenSlides.size === total;
  document.getElementById("goToQuiz").disabled = !allSeen;

  stopSpeech();
}

function renderSlideHtml(slide, pillar) {
  if (slide.type === "hook") {
    const accents = PILLAR_ACCENTS[state.pillarKey] || ["star", "spark"];
    return `
      <div class="deck-dotgrid"></div>
      <div class="deck-blob b1"></div><div class="deck-blob b2"></div>
      <div class="pslide pslide-hook">
        <div class="hook-stage">
          <div class="hook-icon">${ICONS[slide.icon]}</div>
          <div class="hook-sticker s1">${ICONS[accents[0]]}</div>
          <div class="hook-sticker s2">${ICONS[accents[1]]}</div>
        </div>
        <p class="hook-eyebrow">${slide.sub}</p>
        <h3 class="hook-title">${slide.title}</h3>
        <p class="hook-sub">Toca "Siguiente" para comenzar esta lección</p>
        <div class="hook-module-count">${ICONS.flag} ${pillar.modules.length} módulos en este pilar</div>
      </div>`;
  }
  if (slide.type === "concept") {
    return `
      <div class="pslide pslide-concept">
        <div class="concept-icon">${ICONS.idea}</div>
        <p class="concept-label">¿De qué se trata?</p>
        <p class="concept-text">${slide.text}</p>
        <div class="concept-rule"></div>
      </div>`;
  }
  if (slide.type === "point") {
    const colorClass = slide.num === 1 ? "c1" : slide.num === 2 ? "c2" : "c3";
    const deco = slide.num === 1 ? "target" : slide.num === 2 ? "spark" : "star";
    return `
      <div class="pslide pslide-point">
        <div class="point-deco">${ICONS[deco]}</div>
        <div class="point-badge ${colorClass}">${slide.num}</div>
        <p class="point-label">Punto clave ${slide.num} de 3</p>
        <p class="point-text">${slide.text}</p>
      </div>`;
  }
  if (slide.type === "apply") {
    return `
      <div class="pslide pslide-apply">
        <div class="apply-icon">${ICONS.target}</div>
        <div class="apply-ribbon">${ICONS.spark} Llévatelo a tu día a día</div>
        <p class="apply-text">${slide.text}</p>
      </div>`;
  }
  // recap
  const itemsHtml = slide.points.map((p, i) => `
    <div class="recap-item" data-stagger>${ICONS.check_circle}<span>${p}</span></div>
  `).join("");
  const normHtml = slide.norm ? `
    <div class="recap-norm">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 3 4 7v2h16V7l-8-4Z"/><path d="M6 10v8M10 10v8M14 10v8M18 10v8"/><path d="M4 21h16"/></svg>
      ${slide.norm}
    </div>` : "";
  return `
    <div class="deck-dotgrid"></div>
    <div class="deck-blob b1"></div><div class="deck-blob b2"></div>
    <div class="pslide pslide-recap">
      <div class="recap-trophy">${ICONS.trophy}</div>
      <h3 class="recap-title">¡Repasemos "${slide.title}"!</h3>
      <div class="recap-list">${itemsHtml}</div>
      ${normHtml}
      <p class="recap-cheer">Ya puedes continuar a la evaluación →</p>
    </div>`;
}

document.getElementById("prevSlideBtn").addEventListener("click", () => {
  if (state.slideIndex > 0) { state.slideIndex--; state.seenSlides.add(state.slideIndex); renderModuleSlide(); }
});
document.getElementById("nextSlideBtn").addEventListener("click", () => {
  if (state.slideIndex < state.deck.length - 1) { state.slideIndex++; state.seenSlides.add(state.slideIndex); renderModuleSlide(); }
  else if (!document.getElementById("goToQuiz").disabled) goToQuizScreen();
});

document.getElementById("backToPillarFromModule").addEventListener("click", () => {
  stopSpeech();
  renderModuleList();
  showScreen("screen-pillar");
});
document.getElementById("goToQuiz").addEventListener("click", () => {
  if (!document.getElementById("goToQuiz").disabled) goToQuizScreen();
});

// ---------- Narración (texto a voz) ----------
let speaking = false;
function toggleSpeech() {
  const btn = document.getElementById("listenBtn");
  const label = document.getElementById("listenLabel");
  if (!("speechSynthesis" in window)) { label.textContent = "No disponible"; return; }
  if (speaking) { stopSpeech(); return; }
  const slide = state.deck[state.slideIndex];
  let text = "";
  if (slide.type === "hook") text = `${slide.title}.`;
  else if (slide.type === "concept") text = slide.text;
  else if (slide.type === "point") text = `Punto clave ${slide.num}. ${slide.text}`;
  else if (slide.type === "apply") text = `Llévatelo a tu día a día. ${slide.text}`;
  else text = `Repasemos. ${slide.points.join(". ")}. ${slide.norm ? "Norma aplicable: " + slide.norm : ""}`;
  const utter = new SpeechSynthesisUtterance(text);
  utter.lang = "es-ES";
  utter.rate = 0.98;
  utter.onend = () => { speaking = false; btn.classList.remove("playing"); label.textContent = "Escuchar"; };
  window.speechSynthesis.cancel();
  window.speechSynthesis.speak(utter);
  speaking = true;
  btn.classList.add("playing");
  label.textContent = "Detener";
}
function stopSpeech() {
  if ("speechSynthesis" in window) window.speechSynthesis.cancel();
  speaking = false;
  const btn = document.getElementById("listenBtn");
  const label = document.getElementById("listenLabel");
  if (btn) btn.classList.remove("playing");
  if (label) label.textContent = "Escuchar";
}
document.getElementById("listenBtn").addEventListener("click", toggleSpeech);

// ============================================================
// Evaluación del módulo
// ============================================================
function goToQuizScreen() {
  stopSpeech();
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];
  document.getElementById("quizTag").textContent = `${pillar.label} · Módulo ${state.moduleIndex + 1} de ${pillar.modules.length}`;
  document.getElementById("quizTitle").textContent = `Evaluación — ${m.title}`;
  const nameInput = document.getElementById("participantName");
  const docInput = document.getElementById("participantDoc");
  if (session.user) {
    nameInput.value = session.user.name;
    docInput.value = session.user.cedula;
    nameInput.readOnly = true;
    docInput.readOnly = true;
  }
  renderQuiz();
  showScreen("screen-quiz");
}

function renderQuiz() {
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];
  const wrap = document.getElementById("quizQuestions");
  wrap.innerHTML = "";
  m.questions.forEach((q, qi) => {
    const card = document.createElement("div");
    card.className = "q-card";
    const optionsHtml = q.options.map((opt, oi) => `
      <label class="opt">
        <input type="radio" name="q${qi}" value="${oi}">
        <span>${opt}</span>
      </label>`).join("");
    card.innerHTML = `
      <div class="q-num">Pregunta ${qi + 1} de ${m.questions.length}</div>
      <h4>${q.q}</h4>
      ${optionsHtml}
    `;
    wrap.appendChild(card);
  });
  wrap.querySelectorAll('input[type="radio"]').forEach((input) => input.addEventListener("change", updateQuizProgress));
  updateQuizProgress();
  document.getElementById("quizError").textContent = "";
}

function updateQuizProgress() {
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];
  let answered = 0;
  m.questions.forEach((_, qi) => { if (document.querySelector(`input[name="q${qi}"]:checked`)) answered++; });
  document.getElementById("quizProgress").textContent = `${answered} de ${m.questions.length} preguntas respondidas`;
}

document.getElementById("backToContent").addEventListener("click", () => {
  renderModuleSlide();
  showScreen("screen-module");
});

document.getElementById("submitQuiz").addEventListener("click", () => {
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];
  const name = document.getElementById("participantName").value.trim();
  const errEl = document.getElementById("quizError");

  if (!name) {
    errEl.textContent = "Escribe tu nombre completo antes de enviar la evaluación.";
    document.getElementById("participantName").focus();
    return;
  }
  let unanswered = [];
  m.questions.forEach((_, qi) => { if (!document.querySelector(`input[name="q${qi}"]:checked`)) unanswered.push(qi + 1); });
  if (unanswered.length > 0) {
    errEl.textContent = `Faltan por responder las preguntas: ${unanswered.join(", ")}.`;
    return;
  }
  errEl.textContent = "";
  state.participant.name = name;
  state.participant.doc = document.getElementById("participantDoc").value.trim();

  let correctCount = 0;
  m.questions.forEach((q, qi) => {
    const selected = document.querySelector(`input[name="q${qi}"]:checked`);
    if (selected && parseInt(selected.value, 10) === q.correct) correctCount++;
  });

  const score = Math.round((correctCount / m.questions.length) * 5 * 10) / 10;
  state.score = score;
  state.approved = score >= PASSING_SCORE;
  state.certId = null;

  if (state.approved && session.user) {
    setModuleRecord(session.user.cedula, state.pillarKey, m.key, {
      passed: true, score, date: new Date().toISOString(),
    });
  }

  renderResult(correctCount, m.questions.length);
  showScreen("screen-result");
});

// ---------- Resultado ----------
function renderResult(correctCount, total) {
  const pillar = PILLARS[state.pillarKey];
  const scoreEl = document.getElementById("gaugeScore");
  const ring = document.getElementById("gaugeRing");
  const titleEl = document.getElementById("resultTitle");
  const msgEl = document.getElementById("resultMsg");
  const actionsEl = document.getElementById("resultActions");

  scoreEl.textContent = state.score.toFixed(1);
  const pct = (state.score / 5) * 100;
  const color = state.approved ? "#2E7D32" : "#C1121F";
  ring.style.background = `conic-gradient(${color} ${pct}%, #EDE6D3 ${pct}%)`;
  ring.style.WebkitMask = "radial-gradient(farthest-side, transparent 68%, #000 69%)";
  ring.style.mask = "radial-gradient(farthest-side, transparent 68%, #000 69%)";

  actionsEl.innerHTML = "";
  const hasNext = state.moduleIndex + 1 < pillar.modules.length;

  if (state.approved) {
    titleEl.innerHTML = `Módulo aprobado <span class="badge-pass">✓</span>`;
    msgEl.textContent = `Respondiste correctamente ${correctCount} de ${total} preguntas. Tu calificación (${state.score.toFixed(1)} / 5.0) supera el mínimo aprobatorio de 3.0.` +
      (hasNext ? " El siguiente módulo de este pilar ya está disponible." : " Has completado todos los módulos de este pilar.");
    const certBtn = document.createElement("button");
    certBtn.className = "btn btn-accent";
    certBtn.textContent = "Generar certificado →";
    certBtn.addEventListener("click", showCertificate);
    actionsEl.appendChild(certBtn);
  } else {
    titleEl.innerHTML = `Módulo no aprobado <span class="badge-fail">✕</span>`;
    msgEl.textContent = `Respondiste correctamente ${correctCount} de ${total} preguntas. Tu calificación (${state.score.toFixed(1)} / 5.0) no alcanza el mínimo aprobatorio de 3.0. Repasa la lección y vuelve a intentarlo.`;
    const retryBtn = document.createElement("button");
    retryBtn.className = "btn btn-accent";
    retryBtn.textContent = "Repasar módulo";
    retryBtn.addEventListener("click", () => {
      state.slideIndex = 0;
      state.seenSlides = new Set([0]);
      buildSlideDeck();
      renderModuleSlide();
      showScreen("screen-module");
    });
    actionsEl.appendChild(retryBtn);
    const retryQuizBtn = document.createElement("button");
    retryQuizBtn.className = "btn btn-ghost";
    retryQuizBtn.textContent = "Intentar evaluación de nuevo";
    retryQuizBtn.addEventListener("click", () => { renderQuiz(); showScreen("screen-quiz"); });
    actionsEl.appendChild(retryQuizBtn);
  }

  const pillarBtn = document.createElement("button");
  pillarBtn.className = "btn btn-ghost";
  pillarBtn.textContent = "Volver al pilar";
  pillarBtn.addEventListener("click", () => { renderModuleList(); showScreen("screen-pillar"); });
  actionsEl.appendChild(pillarBtn);
}

// ============================================================
// Certificado (por módulo)
// ============================================================
function generateCertId() {
  const d = new Date();
  const rand = Math.random().toString(36).substring(2, 7).toUpperCase();
  return `CF-${d.getFullYear()}${String(d.getMonth() + 1).padStart(2, "0")}${String(d.getDate()).padStart(2, "0")}-${rand}`;
}

function showCertificate() {
  const pillar = PILLARS[state.pillarKey];
  const m = pillar.modules[state.moduleIndex];

  if (!state.certId) {
    const existing = session.user ? getModuleRecord(session.user.cedula, state.pillarKey, m.key) : null;
    state.certId = (existing && existing.certId) || generateCertId();
    if (session.user) setModuleRecord(session.user.cedula, state.pillarKey, m.key, { certId: state.certId });
  }

  document.getElementById("certName").textContent = state.participant.name || (session.user ? session.user.name : "");
  const docValue = state.participant.doc || (session.user ? session.user.cedula : "");
  document.getElementById("certDoc").textContent = docValue ? `Documento: ${docValue}` : "";
  document.getElementById("certCourse").textContent = m.title;
  document.getElementById("certPillar").textContent = pillar.label;
  document.getElementById("certScore").textContent = `${state.score.toFixed(1)} / 5.0`;

  const certLogo = document.getElementById("certLogo");
  if (session.branding.logo) { certLogo.src = session.branding.logo; certLogo.style.display = "inline-block"; }
  else certLogo.style.display = "none";
  document.getElementById("certOrgName").textContent = session.branding.name || "Centro de Formación";
  document.getElementById("certOrgNit").textContent = session.branding.nit ? `NIT: ${session.branding.nit}` : "";

  const today = new Date();
  document.getElementById("certDate").textContent = `Fecha: ${today.toLocaleDateString("es-CO", { year: "numeric", month: "long", day: "numeric" })}`;
  document.getElementById("certId").textContent = `ID: ${state.certId}`;

  const nextBtn = document.getElementById("nextModuleFromCert");
  const hasNext = state.moduleIndex + 1 < pillar.modules.length && isModuleUnlocked(state.pillarKey, state.moduleIndex + 1);
  if (hasNext) {
    nextBtn.style.display = "inline-flex";
    nextBtn.onclick = () => startModule(state.pillarKey, state.moduleIndex + 1);
  } else {
    nextBtn.style.display = "none";
  }

  showScreen("screen-certificate");
}

document.getElementById("printCert").addEventListener("click", () => window.print());
document.getElementById("backToPillarFromCert").addEventListener("click", () => {
  state.certId = null;
  renderModuleList();
  showScreen("screen-pillar");
});

// ============================================================
// Login por cédula
// ============================================================
const LAST_CEDULA_KEY = "ps_last_cedula_v1";

function findInRoster(cedula) {
  const c = (cedula || "").trim();
  return session.roster.find((r) => String(r.cedula).trim() === c) || null;
}
function loginWithCedula(cedula) {
  const errEl = document.getElementById("loginError");
  const found = findInRoster(cedula);
  if (!found) {
    errEl.textContent = session.roster.length
      ? "No encontramos esa cédula en la matrícula. Si acabas de ser inscrito, pide a tu administrador de formación que publique la matrícula actualizada."
      : "Todavía no hay una matrícula cargada en esta aplicación. Contacta a tu administrador de formación.";
    return;
  }
  errEl.textContent = "";
  setCurrentUser(found);
}
function setCurrentUser(userObj) {
  session.user = userObj;
  const badge = document.getElementById("userBadge");
  document.getElementById("userBadgeName").textContent = `${userObj.name} · C.C. ${userObj.cedula}`;
  badge.style.display = "flex";
  try { localStorage.setItem(LAST_CEDULA_KEY, userObj.cedula); } catch (e) {}
  renderTopicsGrid();
  showScreen("screen-home");
}
document.getElementById("loginBtn").addEventListener("click", () => loginWithCedula(document.getElementById("loginCedula").value));
document.getElementById("loginCedula").addEventListener("keydown", (e) => { if (e.key === "Enter") loginWithCedula(document.getElementById("loginCedula").value); });
document.getElementById("logoutBtn").addEventListener("click", () => {
  session.user = null;
  document.getElementById("userBadge").style.display = "none";
  document.getElementById("loginCedula").value = "";
  try { localStorage.removeItem(LAST_CEDULA_KEY); } catch (e) {}
  showScreen("screen-login");
});

// Ingreso automático: si este navegador ya inició sesión antes y la cédula sigue en la matrícula, entra directo
function tryAutoLogin() {
  let lastCedula = null;
  try { lastCedula = localStorage.getItem(LAST_CEDULA_KEY); } catch (e) {}
  if (!lastCedula) return false;
  const found = findInRoster(lastCedula);
  if (!found) return false;
  session.user = found;
  const badge = document.getElementById("userBadge");
  document.getElementById("userBadgeName").textContent = `${found.name} · C.C. ${found.cedula}`;
  badge.style.display = "flex";
  renderTopicsGrid();
  return true;
}

// ---------- Panel admin: agregar un empleado manualmente a la matrícula ----------
document.getElementById("toggleManualAdd").addEventListener("click", () => {
  const box = document.getElementById("manualAddBox");
  box.style.display = box.style.display === "none" ? "block" : "none";
});
document.getElementById("manualAddBtn").addEventListener("click", () => {
  const name = document.getElementById("manualNombre").value.trim();
  const cedula = document.getElementById("manualCedula").value.trim();
  const cargo = document.getElementById("manualCargo").value.trim();
  if (!name || !cedula) {
    alert("Escribe al menos el nombre completo y el número de cédula.");
    return;
  }
  const newEntry = { cedula, name, cargo, area: "", sede: "", correo: "" };
  const existingIdx = session.roster.findIndex((r) => String(r.cedula).trim() === cedula);
  if (existingIdx >= 0) session.roster[existingIdx] = newEntry;
  else session.roster.push(newEntry);
  document.getElementById("manualNombre").value = "";
  document.getElementById("manualCedula").value = "";
  document.getElementById("manualCargo").value = "";
  updateRosterCount();
});

function updateRosterCount() {
  const el = document.getElementById("rosterCurrentCount");
  if (el) el.textContent = `Matrícula actual en esta sesión: ${session.roster.length} empleado(s). Recuerda generar el archivo para publicar después de cualquier cambio.`;
}

// ---------- Carga de matrícula (.csv / .xlsx) ----------
document.getElementById("rosterFile").addEventListener("change", (e) => {
  const file = e.target.files[0];
  const hint = document.getElementById("rosterHint");
  if (!file) return;
  const reader = new FileReader();
  reader.onload = (evt) => {
    try {
      const data = new Uint8Array(evt.target.result);
      const wb = XLSX.read(data, { type: "array" });
      const sheet = wb.Sheets[wb.SheetNames[0]];
      const rows = XLSX.utils.sheet_to_json(sheet, { defval: "" });
      const parsed = rows.map((row) => {
        const get = (keys) => {
          for (const k of keys) {
            const foundKey = Object.keys(row).find((rk) => rk.trim().toLowerCase() === k);
            if (foundKey && String(row[foundKey]).trim() !== "") return String(row[foundKey]).trim();
          }
          return "";
        };
        return {
          cedula: get(["cedula", "cédula", "documento", "numero de documento", "número de documento"]),
          name: get(["nombres y apellidos", "nombre completo", "nombre", "nombres"]),
          cargo: get(["cargo"]),
          area: get(["area", "área", "proceso"]),
          sede: get(["sede", "ciudad"]),
          correo: get(["correo", "correo electronico", "correo electrónico", "email"]),
        };
      }).filter((r) => r.cedula);
      session.roster = parsed;
      hint.textContent = `Matrícula cargada: ${parsed.length} empleados. Recuerda generar el archivo para publicar para que quede incluida.`;
      hint.style.color = "var(--accent-dim)";
      updateRosterCount();
    } catch (err) {
      hint.textContent = "No pudimos leer ese archivo. Verifica que sea un .csv o .xlsx con una columna de cédula y una de nombre.";
      hint.style.color = "#C1121F";
    }
  };
  reader.readAsArrayBuffer(file);
});

// ============================================================
// Panel de administrador: bloqueo / desbloqueo de PILARES
// ============================================================
document.getElementById("openAdminBtn").addEventListener("click", () => {
  document.getElementById("adminPinGate").style.display = "block";
  document.getElementById("adminPanelBody").style.display = "none";
  document.getElementById("adminPinInput").value = "";
  document.getElementById("adminPinError").textContent = "";
  showScreen("screen-admin");
});
document.getElementById("backToLoginFromAdmin").addEventListener("click", () => showScreen("screen-login"));
document.getElementById("adminPinBtn").addEventListener("click", () => {
  const pin = document.getElementById("adminPinInput").value.trim();
  const errEl = document.getElementById("adminPinError");
  if (pin === getAdminPin()) {
    errEl.textContent = "";
    document.getElementById("adminPinGate").style.display = "none";
    document.getElementById("adminPanelBody").style.display = "block";
    renderCourseLockList();
    updateRosterCount();
    document.getElementById("brandName").value = session.branding.name;
    document.getElementById("brandNit").value = session.branding.nit;
    renderBrandLogoPreview();
  } else {
    errEl.textContent = "PIN incorrecto. Intenta de nuevo.";
  }
});

// ---------- Panel admin: marca de la empresa cliente ----------
document.getElementById("brandLogoInput").addEventListener("change", (e) => {
  const file = e.target.files[0];
  if (!file) return;
  const reader = new FileReader();
  reader.onload = (evt) => {
    session.branding.logo = evt.target.result;
    renderBrandLogoPreview();
    renderBrand();
  };
  reader.readAsDataURL(file);
});
document.getElementById("brandName").addEventListener("input", (e) => {
  session.branding.name = e.target.value.trim();
  renderBrand();
});
document.getElementById("brandNit").addEventListener("input", (e) => {
  session.branding.nit = e.target.value.trim();
});

function renderCourseLockList() {
  const wrap = document.getElementById("courseLockList");
  wrap.innerHTML = "";
  const locks = getLockState();
  Object.keys(PILLARS).forEach((key) => {
    const pillar = PILLARS[key];
    const unlocked = !!locks[key];
    const row = document.createElement("div");
    row.className = "lock-row";
    row.innerHTML = `
      <div class="lock-row-name"><span class="icon-sm">${ICONS[pillar.icon]}</span>${pillar.label} <span style="color:var(--muted); font-family:var(--mono); font-size:10.5px;">(${pillar.modules.length} módulos)</span></div>
      <div style="display:flex; align-items:center; gap:10px;">
        <span class="lock-status">${unlocked ? "Habilitado" : "Bloqueado"}</span>
        <button class="toggle ${unlocked ? "on" : ""}" data-key="${key}" aria-label="Alternar disponibilidad de ${pillar.label}"></button>
      </div>
    `;
    wrap.appendChild(row);
  });
  wrap.querySelectorAll(".toggle").forEach((btn) => {
    btn.addEventListener("click", () => {
      const key = btn.dataset.key;
      const nowUnlocked = !btn.classList.contains("on");
      setPillarUnlocked(key, nowUnlocked);
      renderCourseLockList();
      renderTopicsGrid();
    });
  });
}
document.getElementById("savePinBtn").addEventListener("click", () => {
  const newPin = document.getElementById("newPinInput").value.trim();
  const hint = document.getElementById("pinSavedHint");
  if (!/^\d{4,8}$/.test(newPin)) {
    hint.textContent = "El PIN debe tener entre 4 y 8 dígitos numéricos.";
    hint.style.color = "#C1121F";
    return;
  }
  setAdminPin(newPin);
  document.getElementById("newPinInput").value = "";
  hint.textContent = "PIN actualizado. Úsalo la próxima vez que entres al panel.";
  hint.style.color = "var(--accent-dim)";
});

// ============================================================
// Generar archivo único listo para publicar (matrícula incrustada)
// ============================================================
document.getElementById("generatePublishBtn").addEventListener("click", () => {
  const hint = document.getElementById("publishHint");
  if (!session.branding.name) {
    hint.textContent = "Escribe primero el nombre de la empresa cliente (sección 1) — así los certificados salen con su nombre en vez de uno genérico.";
    hint.style.color = "#C1121F";
    return;
  }
  if (session.roster.length === 0) {
    hint.textContent = "Ahora carga o agrega al menos un empleado a la matrícula (sección 2).";
    hint.style.color = "#C1121F";
    return;
  }

  // Guardar la vista actual para restaurarla después de generar el archivo
  const activeScreenId = document.querySelector(".screen.active").id;
  const badge = document.getElementById("userBadge");
  const badgeWasVisible = badge.style.display !== "none";
  const cedulaFieldValue = document.getElementById("loginCedula").value;

  // Poner la app en su estado "de fábrica": pantalla de ingreso, sin sesión iniciada visualmente
  document.querySelectorAll(".screen").forEach((s) => s.classList.remove("active"));
  document.getElementById("screen-login").classList.add("active");
  badge.style.display = "none";
  document.getElementById("loginCedula").value = "";
  document.getElementById("loginError").textContent = "";

  let html = "<!DOCTYPE html>\n" + document.documentElement.outerHTML;
  const rosterJson = JSON.stringify(session.roster);
  const locksJson = JSON.stringify(getLockState());
  const brandingJson = JSON.stringify(session.branding);
  html = html.replace(/let EMBEDDED_ROSTER = \[[\s\S]*?\];/, `let EMBEDDED_ROSTER = ${rosterJson};`);
  html = html.replace(/let EMBEDDED_LOCKS = (?:null|\{[\s\S]*?\});/, `let EMBEDDED_LOCKS = ${locksJson};`);
  html = html.replace(/let EMBEDDED_BRANDING = \{[\s\S]*?\};/, `let EMBEDDED_BRANDING = ${brandingJson};`);
  html = html.replace(/<title>[\s\S]*?<\/title>/, `<title>Centro de Formación · ${session.branding.name}</title>`);

  const safeName = session.branding.name.toLowerCase()
    .normalize("NFD").replace(/[\u0300-\u036f]/g, "")
    .replace(/[^a-z0-9]+/g, "-").replace(/(^-|-$)/g, "");

  const blob = new Blob([html], { type: "text/html;charset=utf-8" });
  const url = URL.createObjectURL(blob);
  const a = document.createElement("a");
  a.href = url;
  a.download = `centro-formacion-${safeName || "empresa"}.html`;
  document.body.appendChild(a);
  a.click();
  document.body.removeChild(a);
  setTimeout(() => URL.revokeObjectURL(url), 4000);

  // Restaurar la vista del administrador
  document.querySelectorAll(".screen").forEach((s) => s.classList.remove("active"));
  document.getElementById(activeScreenId).classList.add("active");
  if (badgeWasVisible) badge.style.display = "flex";
  document.getElementById("loginCedula").value = cedulaFieldValue;

  hint.textContent = `Archivo descargado para "${session.branding.name}" con ${session.roster.length} empleado(s) y el logo/NIT incluidos. Súbelo a tu hosting y comparte esa URL — sus certificados ya saldrán con esta marca.`;
  hint.style.color = "var(--accent-dim)";
});

// ---------- Eventos generales ----------
document.getElementById("searchBtn").addEventListener("click", handleSearch);
document.getElementById("searchInput").addEventListener("keydown", (e) => { if (e.key === "Enter") handleSearch(); });

// ---------- Inicialización ----------
if (Array.isArray(EMBEDDED_ROSTER) && EMBEDDED_ROSTER.length > 0) {
  session.roster = EMBEDDED_ROSTER.slice();
}
if (EMBEDDED_BRANDING && typeof EMBEDDED_BRANDING === "object") {
  session.branding = Object.assign({ logo: "", name: "", nit: "" }, EMBEDDED_BRANDING);
}
renderBrand();
renderTopicsGrid();
if (tryAutoLogin()) {
  showScreen("screen-home");
} else {
  showScreen("screen-login");
}

</script>


</body></html>
