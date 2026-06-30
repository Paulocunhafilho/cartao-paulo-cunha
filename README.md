<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0,viewport-fit=cover"/>
<meta name="theme-color" content="#07112a"/>
<title>Paulo Cunha – Investment Advisor</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet"/>
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
--navy:#07112a;--navy-mid:#0d1e3d;
--gold:#c9a84c;--gold-light:#e8c97a;--gold-dark:#9a7530;
--white:#ffffff;--gray:#c8d4e8;--radius:14px}
html,body{background:var(--navy);font-family:'Inter',sans-serif;
color:var(--white);-webkit-font-smoothing:antialiased;min-height:100%}
.card{max-width:420px;margin:0 auto;min-height:100dvh;
background:radial-gradient(ellipse at 80% 5%,rgba(201,168,76,0.08) 0%,transparent 55%),
radial-gradient(ellipse at 20% 95%,rgba(201,168,76,0.05) 0%,transparent 50%),
linear-gradient(175deg,#07112a 0%,#0d1e3d 45%,#081528 100%);
display:flex;flex-direction:column;position:relative;overflow:hidden}
.card::before{content:'';position:absolute;top:0;left:0;right:0;height:3px;
background:linear-gradient(90deg,transparent 0%,#9a7530 20%,#e8c97a 50%,#9a7530 80%,transparent 100%);z-index:10}
.orb{position:absolute;top:-110px;right:-110px;width:320px;height:320px;
border-radius:50%;border:1px solid rgba(201,168,76,0.09);pointer-events:none}
.orb::after{content:'';position:absolute;inset:22px;border-radius:50%;
border:1px solid rgba(201,168,76,0.05)}
.deco{position:absolute;width:1px;pointer-events:none;
background:linear-gradient(to bottom,transparent,rgba(201,168,76,0.30),transparent)}
.deco-r{top:55px;right:26px;height:170px}
.deco-l{top:75px;left:26px;height:110px}
.hero{display:flex;flex-direction:column;align-items:center;
padding:48px 24px 22px;position:relative;z-index:1}
.photo-ring{width:136px;height:136px;border-radius:50%;padding:3px;
background:conic-gradient(#9a7530 0deg,#e8c97a 90deg,#c9a84c 180deg,#e8c97a 270deg,#9a7530 360deg);
margin-bottom:22px;flex-shrink:0;box-shadow:0 0 36px rgba(201,168,76,0.22)}
.photo-ring img{width:100%;height:100%;border-radius:50%;
object-fit:cover;object-position:center top;display:block;border:3px solid #0d1e3d}
.photo-fallback{width:100%;height:100%;border-radius:50%;background:#0d1e3d;
display:flex;align-items:center;justify-content:center;font-size:50px;border:3px solid #0d1e3d}
.name{font-family:'Playfair Display',serif;font-size:30px;font-weight:700;
color:#fff;text-align:center;letter-spacing:0.4px;line-height:1.15;margin-bottom:6px}
.title-en{font-size:11px;font-weight:600;color:#e8c97a;letter-spacing:3.5px;
text-transform:uppercase;text-align:center;margin-bottom:16px}
.badge{display:flex;align-items:center;gap:10px;
background:rgba(201,168,76,0.08);border:1px solid rgba(201,168,76,0.25);
border-radius:100px;padding:8px 18px}
.badge-icon{font-size:18px;flex-shrink:0}
.badge-text{font-size:10.5px;font-weight:600;letter-spacing:1px;
text-transform:uppercase;color:#c8d4e8;line-height:1.45;text-align:center}
.badge-text strong{display:block;color:#e8c97a;font-size:11px}
.rule{width:calc(100% - 48px);height:1px;margin:0 auto;
background:linear-gradient(90deg,transparent,#9a7530 25%,#c9a84c 50%,#9a7530 75%,transparent);opacity:0.50}
.btns{padding:22px 20px 10px;display:flex;flex-direction:column;gap:11px;position:relative;z-index:1}
.btn{display:flex;align-items:center;gap:14px;padding:14px 18px;
border-radius:var(--radius);text-decoration:none;font-family:'Inter',sans-serif;
font-size:13px;font-weight:500;transition:transform .14s ease,filter .14s ease;
cursor:pointer;border:none;width:100%;text-align:left;-webkit-tap-highlight-color:transparent}
.btn:active{transform:scale(0.975);filter:brightness(0.90)}
.btn-gold{background:linear-gradient(135deg,#b8892e 0%,#d4a843 40%,#e8c97a 70%,#c9a84c 100%);
color:#07112a;font-weight:700;box-shadow:0 6px 24px rgba(201,168,76,0.30),0 2px 8px rgba(0,0,0,0.28)}
.btn-glass{background:rgba(255,255,255,0.055);color:#fff;
border:1px solid rgba(255,255,255,0.10);backdrop-filter:blur(6px);-webkit-backdrop-filter:blur(6px)}
.btn-glass:hover{background:rgba(255,255,255,0.09)}
.bico{width:38px;height:38px;border-radius:10px;display:flex;
align-items:center;justify-content:center;font-size:19px;flex-shrink:0}
.btn-gold .bico{background:rgba(7,17,42,0.18)}
.btn-glass .bico{background:rgba(201,168,76,0.10)}
.bico svg{width:22px;height:22px;fill:currentColor}
.btn-gold .bico svg{color:#07112a}
.btn-glass .bico svg{color:#e8c97a}
.blbl{flex:1}
.blbl .m{display:block;font-size:13px;font-weight:700;letter-spacing:.8px;text-transform:uppercase}
.blbl .s{display:block;font-size:11px;font-weight:400;opacity:.65;margin-top:2px;letter-spacing:0;text-transform:none}
.arr{font-size:18px;opacity:.38;flex-shrink:0}
.btns2{padding:10px 20px 18px;display:grid;grid-template-columns:1fr 1fr;gap:11px;position:relative;z-index:1}
.btn2{display:flex;flex-direction:column;align-items:center;justify-content:center;
gap:7px;padding:15px 12px;border-radius:var(--radius);text-decoration:none;
background:rgba(201,168,76,0.07);border:1px solid rgba(201,168,76,0.22);
color:#e8c97a;font-family:'Inter',sans-serif;font-size:11px;font-weight:700;
letter-spacing:1px;text-transform:uppercase;text-align:center;cursor:pointer;
transition:transform .14s ease,background .14s ease;-webkit-tap-highlight-color:transparent}
.btn2:active{transform:scale(0.96);background:rgba(201,168,76,0.14)}
.btn2 svg{width:22px;height:22px;fill:#e8c97a}
.btn2 .sub{display:block;font-size:10px;font-weight:400;color:#c8d4e8;
letter-spacing:0;text-transform:none;margin-top:1px}
footer{margin-top:auto;position:relative;z-index:1}
.foot-brand{margin:4px 20px 0;background:rgba(255,255,255,0.04);
border:1px solid rgba(201,168,76,0.18);border-radius:var(--radius);padding:18px 20px 16px}
.foot-logos{display:flex;align-items:center;justify-content:center;gap:18px;margin-bottom:14px}
.logo-safra{display:flex;align-items:center;gap:9px}
.safra-ico{width:36px;height:36px;border-radius:50%;
background:linear-gradient(135deg,#1a3a6e,#0d2550);
border:1.5px solid rgba(201,168,76,0.40);display:flex;
align-items:center;justify-content:center;font-size:16px;flex-shrink:0}
.safra-txt span:first-child{display:block;font-family:'Playfair Display',serif;
font-size:17px;font-weight:700;color:#fff;letter-spacing:.5px}
.safra-txt span:last-child{display:block;font-size:10px;font-weight:600;
color:#c9a84c;letter-spacing:2px;text-transform:uppercase}
.logo-div{width:1px;height:44px;
background:linear-gradient(to bottom,transparent,rgba(201,168,76,0.40),transparent);flex-shrink:0}
.logo-mpx{text-align:right;line-height:1.2}
.logo-mpx .mpx-big{display:block;font-size:20px;font-weight:800;color:#fff;letter-spacing:-.5px}
.logo-mpx .mpx-big em{color:#e8c97a;font-style:normal}
.logo-mpx .mpx-sub{display:block;font-size:9.5px;font-weight:600;
color:#c9a84c;letter-spacing:1.8px;text-transform:uppercase}
.foot-addr{text-align:center;font-size:11.5px;color:#c8d4e8;opacity:.72;line-height:1.75}
.foot-privacy{text-align:center;font-size:10.5px;color:#c8d4e8;opacity:.38;padding:12px 24px 28px}
#toast{position:fixed;bottom:36px;left:50%;
transform:translateX(-50%) translateY(90px);
background:rgba(201,168,76,0.97);color:#07112a;
font-size:13px;font-weight:700;padding:12px 26px;border-radius:100px;
white-space:nowrap;z-index:9999;
transition:transform .35s cubic-bezier(.34,1.56,.64,1);
pointer-events:none;box-shadow:0 8px 24px rgba(0,0,0,0.30)}
#toast.show{transform:translateX(-50%) translateY(0)}
@media(min-width:440px){.card{border-radius:28px;margin:28px auto;
min-height:auto;box-shadow:0 40px 100px rgba(0,0,0,0.55)}}
</style>
</head>
<body>
<div class="card">
<div class="orb"></div>
<div class="deco deco-r"></div>
<div class="deco deco-l"></div>

<div class="hero">
<div class="photo-ring" id="photoRing">
<img src="paulo.jpg" alt="Paulo Cunha" id="photoImg"/>
</div>
<h1 class="name">Paulo Cunha</h1>
<p class="title-en">Investment Advisor</p>
<div class="badge">
<span class="badge-icon">🏅</span>
<div class="badge-text">
Assessor de Investimentos
<strong>Credenciado à Safra Invest</strong>
</div>
</div>
</div>

<div class="rule"></div>

<div class="btns">

<a class="btn btn-gold" href="paulo-cunha.vcf" download>
<div class="bico">
<svg viewBox="0 0 24 24"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 14H4V6h16v12zM6 10h2v2H6zm0 4h8v2H6zm10 0h2v2h-2zm-6-4h6v2h-6z"/></svg>
</div>
<div class="blbl">
<span class="m">Salvar Contato</span>
<span class="s">Adicionar à agenda</span>
</div>
<span class="arr">›</span>
</a>

<a class="btn btn-glass"
href="https://wa.me/5511991507557?text=Olá%20Paulo%2C%20vim%20pelo%20seu%20cartão%20digital!"
target="_blank" rel="noopener">
<div class="bico">
<svg viewBox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/><path d="M12 0C5.373 0 0 5.373 0 12c0 2.127.558 4.122 1.532 5.852L.057 23.5l5.797-1.52A11.93 11.93 0 0012 24c6.627 0 12-5.373 12-12S18.627 0 12 0zm0 21.894a9.877 9.877 0 01-5.031-1.378l-.36-.214-3.742.981 1-3.642-.235-.374A9.865 9.865 0 012.106 12C2.106 6.58 6.58 2.106 12 2.106S21.894 6.58 21.894 12 17.42 21.894 12 21.894z"/></svg>
</div>
<div class="blbl">
<span class="m">WhatsApp</span>
<span class="s">Fale comigo · (11) 99150-7557</span>
</div>
<span class="arr">›</span>
</a>

<a class="btn btn-glass"
href="https://wa.me/c/5511991507557"
target="_blank" rel="noopener">
<div class="bico">
<svg viewBox="0 0 24 24"><path d="M18 2H6c-1.1 0-2 .9-2 2v16c0 1.1.9 2 2 2h12c1.1 0 2-.9 2-2V4c0-1.1-.9-2-2-2zM6 4h5v8l-2.5-1.5L6 12V4zm0 15l3-3.86 2.14 2.58 3-3.86L18 19H6z"/></svg>
</div>
<div class="blbl">
<span class="m">Catálogo de Investimentos</span>
<span class="s">Ver produtos no WhatsApp</span>
</div>
<span class="arr">›</span>
</a>

<a class="btn btn-glass"
href="https://www.mpxprimecapital.com.br"
target="_blank" rel="noopener">
<div class="bico">
<svg viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 17.93c-3.95-.49-7-3.85-7-7.93 0-.62.08-1.21.21-1.79L9 15v1c0 1.1.9 2 2 2v1.93zm6.9-2.54c-.26-.81-1-1.39-1.9-1.39h-1v-3c0-.55-.45-1-1-1H8v-2h2c.55 0 1-.45 1-1V7h2c1.1 0 2-.9 2-2v-.41c2.93 1.19 5 4.06 5 7.41 0 2.08-.8 3.97-2.1 5.39z"/></svg>
</div>
<div class="blbl">
<span class="m">MPX Prime Capital</span>
<span class="s">mpxprimecapital.com.br</span>
</div>
<span class="arr">›</span>
</a>

<a class="btn btn-glass"
href="https://www.mpxprime.com.br"
target="_blank" rel="noopener">
<div class="bico">
<svg viewBox="0 0 24 24"><path d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"/></svg>
</div>
<div class="blbl">
<span class="m">MPX Prime</span>
<span class="s">mpxprime.com.br</span>
</div>
<span class="arr">›</span>
</a>

<a class="btn btn-glass"
href="mailto:paulo.cunha@mpxprimecapital.com.br">
<div class="bico">
<svg viewBox="0 0 24 24"><path d="M20 4H4c-1.1 0-2 .9-2 2v12c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
</div>
<div class="blbl">
<span class="m">Enviar E-mail</span>
<span class="s">paulo.cunha@mpxprimecapital.com.br</span>
</div>
<span class="arr">›</span>
</a>

</div>
<div class="rule" style="margin:4px auto"></div>

<div class="btns2">

<button class="btn2" onclick="compartilhar()">
<svg viewBox="0 0 24 24"><path d="M18 16.08c-.76 0-1.44.3-1.96.77L8.91 12.7c.05-.23.09-.46.09-.7s-.04-.47-.09-.7l7.05-4.11c.54.5 1.25.81 2.04.81 1.66 0 3-1.34 3-3s-1.34-3-3-3-3 1.34-3 3c0 .24.04.47.09.7L8.04 9.81C7.5 9.31 6.79 9 6 9c-1.66 0-3 1.34-3 3s1.34 3 3 3c.79 0 1.5-.31 2.04-.81l7.12 4.16c-.05.21-.08.43-.08.65 0 1.61 1.31 2.92 2.92 2.92s2.92-1.31 2.92-2.92-1.31-2.92-2.92-2.92z"/></svg>
<span>Compartilhar</span>
<span class="sub">Enviar meu cartão</span>
</button>

<a class="btn2"
href="https://maps.google.com/?q=Rua+do+Bosque+1484+Barra+Funda+São+Paulo+SP"
target="_blank" rel="noopener">
<svg viewBox="0 0 24 24"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/></svg>
<span>Localização</span>
<span class="sub">Abrir no mapa</span>
</a>

</div>

<div class="rule" style="margin:0 auto 4px"></div>

<footer>
<div class="foot-brand">
<div class="foot-logos">
<div class="logo-safra">
<div class="safra-ico">💰</div>
<div class="safra-txt">
<span>Safra</span>
<span>Invest</span>
</div>
</div>
<div class="logo-div"></div>
<div class="logo-mpx">
<span class="mpx-big">MP<em>X</em></span>
<span class="mpx-sub">Prime Capital</span>
</div>
</div>
<p class="foot-addr">
📍 Rua do Bosque, 1484 · 6° andar · Conjunto 611<br/>
Barra Funda · São Paulo / SP · CEP 01136-001<br/>
☎ (11) 3500-5940
</p>
</div>
<p class="foot-privacy">🔒 Seus dados estão protegidos.</p>
</footer>

</div>
<div id="toast"></div>

<script>
document.getElementById('photoImg').onerror=function(){
this.style.display='none';
var fb=document.createElement('div');
fb.className='photo-fallback';
fb.textContent='👤';
document.getElementById('photoRing').appendChild(fb);
};
async function compartilhar(){
var p={
title:'Paulo Cunha – Investment Advisor',
text:'Cartão digital de Paulo Cunha · Assessor de Investimentos credenciado à Safra Invest · MPX Prime Capital.',
url:window.location.href
};
if(navigator.share){
try{await navigator.share(p);}catch(_){}
}else{
try{
await navigator.clipboard.writeText(window.location.href);
toast('🔗 Link copiado!');
}catch{
toast('📋 Copie o link da barra de endereço');
}
}
}
function toast(msg,ms){
ms=ms||2800;
var el=document.getElementById('toast');
el.textContent=msg;
el.classList.add('show');
setTimeout(function(){el.classList.remove('show');},ms);
}
</script>
</body>
</html>
