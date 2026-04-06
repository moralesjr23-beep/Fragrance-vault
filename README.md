
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>The Vault — AJ's Collection</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400&family=Josefin+Sans:wght@100;200;300;400&display=swap" rel="stylesheet">
<style>
:root {
  --ink:#ede8de;--parchment:#2a1e10;--gold:#8a5e1e;--gold-light:#6b4a18;--gold-dim:#a07830;
  --smoke:#ffffff;--ash:#e8e2d8;--char:#dfd9cf;--dove:#6a5a4a;--cream:#1a1208;
  --rose:#b05a42;--aqua:#2a6575;--forest:#2d5028;--ab:rgba(140,100,40,0.18);
}
[data-theme="dark"] {
  --ink:#0e0c09;--parchment:#e8ddd0;--gold:#c9a84c;--gold-light:#e8d5a3;--gold-dim:#8a6e2e;
  --smoke:#181410;--ash:#252018;--char:#1e1a14;--dove:#8a7a6a;--cream:#ede8dc;
  --rose:#c06050;--aqua:#4a8595;--forest:#4d7048;--ab:rgba(201,168,76,0.18);
}
[data-theme="dark"] body{background:#0e0c09;color:#e8ddd0;}
[data-theme="dark"] .header{background:rgba(14,12,9,0.97);}
[data-theme="dark"] .nav-bar{background:#181410;}
[data-theme="dark"] .card,[data-theme="dark"] .acard,[data-theme="dark"] .lcard,
[data-theme="dark"] .ritem,[data-theme="dark"] .dnaf,[data-theme="dark"] .ins-card,
[data-theme="dark"] .wl-card,[data-theme="dark"] .sug-card,[data-theme="dark"] .lcard,
[data-theme="dark"] .morning-card{background:#181410;border-color:rgba(201,168,76,.12);}
[data-theme="dark"] .card:hover,[data-theme="dark"] .ritem:hover,[data-theme="dark"] .dnaf:hover{background:#252018;}
[data-theme="dark"] .modal,[data-theme="dark"] .add-modal{background:#181410;border-color:rgba(201,168,76,.15);}
[data-theme="dark"] .confirm-box{background:#1e1a14;}
[data-theme="dark"] select,[data-theme="dark"] .sw input,[data-theme="dark"] .tag-input,
[data-theme="dark"] textarea.notes,[data-theme="dark"] .alf input,[data-theme="dark"] .alf textarea,
[data-theme="dark"] .add-modal input,[data-theme="dark"] .add-modal select{background:#252018;border-color:rgba(201,168,76,.18);color:#e8ddd0;}
[data-theme="dark"] .ql-panel{background:#181410;border-color:rgba(201,168,76,.15);}
[data-theme="dark"] .ql-item:hover{background:#252018;}
[data-theme="dark"] .weather-bar,[data-theme="dark"] .suggester,[data-theme="dark"] .alf{background:#1e1a14;}
[data-theme="dark"] .dna-panel{background:#1e1a14;}
[data-theme="dark"] .wl-form{background:#1e1a14;}
[data-theme="dark"] .grid{background:rgba(201,168,76,.08);}
[data-theme="dark"] .agrid,[data-theme="dark"] .lab-grid,[data-theme="dark"] .ins-grid,
[data-theme="dark"] .wl-grid,[data-theme="dark"] .sug-cards,[data-theme="dark"] .dna-hero{background:rgba(201,168,76,.08);}
[data-theme="dark"] #page-collection,[data-theme="dark"] #page-classification,
[data-theme="dark"] #page-layering,[data-theme="dark"] #page-analytics,
[data-theme="dark"] #page-rotation,[data-theme="dark"] #page-starred,
[data-theme="dark"] #page-weather,[data-theme="dark"] #page-insights,
[data-theme="dark"] #page-wishlist,[data-theme="dark"] #page-search,
[data-theme="dark"] #page-bottle,[data-theme="dark"] #page-importexport,
[data-theme="dark"] #page-duaadvisor{background:#0e0c09;}
[data-theme="dark"] .main{background:#0e0c09;}
*{margin:0;padding:0;box-sizing:border-box;}
body{background:#f0ebe3;color:var(--parchment);font-family:'Josefin Sans',sans-serif;font-weight:400;min-height:100vh;overflow-x:hidden;}
body::before{content:'';position:fixed;inset:0;background-image:url("data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='n'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23n)' opacity='0.035'/%3E%3C/svg%3E");pointer-events:none;z-index:9999;opacity:.7;}

.header{display:flex;align-items:center;justify-content:space-between;padding:14px 20px;border-bottom:1px solid var(–ab);position:sticky;top:0;background:rgba(247,243,238,0.97);backdrop-filter:blur(16px);z-index:100;gap:12px;flex-wrap:wrap;}
.brand-name{font-family:‘Cormorant Garamond’,serif;font-size:24px;font-weight:600;letter-spacing:.2em;color:var(–gold);text-transform:uppercase;}
.brand-sub{font-size:7.5px;letter-spacing:.26em;color:var(–dove);text-transform:uppercase;margin-top:1px;}
.stats-strip{display:flex;gap:16px;align-items:center;}
.stat{text-align:center;}
.stat-num{font-family:‘Cormorant Garamond’,serif;font-size:22px;color:var(–gold);display:block;line-height:1;font-weight:600;}
.stat-label{font-size:7.5px;letter-spacing:.18em;color:var(–dove);text-transform:uppercase;margin-top:2px;font-weight:600;}
.sdiv{width:1px;height:24px;background:var(–ab);}
.add-btn{display:flex;align-items:center;gap:6px;padding:8px 16px;background:transparent;border:1px solid var(–gold);color:var(–gold);font-family:‘Josefin Sans’,sans-serif;font-size:8.5px;letter-spacing:.2em;text-transform:uppercase;cursor:pointer;transition:all .2s;}
.add-btn:hover{background:rgba(201,168,76,.1);}

.nav-bar{display:flex;padding:0 8px;border-bottom:1px solid rgba(140,100,40,.12);background:#ece6dc;overflow-x:auto;}
.nav-bar::-webkit-scrollbar{display:none;}
.nav-tab{padding:11px 14px;font-size:8.5px;letter-spacing:.15em;text-transform:uppercase;color:var(–dove);cursor:pointer;border-bottom:2px solid transparent;transition:all .2s;white-space:nowrap;background:none;border-left:none;border-right:none;border-top:none;font-family:‘Josefin Sans’,sans-serif;font-weight:600;}
.nav-tab:hover{color:var(–gold-light);}
.nav-tab.active{color:var(–gold);border-bottom-color:var(–gold);}

.main{padding:18px 16px;max-width:1700px;margin:0 auto;}@media(min-width:768px){.main{padding:28px 36px;}}
.page{display:none;background:#f0ebe3;}
.page.active{display:block;}

.toolbar{display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-bottom:20px;}.toolbar .sw{grid-column:1/-1;}
.sw{position:relative;flex:1;min-width:200px;}
.sw input{width:100%;background:#ffffff;border:1px solid rgba(140,100,40,.25);color:var(–parchment);padding:9px 13px 9px 35px;font-family:‘Josefin Sans’,sans-serif;font-size:10px;letter-spacing:.1em;outline:none;transition:border-color .2s;border-radius:0;}
.sw input:focus{border-color:rgba(201,168,76,.4);}
.sw input::placeholder{color:var(–dove);}
.si{position:absolute;left:11px;top:50%;transform:translateY(-50%);color:var(–dove);font-size:14px;}
select{background:#ffffff;border:1px solid rgba(140,100,40,.25);color:var(–parchment);padding:8px 11px;font-family:‘Josefin Sans’,sans-serif;font-size:9px;letter-spacing:.13em;text-transform:uppercase;cursor:pointer;outline:none;border-radius:0;-webkit-appearance:none;appearance:none;}
select option{background:#ffffff;}

.sec-hdr{display:flex;align-items:baseline;gap:12px;margin-bottom:18px;}
.sec-title{font-family:‘Cormorant Garamond’,serif;font-size:22px;font-weight:600;color:var(–cream);letter-spacing:.04em;}
.sec-ct{font-size:8.5px;letter-spacing:.2em;color:var(–dove);text-transform:uppercase;}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(260px,1fr));gap:1px;background:rgba(140,100,40,.12);}@media(max-width:600px){.grid{grid-template-columns:1fr;}}

.card{background:#ffffff;padding:18px 20px;cursor:pointer;transition:background .15s;position:relative;overflow:hidden;animation:fu .3s ease;border-bottom:1px solid rgba(140,100,40,.06);}
@keyframes fu{from{opacity:0;transform:translateY(7px);}to{opacity:1;transform:none;}}
.card:hover{background:#f0ebe3;}
.card::before{content:’’;position:absolute;left:0;top:0;bottom:0;width:3px;}
.card.ss::before{background:#2a6575;}
.card.fw::before{background:#8a5e1e;}
.card.yr::before{background:#8a7a6a;}
.card-house{font-size:7px;letter-spacing:.2em;text-transform:uppercase;color:var(–gold);margin-bottom:3px;font-weight:700;}
.card-name{font-family:‘Cormorant Garamond’,serif;font-size:18px;color:var(–cream);line-height:1.15;margin-bottom:5px;font-weight:600;}
.card-insp{font-size:9.5px;color:var(–dove);letter-spacing:.02em;margin-bottom:9px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;font-style:italic;font-weight:400;}
.card-tags{display:flex;gap:5px;flex-wrap:wrap;}
.tag{font-size:7.5px;letter-spacing:.12em;text-transform:uppercase;padding:3px 8px;border:1px solid;font-weight:600;border-radius:0;}
.td{border-color:rgba(176,90,66,.4);color:var(–rose);}
.to{border-color:rgba(58,117,133,.4);color:var(–aqua);}
.te{border-color:rgba(201,168,76,.3);color:var(–gold-dim);}
.tc{border-color:rgba(107,99,88,.4);color:var(–dove);}
.ts{border-color:rgba(61,96,56,.4);color:var(–forest);}
.tsp{border-color:rgba(201,168,76,.55);color:var(–gold);}
.tsea{border-color:rgba(201,168,76,.1);color:var(–dove);}
.tbase{border-color:rgba(201,168,76,.5);color:var(–gold);font-size:6.5px;}
.card-star{position:absolute;top:11px;right:13px;color:var(–gold);font-size:12px;opacity:0;transition:opacity .2s;}
.card.starred .card-star{opacity:1;}
.card-del{position:absolute;bottom:9px;right:11px;font-size:10px;color:var(–dove);opacity:0;transition:opacity .2s;background:none;border:none;cursor:pointer;padding:3px;line-height:1;}
.card:hover .card-del{opacity:1;}
.card-del:hover{color:var(–rose);}

/* MODAL SHARED */
.overlay{position:fixed;inset:0;background:rgba(9,8,6,.88);z-index:200;display:flex;align-items:center;justify-content:center;backdrop-filter:blur(5px);}
.overlay.hidden{display:none!important;}
@keyframes sm{from{transform:translateY(16px);opacity:0;}to{transform:none;opacity:1;}}
.modal,.add-modal,.confirm-box{animation:sm .22s ease;}

/* DETAIL MODAL */
.modal{background:#ffffff;border:1px solid rgba(140,100,40,.2);max-width:640px;width:92vw;max-height:88vh;overflow-y:auto;position:relative;}
.modal::-webkit-scrollbar{width:3px;}
.modal::-webkit-scrollbar-thumb{background:var(–gold-dim);}
.mh{padding:26px 30px 20px;border-bottom:1px solid rgba(201,168,76,.09);position:relative;}
.m-house{font-size:7.5px;letter-spacing:.3em;color:var(–gold);text-transform:uppercase;margin-bottom:5px;}
.m-name{font-family:‘Cormorant Garamond’,serif;font-size:27px;color:var(–cream);line-height:1.1;margin-bottom:5px;font-weight:600;}
.m-insp{font-family:‘Cormorant Garamond’,serif;font-style:italic;font-size:14px;color:var(–dove);}
.mcl{position:absolute;top:16px;right:20px;background:none;border:none;color:var(–dove);font-size:17px;cursor:pointer;font-family:‘Josefin Sans’,sans-serif;transition:color .2s;padding:4px 8px;}
.mcl:hover{color:var(–gold);}
.mb{padding:22px 30px;}
.row{display:flex;gap:18px;margin-bottom:16px;flex-wrap:wrap;}
.field{flex:1;min-width:110px;}
.fl{font-size:8px;letter-spacing:.2em;text-transform:uppercase;color:var(–gold);margin-bottom:5px;font-weight:700;}
.fv{font-family:‘Cormorant Garamond’,serif;font-size:14px;color:var(–cream);}
.mdiv{height:1px;background:rgba(201,168,76,.06);margin:16px 0;}
textarea.notes{width:100%;background:#f0ebe3;border:1px solid rgba(140,100,40,.2);color:var(–cream);font-family:‘Cormorant Garamond’,serif;font-size:14px;line-height:1.6;padding:11px 13px;resize:vertical;min-height:68px;outline:none;transition:border-color .2s;}
textarea.notes:focus{border-color:rgba(201,168,76,.32);}
textarea.notes::placeholder{color:var(–dove);font-style:italic;}
.btn-row{display:flex;gap:7px;flex-wrap:wrap;margin-top:11px;}
.btn{display:inline-flex;align-items:center;gap:5px;padding:7px 15px;background:transparent;border:1px solid;font-family:‘Josefin Sans’,sans-serif;font-size:8.5px;letter-spacing:.15em;text-transform:uppercase;cursor:pointer;transition:all .2s;font-weight:600;}
.btn-gold{border-color:rgba(201,168,76,.35);color:var(–gold);}
.btn-gold:hover{background:rgba(201,168,76,.08);border-color:var(–gold);}
.btn-muted{border-color:rgba(107,99,88,.28);color:var(–dove);}
.btn-muted:hover{border-color:var(–dove);color:var(–cream);}
.btn-danger{border-color:rgba(176,90,66,.28);color:var(–rose);}
.btn-danger:hover{background:rgba(176,90,66,.08);border-color:var(–rose);}
.stars{display:flex;gap:3px;}
.star{font-size:15px;cursor:pointer;color:#ccc;transition:color .1s;}
.star.lit{color:var(–gold);}
.star:hover{color:var(–gold-light);}
.wear-entry{display:flex;justify-content:space-between;padding:6px 0;border-bottom:1px solid rgba(201,168,76,.04);font-size:10px;color:var(–dove);}
.wear-date{color:var(–cream);}

/* DNA pills */
.class-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:4px;}
.cpill{padding:5px 9px;border:1px solid var(–ab);background:rgba(201,168,76,.03);font-size:7.5px;letter-spacing:.13em;text-transform:uppercase;color:var(–gold-light);cursor:pointer;transition:all .2s;text-align:center;}
.cpill.sel{background:rgba(201,168,76,.14);border-color:var(–gold);color:var(–gold);}
.cpill:hover{border-color:rgba(201,168,76,.38);}

/* Layering in modal */
.lc-row{display:flex;align-items:flex-start;gap:9px;padding:9px 0;border-bottom:1px solid rgba(201,168,76,.04);}
.lc-names{font-family:‘Cormorant Garamond’,serif;font-size:14px;color:var(–cream);margin-bottom:2px;}
.lc-ratio{font-size:7.5px;letter-spacing:.12em;text-transform:uppercase;color:var(–gold-dim);}
.lc-desc{font-size:9.5px;color:var(–dove);line-height:1.5;margin-top:3px;}
.lc-del{background:none;border:none;color:var(–dove);cursor:pointer;font-size:11px;padding:3px;transition:color .2s;flex-shrink:0;}
.lc-del:hover{color:var(–rose);}

/* Add layer form */
.alf{background:#ede8de;border:1px solid rgba(140,100,40,.18);padding:13px;margin-top:9px;}
.alf input,.alf textarea{width:100%;background:#ffffff;border:1px solid rgba(140,100,40,.15);color:var(–parchment);padding:7px 10px;font-family:‘Josefin Sans’,sans-serif;font-size:9.5px;letter-spacing:.07em;outline:none;margin-bottom:7px;}
.alf textarea{font-family:‘Cormorant Garamond’,serif;font-size:13px;resize:vertical;min-height:50px;}
.alf input::placeholder,.alf textarea::placeholder{color:var(–dove);}

/* ADD BOTTLE MODAL */
.add-modal{background:#ffffff;border:1px solid rgba(140,100,40,.2);max-width:540px;width:92vw;max-height:88vh;overflow-y:auto;position:relative;}
.add-modal::-webkit-scrollbar{width:3px;}
.add-modal::-webkit-scrollbar-thumb{background:var(–gold-dim);}
.add-modal input,.add-modal select,.add-modal textarea{width:100%;background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(–parchment);padding:9px 12px;font-family:‘Josefin Sans’,sans-serif;font-size:10px;letter-spacing:.07em;outline:none;margin-bottom:9px;transition:border-color .2s;}
.add-modal input:focus,.add-modal select:focus{border-color:rgba(201,168,76,.38);}
.add-modal input::placeholder{color:var(–dove);}
.add-modal select option{background:var(–ash);}
.flabel{font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(–gold-dim);margin-bottom:4px;display:block;}
.form-row{display:grid;grid-template-columns:1fr 1fr;gap:11px;}

/* ANALYTICS */
.agrid{display:grid;grid-template-columns:repeat(auto-fit,minmax(250px,1fr));gap:1px;background:rgba(140,100,40,.15);}
.acard{background:#ffffff;padding:24px 26px;}
.atitle{font-size:8px;letter-spacing:.2em;text-transform:uppercase;color:var(–gold);margin-bottom:14px;font-weight:700;}
.br{display:flex;align-items:center;gap:8px;margin-bottom:8px;}
.blbl{font-size:9.5px;letter-spacing:.03em;color:var(–cream);width:118px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis;flex-shrink:0;font-weight:500;}
.btrack{flex:1;height:2px;background:rgba(201,168,76,.08);}
.bfill{height:2px;background:linear-gradient(90deg,var(–gold-dim),var(–gold));transition:width .6s ease;}
.bnum{font-size:8.5px;color:var(–gold);width:20px;text-align:right;flex-shrink:0;}
.bignum{font-family:‘Cormorant Garamond’,serif;font-size:48px;font-weight:300;color:var(–gold);line-height:1;margin-bottom:3px;}
.biglbl{font-size:8px;letter-spacing:.16em;text-transform:uppercase;color:var(–dove);}
.dw{display:flex;align-items:center;gap:18px;}
.li{display:flex;align-items:center;gap:7px;margin-bottom:6px;font-size:9px;color:var(–dove);}
.ldot{width:6px;height:6px;border-radius:50%;flex-shrink:0;}

/* DNA PAGE */
.dna-hero{display:grid;grid-template-columns:repeat(auto-fill,minmax(190px,1fr));gap:1px;background:rgba(140,100,40,.12);}
.dnaf{background:#ffffff;padding:20px 22px;cursor:pointer;transition:background .15s;border-left:3px solid;}
.dnaf:hover{background:#f0ebe3;}
.dnaf-name{font-family:‘Cormorant Garamond’,serif;font-size:17px;color:var(–cream);margin-bottom:3px;font-weight:600;}
.dnaf-ct{font-size:7.5px;letter-spacing:.18em;color:var(–dove);text-transform:uppercase;}
.dnaf-list{font-size:8.5px;color:var(–dove);margin-top:7px;line-height:1.65;}
.dna-panel{background:#f0ebe3;border:1px solid rgba(140,100,40,.2);padding:26px;margin-top:1px;display:none;}
.dna-panel.open{display:block;}

/* LAB PAGE */
.lab-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(330px,1fr));gap:1px;background:rgba(140,100,40,.12);}
.lcard{background:#ffffff;padding:20px 24px;}
.lcomb{display:flex;align-items:center;gap:7px;margin-bottom:9px;flex-wrap:wrap;}
.litem{font-family:‘Cormorant Garamond’,serif;font-size:16px;color:var(–cream);font-weight:600;}
.lplus{color:var(–gold-dim);font-size:10px;}
.lratio{background:rgba(201,168,76,.07);border:1px solid rgba(201,168,76,.2);color:var(–gold);font-size:7.5px;letter-spacing:.13em;padding:2px 7px;margin-left:auto;}
.ldesc{font-size:10px;color:var(–dove);line-height:1.55;letter-spacing:.04em;}

/* AI SUGGESTER */
.suggester{background:#ffffff;border:1px solid rgba(140,100,40,.2);padding:28px 32px;margin-bottom:1px;}
.sug-title{font-family:‘Cormorant Garamond’,serif;font-size:20px;color:var(–cream);margin-bottom:4px;}
.sug-sub{font-size:8.5px;letter-spacing:.16em;text-transform:uppercase;color:var(–dove);margin-bottom:22px;}
.sug-controls{display:flex;align-items:flex-end;gap:14px;flex-wrap:wrap;margin-bottom:18px;}
.sug-select{flex:1;min-width:220px;background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(–parchment);padding:10px 13px;font-family:‘Josefin Sans’,sans-serif;font-size:10px;letter-spacing:.08em;outline:none;}
.sug-select:focus{border-color:rgba(201,168,76,.4);}
.spray-wrap{display:flex;flex-direction:column;gap:5px;min-width:160px;}
.spray-label{font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(–gold-dim);}
.spray-row{display:flex;align-items:center;gap:9px;}
.spray-btn{width:26px;height:26px;background:none;border:1px solid rgba(201,168,76,.25);color:var(–gold);font-size:14px;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all .15s;flex-shrink:0;}
.spray-btn:hover{background:rgba(201,168,76,.1);border-color:var(–gold);}
.spray-count{font-family:‘Cormorant Garamond’,serif;font-size:22px;color:var(–gold);min-width:28px;text-align:center;}
.spray-dots{display:flex;gap:4px;align-items:center;}
.spray-dot{width:7px;height:7px;border-radius:50%;background:rgba(201,168,76,.15);border:1px solid rgba(201,168,76,.2);transition:all .15s;}
.spray-dot.active{background:var(–gold);}
.sug-btn{padding:10px 22px;background:transparent;border:1px solid var(–gold);color:var(–gold);font-family:‘Josefin Sans’,sans-serif;font-size:8.5px;letter-spacing:.2em;text-transform:uppercase;cursor:pointer;transition:all .2s;white-space:nowrap;}
.sug-btn:hover{background:rgba(201,168,76,.1);}
.sug-btn:disabled{opacity:.4;cursor:not-allowed;}

.sug-results{display:none;}
.sug-results.open{display:block;animation:fu .3s ease;}
.sug-chosen{display:flex;align-items:center;gap:10px;margin-bottom:20px;padding-bottom:18px;border-bottom:1px solid rgba(201,168,76,.08);}
.sug-chosen-name{font-family:‘Cormorant Garamond’,serif;font-size:18px;color:var(–gold);}
.sug-chosen-spray{font-size:8.5px;letter-spacing:.14em;text-transform:uppercase;color:var(–dove);}
.sug-arrow{color:rgba(201,168,76,.3);font-size:20px;}
.sug-cards{display:grid;grid-template-columns:repeat(auto-fill,minmax(290px,1fr));gap:1px;background:rgba(140,100,40,.12);}
.sug-card{background:#ffffff;padding:18px 22px;border-top:2px solid;}
.sug-card-title{font-size:7px;letter-spacing:.24em;text-transform:uppercase;margin-bottom:10px;}
.sug-combo-row{display:flex;align-items:center;gap:8px;margin-bottom:8px;flex-wrap:wrap;}
.sug-frag{font-family:‘Cormorant Garamond’,serif;font-size:15px;color:var(–cream);}
.sug-sprays{background:rgba(201,168,76,.1);border:1px solid rgba(201,168,76,.25);color:var(–gold);font-size:8px;letter-spacing:.12em;padding:2px 8px;white-space:nowrap;}
.sug-plus{color:var(–gold-dim);font-size:11px;}
.sug-note{font-size:10px;color:var(–dove);line-height:1.58;margin-top:6px;}
.sug-occasion{font-size:7.5px;letter-spacing:.15em;text-transform:uppercase;color:var(–gold-dim);margin-top:8px;}
.sug-loading{padding:32px 0;text-align:center;color:var(–dove);}
.wx-occ-btn{padding:5px 13px;background:transparent;border:1px solid rgba(201,168,76,.2);color:var(–dove);font-family:‘Josefin Sans’,sans-serif;font-size:8px;letter-spacing:.16em;text-transform:uppercase;cursor:pointer;transition:all .2s;}
.wx-occ-btn:hover{border-color:var(–gold);color:var(–gold-light);}
.wx-occ-btn.active{border-color:var(–gold);color:var(–gold);background:rgba(201,168,76,.07);}
.sug-loading em{display:block;font-family:‘Cormorant Garamond’,serif;font-style:italic;font-size:17px;color:rgba(201,168,76,.3);animation:pulse 1.4s ease-in-out infinite;}
@keyframes pulse{0%,100%{opacity:.3;}50%{opacity:.8;}}
.sug-err{padding:18px;background:rgba(176,90,66,.07);border:1px solid rgba(176,90,66,.2);color:var(–rose);font-size:10px;line-height:1.6;margin-top:12px;}
.weather-bar{display:flex;align-items:center;gap:18px;padding:10px 16px;background:#f0ebe3;border:1px solid rgba(140,100,40,.15);margin-bottom:16px;flex-wrap:wrap;}
.weather-icon{font-size:22px;line-height:1;}
.weather-info{flex:1;}
.weather-temp{font-family:‘Cormorant Garamond’,serif;font-size:20px;color:var(–gold);display:inline;}
.weather-desc{font-size:8.5px;letter-spacing:.14em;text-transform:uppercase;color:var(–dove);margin-left:8px;}
.weather-note{font-size:9px;color:var(–gold-dim);letter-spacing:.06em;margin-top:2px;}
.weather-loading{font-size:8.5px;color:var(–dove);letter-spacing:.14em;text-transform:uppercase;animation:pulse 1.4s ease-in-out infinite;}
.weather-badge{font-size:7px;letter-spacing:.16em;text-transform:uppercase;padding:2px 8px;border:1px solid;margin-top:6px;display:inline-block;}

/* ROTATION */
.ritem{background:#ffffff;padding:13px 20px;display:flex;align-items:center;gap:16px;cursor:pointer;transition:background .15s;border-bottom:1px solid rgba(201,168,76,.03);}
.ritem:hover{background:#f0ebe3;}
.rrank{font-family:‘Cormorant Garamond’,serif;font-size:19px;color:var(–gold-dim);width:28px;flex-shrink:0;}
.rname{font-family:‘Cormorant Garamond’,serif;font-size:16px;color:var(–cream);margin-bottom:2px;font-weight:600;}
.rmeta{font-size:8px;color:var(–dove);letter-spacing:.07em;}
.rdays{font-family:‘Cormorant Garamond’,serif;font-size:19px;display:block;}
.rdays.n{color:rgba(107,99,88,.4);}
.rdays.s{color:var(–rose);}
.rdays.w{color:var(–gold-dim);}
.rdays.f{color:var(–forest);}

.empty-st{padding:65px;text-align:center;color:var(–dove);font-size:9.5px;letter-spacing:.14em;text-transform:uppercase;}
.empty-st em{display:block;font-family:‘Cormorant Garamond’,serif;font-style:italic;font-size:19px;color:rgba(201,168,76,.18);margin-bottom:7px;letter-spacing:0;text-transform:none;}

.confirm-box{background:#ffffff;border:1px solid rgba(176,90,66,.4);padding:22px 25px;max-width:370px;width:90vw;}
.confirm-box h3{font-family:‘Cormorant Garamond’,serif;font-size:20px;color:var(–cream);margin-bottom:7px;}
.confirm-box p{font-size:10px;color:var(–dove);line-height:1.6;margin-bottom:16px;}

::-webkit-scrollbar{width:4px;height:4px;}
::-webkit-scrollbar-track{background:#f0ebe3;}
::-webkit-scrollbar-thumb{background:rgba(140,100,40,.17);}

/* QUICK LOG */
.quick-log{position:fixed;bottom:24px;right:24px;z-index:150;}
.ql-btn{width:56px;height:56px;border-radius:50%;background:var(–gold);border:none;color:#fff;font-size:22px;cursor:pointer;box-shadow:0 4px 16px rgba(140,100,40,.35);transition:all .2s;display:flex;align-items:center;justify-content:center;}
.ql-btn:hover{transform:scale(1.08);}
.ql-panel{position:fixed;bottom:90px;right:24px;background:#ffffff;border:1px solid rgba(140,100,40,.2);padding:18px;width:300px;z-index:150;box-shadow:0 8px 32px rgba(0,0,0,.12);display:none;}
.ql-panel.open{display:block;animation:fu .2s ease;}
.ql-search{width:100%;background:var(–ash);border:1px solid rgba(140,100,40,.2);color:var(–parchment);padding:9px 12px;font-family:‘Josefin Sans’,sans-serif;font-size:10px;outline:none;margin-bottom:8px;font-weight:500;}
.ql-list{max-height:220px;overflow-y:auto;}
.ql-item{padding:9px 12px;cursor:pointer;font-size:10px;color:var(–cream);border-bottom:1px solid rgba(140,100,40,.08);transition:background .1s;font-weight:500;}
.ql-item:hover{background:#f0ebe3;}
.ql-item-house{font-size:7.5px;color:var(–gold);letter-spacing:.14em;text-transform:uppercase;font-weight:600;}
/* INSIGHTS */
.ins-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(300px,1fr));gap:1px;background:rgba(140,100,40,.12);}
.ins-card{background:#ffffff;padding:24px 26px;}
.ins-card-title{font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(–gold);margin-bottom:14px;font-weight:700;}
.ins-big{font-family:‘Cormorant Garamond’,serif;font-size:42px;font-weight:600;color:var(–gold);line-height:1;}
.ins-sub{font-size:9px;color:var(–dove);letter-spacing:.06em;margin-top:3px;font-weight:500;}
.ins-list-item{display:flex;align-items:center;justify-content:space-between;padding:8px 0;border-bottom:1px solid rgba(140,100,40,.08);font-size:10px;color:var(–cream);font-weight:500;}
.ins-list-item:last-child{border-bottom:none;}
.ins-list-rank{font-family:‘Cormorant Garamond’,serif;font-size:18px;color:var(–gold-dim);width:24px;flex-shrink:0;font-weight:600;}
.ins-list-name{flex:1;padding:0 8px;}
.ins-list-meta{font-size:8.5px;color:var(–dove);font-weight:500;}
.redundancy-item{padding:10px 0;border-bottom:1px solid rgba(140,100,40,.08);}
.redundancy-insp{font-size:8px;letter-spacing:.14em;text-transform:uppercase;color:var(–gold);margin-bottom:5px;font-weight:700;}
.redundancy-bottles{font-size:10px;color:var(–cream);line-height:1.6;font-weight:500;}
.gap-pill{display:inline-block;padding:4px 12px;border:1px solid;font-size:8px;letter-spacing:.12em;text-transform:uppercase;margin:3px;font-weight:600;}
.alert-item{display:flex;align-items:center;gap:12px;padding:10px 0;border-bottom:1px solid rgba(140,100,40,.08);}
.alert-dot{width:8px;height:8px;border-radius:50%;flex-shrink:0;}
.alert-text{font-size:10px;color:var(–cream);font-weight:500;}
.alert-sub{font-size:8.5px;color:var(–dove);margin-top:2px;}
/* WISHLIST */
.wl-form{background:#f0ebe3;border:1px solid rgba(140,100,40,.2);padding:20px 24px;margin-bottom:1px;}
.wl-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:1px;background:rgba(140,100,40,.12);}
.wl-card{background:#ffffff;padding:18px 22px;position:relative;}
.wl-badge{font-size:7px;letter-spacing:.16em;text-transform:uppercase;padding:2px 8px;border:1px solid;font-weight:700;display:inline-block;margin-bottom:8px;}
.wl-name{font-family:‘Cormorant Garamond’,serif;font-size:16px;color:var(–cream);font-weight:600;margin-bottom:2px;}
.wl-house{font-size:8px;letter-spacing:.16em;text-transform:uppercase;color:var(–gold);font-weight:600;margin-bottom:5px;}
.wl-note{font-size:9.5px;color:var(–dove);line-height:1.5;}
.wl-del{position:absolute;top:10px;right:12px;background:none;border:none;color:var(–dove);cursor:pointer;font-size:14px;padding:3px;}
.wl-del:hover{color:var(–rose);}
.stock-btn{font-size:7px;letter-spacing:.12em;text-transform:uppercase;padding:3px 8px;border:1px solid;cursor:pointer;background:transparent;font-family:‘Josefin Sans’,sans-serif;font-weight:600;margin-left:6px;transition:all .15s;}
.stock-low{border-color:var(–rose)!important;color:var(–rose)!important;}
/* CUSTOM TAGS */
.ctag{display:inline-flex;align-items:center;gap:4px;padding:2px 8px;border:1px solid rgba(140,100,40,.3);background:rgba(140,100,40,.06);font-size:7.5px;letter-spacing:.12em;text-transform:uppercase;color:var(–gold);font-weight:600;margin:2px;}
.ctag-del{background:none;border:none;color:var(–dove);cursor:pointer;font-size:10px;padding:0 0 0 2px;line-height:1;}
.ctag-del:hover{color:var(–rose);}
.tag-input{background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(–parchment);padding:6px 10px;font-family:‘Josefin Sans’,sans-serif;font-size:10px;outline:none;width:140px;}
/* MORNING REC */
.morning-card{background:#ffffff;border:1px solid rgba(140,100,40,.25);border-left:4px solid var(–gold);padding:20px 24px;margin-bottom:16px;position:relative;}

.morning-pick{font-family:‘Cormorant Garamond’,serif;font-size:22px;color:var(–cream);font-weight:600;margin:4px 0 3px;}
.morning-house{font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(–gold);font-weight:700;}
.morning-reason{font-size:9.5px;color:var(–dove);line-height:1.5;margin-top:4px;}
/* SOTD CARD */
.sotd-card{background:#ffffff;border:2px solid rgba(140,100,40,.2);padding:20px;text-align:center;max-width:320px;margin:0 auto;}
.sotd-date{font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(–gold);font-weight:700;margin-bottom:8px;}
.sotd-name{font-family:‘Cormorant Garamond’,serif;font-size:22px;font-weight:600;color:var(–cream);margin-bottom:3px;}
.sotd-house{font-size:9px;color:var(–dove);letter-spacing:.1em;margin-bottom:10px;}
.sotd-meta{font-size:9px;color:var(–dove);line-height:1.8;}
/* COST PER WEAR */
.cpw-good{color:var(–forest);font-weight:700;}
.cpw-ok{color:var(–gold);font-weight:700;}
.cpw-bad{color:var(–rose);font-weight:700;}
/* STREAK */
.streak-num{font-family:‘Cormorant Garamond’,serif;font-size:52px;color:var(–gold);font-weight:600;line-height:1;}
.streak-fire{font-size:28px;}
/* BOTTLE PAGE */
#page-bottle .cpill{font-size:7px;padding:4px 8px;}
.bp-wear-entry{display:flex;align-items:center;justify-content:space-between;padding:6px 0;border-bottom:1px solid rgba(140,100,40,.08);font-size:10px;font-weight:500;}
.bp-wear-date{color:var(–cream);}
/* SEARCH */
#srch-grid .card{cursor:pointer;}
</style>

  <link rel="manifest" href="data:application/json,%7B%22name%22%3A%22The+Vault%22%2C%22short_name%22%3A%22Vault%22%2C%22start_url%22%3A%22.%2F%22%2C%22display%22%3A%22standalone%22%2C%22background_color%22%3A%22%23ede8de%22%2C%22theme_color%22%3A%22%238a5e1e%22%7D">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="default">
  <meta name="apple-mobile-web-app-title" content="The Vault">
  <meta name="theme-color" content="#8a5e1e">
</head>
<body>

<header class="header">
  <div>
    <div class="brand-name">The Vault</div>
    <div class="brand-sub">AJ's Collection · Est. 2022</div>
  </div>
  <div class="stats-strip">
    <div class="stat"><span class="stat-num" id="s-total">0</span><span class="stat-label">Bottles</span></div>
    <div class="sdiv"></div>
    <div class="stat"><span class="stat-num" id="s-houses">0</span><span class="stat-label">Houses</span></div>
    <div class="sdiv"></div>
    <div class="stat"><span class="stat-num" id="s-worn">0</span><span class="stat-label">Wears</span></div>
    <div class="sdiv"></div>
    <div class="stat"><span class="stat-num" id="s-starred">0</span><span class="stat-label">Starred</span></div>
  </div>
  <div style="display:flex;gap:8px;align-items:center;">
    <button class="add-btn" onclick="openAddModal()">+ Add Bottle</button>
    <button id="dark-toggle" onclick="toggleDarkMode()" style="width:36px;height:36px;border-radius:50%;border:1px solid var(--gold);background:transparent;color:var(--gold);cursor:pointer;font-size:16px;display:flex;align-items:center;justify-content:center;transition:all .2s;" title="Toggle dark mode">☀</button>
  </div>
</header>

<nav class="nav-bar">
  <button class="nav-tab active" onclick="showPage('collection',this)">Collection</button>
  <button class="nav-tab" onclick="showPage('classification',this)">DNA Classification</button>
  <button class="nav-tab" onclick="showPage('layering',this)">Layering Lab</button>
  <button class="nav-tab" onclick="showPage('analytics',this)">Analytics</button>
  <button class="nav-tab" onclick="showPage('rotation',this)">Rotation</button>
  <button class="nav-tab" onclick="showPage('starred',this)">Starred</button>
  <button class="nav-tab" onclick="showPage('weather',this)">&#9728; Weather</button>
  <button class="nav-tab" onclick="showPage('insights',this)">&#10024; Insights</button>
  <button class="nav-tab" onclick="showPage('wishlist',this)">&#9734; Wishlist</button>
  <button class="nav-tab" onclick="showPage('search',this)">&#128269; Search</button>
  <button class="nav-tab" onclick="showPage('importexport',this)">&#8645; Import / Export</button>
  <button class="nav-tab" onclick="showPage('duaadvisor',this)" style="color:var(--gold);font-weight:700;">✦ Dua Advisor</button>
</nav>

<main class="main">

<!-- COLLECTION -->

<div id="page-collection" class="page active">
  <div class="toolbar">
    <div class="sw"><span class="si">⌕</span><input type="text" id="search" placeholder="Search name, inspiration, house…" oninput="renderGrid()"></div>
    <select id="fh" onchange="renderGrid()"><option value="">All Houses</option></select>
    <select id="fs" onchange="renderGrid()"><option value="">All Seasons</option><option value="ss">Spring · Summer</option><option value="fw">Fall · Winter</option><option value="yr">Year-Round</option></select>
    <select id="fo" onchange="renderGrid()"><option value="">All Occasions</option><option value="date">Date / Romantic</option><option value="office">Office / Formal</option><option value="evening">Evening / Club</option><option value="casual">Casual</option><option value="sport">Sport / Outdoor</option><option value="special">Special Occasion</option></select>
    <select id="fd" onchange="renderGrid()">
      <option value="">All DNA Families</option>
      <option>Aquatic / Marine</option><option>Fougère</option><option>Woody / Aromatic</option>
      <option>Oriental / Amber</option><option>Oud / Resinous</option><option>Citrus / Fresh</option>
      <option>Gourmand</option><option>Floral</option><option>Chypre</option>
      <option>Tobacco / Smoky</option><option>Musky / Skin</option>
    </select>
    <select id="ftag" onchange="renderGrid()"><option value="">All Tags</option></select>
    <select id="fsort" onchange="renderGrid()">
      <option value="default">Sort: Default</option>
      <option value="name">Sort: Name A-Z</option>
      <option value="house">Sort: House</option>
      <option value="rating">Sort: Highest Rated</option>
      <option value="wears">Sort: Most Worn</option>
      <option value="recent">Sort: Recently Added</option>
      <option value="unworn">Sort: Never Worn First</option>
    </select>
  </div>
  <!-- MORNING RECOMMENDATION -->
  <div class="morning-card" id="morning-rec" style="display:none;">
    <div style="display:flex;align-items:flex-start;justify-content:space-between;flex-wrap:wrap;gap:12px;">
      <div style="flex:1;">
        <div style="font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);font-weight:700;margin-bottom:4px;">&#127774; Today&#39;s Recommendation</div>
        <div class="morning-house" id="mr-house"></div>
        <div class="morning-pick" id="mr-name"></div>
        <div class="morning-reason" id="mr-reason"></div>
        <div style="margin-top:10px;display:flex;gap:8px;flex-wrap:wrap;">
          <button class="btn btn-gold" style="font-size:8px;" onclick="logMorningWear()">&#10022; Wear This Today</button>
          <button class="btn btn-muted" style="font-size:8px;" onclick="refreshMorningRec()">&#8635; Different Pick</button>
        </div>
      </div>
      <div style="text-align:right;flex-shrink:0;">
        <div id="mr-sprays" style="font-family:'Cormorant Garamond',serif;font-size:32px;color:var(--gold);font-weight:600;line-height:1;"></div>
        <div style="font-size:8px;color:var(--dove);letter-spacing:.1em;">sprays</div>
        <div id="mr-weather-badge" style="margin-top:8px;"></div>
      </div>
    </div>
  </div>

  <div class="sec-hdr"><span class="sec-title">The Collection</span><span class="sec-ct" id="grid-count"></span></div>
  <div class="grid" id="grid"></div>
</div>

<!-- DNA CLASSIFICATION -->

<div id="page-classification" class="page">
  <div class="sec-hdr"><span class="sec-title">DNA Classification</span><span class="sec-ct">olfactory families</span></div>
  <div class="dna-hero" id="dna-families"></div>
  <div class="dna-panel" id="dna-panel"></div>
</div>

<!-- LAYERING LAB -->

<div id="page-layering" class="page">
  <div class="sec-hdr"><span class="sec-title">Layering Lab</span><span class="sec-ct" id="lab-ct"></span></div>

  <!-- AI SUGGESTER -->

  <div class="suggester">
    <div class="sug-title">Smart Layering Suggestions</div>
    <div class="sug-sub">Choose a fragrance &middot; set your spray count &middot; get AI pairings from your collection</div>
    <div class="weather-bar" id="weather-bar"><span class="weather-loading" id="weather-loading">Fetching Arlington, VA weather…</span></div>
    <div class="sug-controls">
      <select class="sug-select" id="sug-frag">
        <option value="">Select a fragrance to layer&hellip;</option>
      </select>
      <div class="spray-wrap">
        <div class="spray-label">Your Spray Count</div>
        <div class="spray-row">
          <button class="spray-btn" onclick="changeSpray(-1)">&#8722;</button>
          <span class="spray-count" id="spray-num">2</span>
          <div class="spray-dots" id="spray-dots"></div>
          <button class="spray-btn" onclick="changeSpray(1)">+</button>
        </div>
      </div>
      <div class="spray-wrap">
        <div class="spray-label">Occasion</div>
        <select id="sug-occ" style="background:var(--ash);border:1px solid var(--ab);color:var(--parchment);padding:8px 11px;font-family:'Josefin Sans',sans-serif;font-size:9px;letter-spacing:.1em;outline:none;margin-top:2px;">
          <option value="">Any Occasion</option>
          <option value="date">♥ Date Night</option>
          <option value="office">◆ Office / Day</option>
          <option value="evening">✦ Evening / Club</option>
          <option value="casual">■ Casual</option>
          <option value="sport">▲ Sport / Active</option>
          <option value="special">★ Special Occasion</option>
        </select>
      </div>
      <button class="sug-btn" id="sug-go-btn" onclick="runSuggester()">Suggest Pairings &#10022;</button>
    </div>
    <div id="sug-results" class="sug-results"></div>
  </div>

  <!-- SAVED COMBOS -->

  <div style="display:flex;align-items:center;justify-content:space-between;margin:22px 0 14px;">
    <div class="sec-title" style="font-size:17px;">Saved Combos</div>
    <button class="btn btn-gold" onclick="toggleGLForm()">+ Add Manually</button>
  </div>
  <div class="alf hidden" id="gl-form" style="margin-bottom:1px;">
    <div class="fl" style="margin-bottom:6px;">New Layering Combo</div>
    <input type="text" id="gl-items" placeholder="Fragrance names, comma separated">
    <input type="text" id="gl-ratio" placeholder="Ratio / spray count (e.g. 2+2, Oil + 3 sprays)">
    <textarea id="gl-desc" placeholder="Notes on this combo..."></textarea>
    <div style="display:flex;gap:8px;"><button class="btn btn-gold" onclick="saveGlobalLayer()">Save</button><button class="btn btn-muted" onclick="toggleGLForm()">Cancel</button></div>
  </div>
  <div class="lab-grid" id="lab-grid"></div>
</div>

<!-- ANALYTICS -->

<div id="page-analytics" class="page">
  <div class="sec-hdr"><span class="sec-title">Analytics</span></div>
  <div class="agrid">
    <div class="acard"><div class="atitle">Bottles by House</div><div id="ch-houses"></div></div>
    <div class="acard"><div class="atitle">Season Split</div><div class="dw"><svg style="width:88px;height:88px;flex-shrink:0;" viewBox="0 0 36 36" id="donut-s"></svg><div id="legend-s"></div></div></div>
    <div class="acard"><div class="atitle">Occasion Breakdown</div><div id="ch-occ"></div></div>
    <div class="acard"><div class="atitle">DNA Family Distribution</div><div id="ch-dna"></div></div>
    <div class="acard"><div class="atitle">Overview</div><div class="bignum" id="a-total">0</div><div class="biglbl">Total Bottles</div><div style="margin-top:12px;font-size:9.5px;color:var(--dove);line-height:1.85;letter-spacing:.04em;" id="a-overview"></div></div>
    <div class="acard"><div class="atitle">Top Inspirations</div><div id="ch-insp"></div></div>
  </div>
</div>

<!-- ROTATION -->

<div id="page-rotation" class="page">
  <div class="sec-hdr"><span class="sec-title">Rotation Tracker</span><span class="sec-ct">sorted by days since last wear</span></div>
  <div id="rot-list"></div>
</div>

<!-- STARRED -->

<div id="page-starred" class="page">
  <div class="sec-hdr"><span class="sec-title">Starred</span><span class="sec-ct" id="starred-ct"></span></div>
  <div class="grid" id="starred-grid"></div>
</div>

<!-- WEATHER -->

<div id="page-weather" class="page">
  <div class="sec-hdr"><span class="sec-title">Weather & Your Vault</span><span class="sec-ct" id="wx-location">Arlington, VA</span></div>

  <!-- Current conditions card -->

  <div id="wx-main-card" style="background:#ffffff;border:1px solid rgba(140,100,40,.2);padding:28px 32px;margin-bottom:1px;">
    <div id="wx-loading" style="font-size:9px;letter-spacing:.18em;text-transform:uppercase;color:var(--dove);animation:pulse 1.4s ease-in-out infinite;">Fetching current conditions…</div>
    <div id="wx-content" style="display:none;">
      <div style="display:flex;align-items:center;gap:22px;flex-wrap:wrap;margin-bottom:22px;">
        <div id="wx-icon-big" style="font-size:52px;line-height:1;"></div>
        <div>
          <div style="display:flex;align-items:baseline;gap:12px;">
            <span id="wx-temp-big" style="font-family:'Cormorant Garamond',serif;font-size:56px;font-weight:300;color:var(--gold);line-height:1;"></span>
            <span id="wx-desc-big" style="font-size:11px;letter-spacing:.18em;text-transform:uppercase;color:var(--dove);"></span>
          </div>
          <div id="wx-meta" style="font-size:9.5px;color:var(--dove);margin-top:6px;letter-spacing:.06em;"></div>
        </div>
        <div id="wx-badge-wrap" style="margin-left:auto;"></div>
      </div>
      <div id="wx-scent-tip" style="background:rgba(201,168,76,.05);border:1px solid rgba(201,168,76,.1);padding:14px 18px;font-size:10.5px;color:var(--cream);line-height:1.65;letter-spacing:.04em;margin-bottom:22px;"></div>

```
  <!-- Spray guide -->
  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:1px;background:rgba(201,168,76,.05);margin-bottom:1px;">
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold-dim);margin-bottom:8px;">Recommended Sprays</div>
      <div id="wx-sprays" style="font-family:'Cormorant Garamond',serif;font-size:32px;color:var(--gold);"></div>
      <div id="wx-spray-note" style="font-size:9px;color:var(--dove);margin-top:4px;"></div>
    </div>
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold-dim);margin-bottom:8px;">Best DNA Families Today</div>
      <div id="wx-dna-best" style="font-size:10px;color:var(--cream);line-height:1.8;"></div>
    </div>
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold-dim);margin-bottom:8px;">Avoid Today</div>
      <div id="wx-dna-avoid" style="font-size:10px;color:var(--dove);line-height:1.8;"></div>
    </div>
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold-dim);margin-bottom:8px;">Conditions</div>
      <div id="wx-feels" style="font-size:10px;color:var(--cream);line-height:1.8;"></div>
    </div>
  </div>
</div>
```

  </div>

  <!-- Today's picks from your vault -->

  <div style="display:flex;align-items:center;justify-content:space-between;margin:20px 0 14px;">
    <div class="sec-title" style="font-size:18px;">Today's Picks From Your Vault</div>
    <span id="wx-picks-meta" style="font-size:8.5px;letter-spacing:.14em;text-transform:uppercase;color:var(--dove);"></span>
  </div>
  <div class="grid" id="wx-picks-grid"></div>

  <!-- Occasion picks -->

  <div style="margin:22px 0 14px;display:flex;align-items:center;gap:14px;flex-wrap:wrap;">
    <div class="sec-title" style="font-size:18px;">By Occasion</div>
    <div style="display:flex;gap:7px;flex-wrap:wrap;" id="wx-occ-tabs">
      <button class="wx-occ-btn active" onclick="showWxOcc('date',this)">♥ Date</button>
      <button class="wx-occ-btn" onclick="showWxOcc('office',this)">◆ Office</button>
      <button class="wx-occ-btn" onclick="showWxOcc('evening',this)">✦ Evening</button>
      <button class="wx-occ-btn" onclick="showWxOcc('casual',this)">■ Casual</button>
      <button class="wx-occ-btn" onclick="showWxOcc('sport',this)">▲ Sport</button>
      <button class="wx-occ-btn" onclick="showWxOcc('special',this)">★ Special</button>
    </div>
  </div>
  <div class="grid" id="wx-occ-grid"></div>
</div>

<!-- INSIGHTS PAGE -->

<div id="page-insights" class="page">
  <div class="sec-hdr"><span class="sec-title">&#10024; Insights</span><span class="sec-ct">your collection at a glance</span></div>

  <!-- ROTATION REMINDERS BANNER -->

  <div id="reminder-banner" style="display:none;background:#ffffff;border:1px solid rgba(140,100,40,.2);border-left:4px solid var(--gold);padding:16px 20px;margin-bottom:1px;">
    <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:8px;font-weight:700;">&#128276; Rotation Reminders</div>
    <div id="reminder-list"></div>
    <div style="margin-top:10px;display:flex;gap:8px;flex-wrap:wrap;">
      <button class="btn btn-gold" style="font-size:7.5px;" onclick="requestNotificationPermission()">&#128276; Enable Push Reminders</button>
      <button class="btn btn-muted" style="font-size:7.5px;" id="notif-status"></button>
    </div>
  </div>
  <div class="ins-grid" id="ins-grid"></div>
</div>

<!-- WISHLIST PAGE -->

<div id="page-wishlist" class="page">
  <div class="sec-hdr"><span class="sec-title">&#9734; Wishlist &amp; Destash</span></div>
  <div class="wl-form" id="wl-form">
    <div style="display:flex;gap:12px;flex-wrap:wrap;margin-bottom:10px;">
      <input type="text" id="wl-name" placeholder="Fragrance name" style="flex:1;min-width:160px;background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(--parchment);padding:9px 12px;font-family:'Josefin Sans',sans-serif;font-size:10px;outline:none;font-weight:500;">
      <input type="text" id="wl-house" placeholder="House / Brand" style="flex:1;min-width:140px;background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(--parchment);padding:9px 12px;font-family:'Josefin Sans',sans-serif;font-size:10px;outline:none;font-weight:500;">
      <select id="wl-type" style="background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(--parchment);padding:9px 12px;font-family:'Josefin Sans',sans-serif;font-size:9px;outline:none;font-weight:600;">
        <option value="want">&#9734; Want to Buy</option>
        <option value="destash">&#10060; Destash</option>
        <option value="decant">&#x1F4E6; Want a Decant</option>
        <option value="low">&#9888; Running Low</option>
      </select>
    </div>
    <input type="text" id="wl-note" placeholder="Notes (price, where to buy, why destashing...)" style="width:100%;background:#ffffff;border:1px solid rgba(140,100,40,.2);color:var(--parchment);padding:9px 12px;font-family:'Josefin Sans',sans-serif;font-size:10px;outline:none;margin-bottom:10px;font-weight:400;">
    <button class="btn btn-gold" onclick="addWishlistItem()">Add Item</button>
  </div>
  <div class="wl-grid" id="wl-grid"></div>
</div>

<!-- BOTTLE PROFILE PAGE -->

<div id="page-bottle" class="page">
  <div style="display:flex;align-items:center;gap:14px;margin-bottom:22px;flex-wrap:wrap;">
    <button class="btn btn-muted" onclick="closeBottlePage()" style="font-size:8px;">&#8592; Back</button>
    <div id="bp-breadcrumb" style="font-size:8.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--dove);font-weight:500;"></div>
  </div>

  <!-- Header -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.15);padding:28px 32px;margin-bottom:1px;position:relative;">
    <div id="bp-house" style="font-size:8px;letter-spacing:.28em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;"></div>
    <div id="bp-name" style="font-family:'Cormorant Garamond',serif;font-size:34px;font-weight:600;color:var(--cream);line-height:1.1;margin-bottom:5px;"></div>
    <div id="bp-insp" style="font-family:'Cormorant Garamond',serif;font-style:italic;font-size:15px;color:var(--dove);margin-bottom:14px;"></div>
    <div style="display:flex;gap:8px;flex-wrap:wrap;" id="bp-tags"></div>
    <div style="position:absolute;top:20px;right:24px;display:flex;gap:8px;align-items:center;">
      <button class="btn btn-muted" id="bp-star-btn" onclick="toggleStar()" style="font-size:8px;"></button>
      <button class="btn btn-muted" id="bp-stock-btn" onclick="cycleStock()" style="font-size:7.5px;"></button>
    </div>
  </div>

  <!-- Stats row -->

  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:1px;background:rgba(140,100,40,.1);margin-bottom:1px;">
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Total Wears</div>
      <div id="bp-wears" style="font-family:'Cormorant Garamond',serif;font-size:36px;color:var(--gold);font-weight:600;line-height:1;"></div>
    </div>
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Last Worn</div>
      <div id="bp-lastworn" style="font-family:'Cormorant Garamond',serif;font-size:16px;color:var(--cream);font-weight:600;line-height:1.3;"></div>
    </div>
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Your Rating</div>
      <div id="bp-stars" style="font-size:18px;"></div>
    </div>
    <div style="background:#ffffff;padding:16px 18px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">DNA Family</div>
      <div id="bp-dna-label" style="font-size:11px;font-weight:600;color:var(--cream);"></div>
    </div>
  </div>

  <div style="display:grid;grid-template-columns:1fr 1fr;gap:1px;background:rgba(140,100,40,.1);margin-bottom:1px;">

```
<!-- DNA Classification -->
<div style="background:#ffffff;padding:20px 22px;">
  <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:12px;font-weight:700;">DNA Classification</div>
  <div class="class-grid" id="bp-dna-grid" style="grid-template-columns:1fr 1fr;"></div>
</div>
```

  </div>

  <!-- Custom Tags + Photo + Cost Per Wear -->

  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:1px;background:rgba(140,100,40,.1);margin-bottom:1px;">
    <div style="background:#ffffff;padding:20px 22px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:10px;font-weight:700;">Custom Tags</div>
      <div id="bp-custom-tags" style="margin-bottom:10px;display:flex;flex-wrap:wrap;gap:2px;"></div>
      <div style="display:flex;gap:6px;">
        <input class="tag-input" type="text" id="bp-tag-input" placeholder="Add tag (e.g. signature, travel)" onkeydown="if(event.key==='Enter')addCustomTag()">
        <button class="btn btn-muted" style="font-size:8px;padding:5px 10px;" onclick="addCustomTag()">+</button>
      </div>
    </div>
    <div style="background:#ffffff;padding:20px 22px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:10px;font-weight:700;">Photo</div>
      <div id="bp-photo-preview" style="margin-bottom:10px;"></div>
      <label class="btn btn-muted" style="cursor:pointer;font-size:8px;">
        &#128247; Add Photo
        <input type="file" accept="image/*" onchange="addBottlePhoto(this)" style="display:none;">
      </label>
      <button class="btn btn-danger" style="font-size:7.5px;margin-top:6px;" onclick="removeBottlePhoto()" id="bp-photo-del" style="display:none;">Remove</button>
    </div>
    <div style="background:#ffffff;padding:20px 22px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:10px;font-weight:700;">Cost Per Wear</div>
      <div style="margin-bottom:10px;">
        <div style="font-size:8.5px;color:var(--dove);margin-bottom:5px;font-weight:500;">Estimated value ($)</div>
        <input type="number" id="bp-value" placeholder="e.g. 45" min="0" onchange="saveBottleValue()" style="width:100%;background:var(--ash);border:1px solid rgba(140,100,40,.2);color:var(--parchment);padding:7px 10px;font-family:'Josefin Sans',sans-serif;font-size:11px;outline:none;">
      </div>
      <div id="bp-cpw" style="font-size:11px;font-weight:600;"></div>
    </div>
  </div>

  <!-- Shareable SOTD Card -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);padding:20px 22px;margin-bottom:1px;">
    <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:12px;font-weight:700;">&#128248; Scent of the Day Card</div>
    <div id="sotd-preview"></div>
    <button class="btn btn-muted" style="margin-top:12px;font-size:8px;" onclick="generateSOTD()">Generate SOTD Card</button>
    <div style="font-size:8.5px;color:var(--dove);margin-top:6px;">Screenshot and share with friends</div>
  </div>

  <div style="display:grid;grid-template-columns:1fr 1fr;gap:1px;background:rgba(140,100,40,.1);margin-bottom:1px;">
    <!-- DNA Classification (already above) --><div style="display:none;"></div>

```
<!-- Notes -->
<div style="background:#ffffff;padding:20px 22px;">
  <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:8px;font-weight:700;">Personal Notes</div>
  <textarea class="notes" id="bp-notes" placeholder="Observations, longevity, sillage, pairings…" onchange="saveNotes()" style="min-height:100px;"></textarea>
</div>
```

  </div>

  <!-- Wear calendar -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);padding:20px 22px;margin-bottom:1px;">
    <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:14px;font-weight:700;">Wear History</div>
    <div style="display:flex;gap:24px;flex-wrap:wrap;align-items:flex-start;">
      <div id="bp-calendar" style="flex:1;min-width:200px;"></div>
      <div id="bp-wear-log" style="flex:1;min-width:180px;max-height:200px;overflow-y:auto;"></div>
    </div>
    <button class="btn btn-gold" onclick="logWear()" style="margin-top:14px;">&#10022; Log Wear Today</button>
  </div>

  <!-- Layering -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);padding:20px 22px;margin-bottom:1px;">
    <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:12px;">
      <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);font-weight:700;">Layering Combos</div>
      <button class="btn btn-muted" style="font-size:7.5px;padding:4px 11px;" onclick="toggleLayerForm()">+ Add Combo</button>
    </div>
    <div id="bp-layer-list"></div>
    <div class="alf hidden" id="m-layer-form">
      <input type="text" id="lf-items" placeholder="Other fragrances to combine with (comma separated)">
      <input type="text" id="lf-ratio" placeholder="Ratio (e.g. 2+2, Oil base + spray)">
      <textarea id="lf-desc" placeholder="Notes on this combo…"></textarea>
      <div style="display:flex;gap:8px;"><button class="btn btn-gold" onclick="saveBottleLayer()">Save</button><button class="btn btn-muted" onclick="document.getElementById('m-layer-form').classList.add('hidden')">Cancel</button></div>
    </div>
  </div>

  <!-- Analytics for this bottle -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);padding:20px 22px;margin-bottom:1px;">
    <div style="font-size:7.5px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:14px;font-weight:700;">Similar in Your Collection</div>
    <div class="grid" id="bp-similar" style="grid-template-columns:repeat(auto-fill,minmax(220px,1fr));"></div>
  </div>

  <!-- Actions -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);padding:16px 22px;display:flex;gap:10px;flex-wrap:wrap;">
    <button class="btn btn-danger" onclick="deleteCurrentBottle()">&#10005; Remove from Vault</button>
    <button class="btn btn-muted" onclick="closeBottlePage()">&#8592; Back to Collection</button>
  </div>
</div>

<!-- SEARCH PAGE -->

<div id="page-search" class="page">
  <div class="sec-hdr"><span class="sec-title">&#128269; Search</span></div>
  <div style="position:relative;margin-bottom:20px;">
    <span class="si" style="position:absolute;left:14px;top:50%;transform:translateY(-50%);font-size:18px;color:var(--gold);">&#128269;</span>
    <input type="text" id="srch-input" placeholder="Search by name, house, inspiration, DNA, occasion…"
      oninput="runSearch(this.value)"
      style="width:100%;background:#ffffff;border:1px solid rgba(140,100,40,.25);color:var(--parchment);padding:14px 16px 14px 44px;font-family:'Josefin Sans',sans-serif;font-size:12px;outline:none;font-weight:500;letter-spacing:.04em;">
  </div>
  <div id="srch-meta" style="font-size:8.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--dove);margin-bottom:14px;font-weight:500;"></div>
  <div class="grid" id="srch-grid"></div>
</div>

<!-- IMPORT / EXPORT PAGE -->

<div id="page-importexport" class="page">
  <div class="sec-hdr"><span class="sec-title">&#8645; Import / Export</span><span class="sec-ct">share your vault with friends</span></div>

  <!-- HOW IT WORKS -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.15);padding:24px 28px;margin-bottom:1px;">
    <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:12px;font-weight:700;">How to Share With a Friend</div>
    <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:16px;">
      <div style="display:flex;gap:12px;align-items:flex-start;">
        <div style="font-family:'Cormorant Garamond',serif;font-size:28px;color:var(--gold);font-weight:600;line-height:1;flex-shrink:0;">1</div>
        <div><div style="font-size:10px;color:var(--cream);font-weight:600;margin-bottom:3px;">Download the template</div><div style="font-size:9px;color:var(--dove);">A CSV file with the correct columns pre-filled</div></div>
      </div>
      <div style="display:flex;gap:12px;align-items:flex-start;">
        <div style="font-family:'Cormorant Garamond',serif;font-size:28px;color:var(--gold);font-weight:600;line-height:1;flex-shrink:0;">2</div>
        <div><div style="font-size:10px;color:var(--cream);font-weight:600;margin-bottom:3px;">Fill it in Excel or Google Sheets</div><div style="font-size:9px;color:var(--dove);">Add their bottles — one per row</div></div>
      </div>
      <div style="display:flex;gap:12px;align-items:flex-start;">
        <div style="font-family:'Cormorant Garamond',serif;font-size:28px;color:var(--gold);font-weight:600;line-height:1;flex-shrink:0;">3</div>
        <div><div style="font-size:10px;color:var(--cream);font-weight:600;margin-bottom:3px;">Import the CSV here</div><div style="font-size:9px;color:var(--dove);">Their collection loads instantly</div></div>
      </div>
    </div>
  </div>

  <!-- EXPORT YOUR COLLECTION -->

  <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:1px;background:rgba(140,100,40,.12);margin-bottom:1px;">

```
<div style="background:#ffffff;padding:24px 26px;">
  <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">&#11015; Export Your Collection</div>
  <div style="font-size:9.5px;color:var(--dove);margin-bottom:14px;line-height:1.6;">Download your bottles as a CSV file. Open in Excel or Google Sheets, share with friends, or use as a backup.</div>
  <button class="btn btn-gold" onclick="exportCSV()" style="margin-bottom:8px;width:100%;justify-content:center;">Download Collection CSV</button>
  <button class="btn btn-muted" onclick="downloadTemplate()" style="width:100%;justify-content:center;">Download Blank Template</button>
</div>

<div style="background:#ffffff;padding:24px 26px;">
  <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">&#11014; Import a Collection</div>
  <div style="font-size:9.5px;color:var(--dove);margin-bottom:14px;line-height:1.6;">Load a CSV file to replace or merge with your current collection. Use the template above so the columns match.</div>
  <div style="margin-bottom:10px;">
    <label style="display:flex;align-items:center;gap:8px;font-size:9px;color:var(--cream);font-weight:500;margin-bottom:8px;">
      <input type="radio" name="import-mode" value="replace" checked id="ir-replace"> Replace my entire collection
    </label>
    <label style="display:flex;align-items:center;gap:8px;font-size:9px;color:var(--cream);font-weight:500;">
      <input type="radio" name="import-mode" value="merge" id="ir-merge"> Merge (add new bottles only)
    </label>
  </div>
  <label class="btn btn-gold" style="width:100%;justify-content:center;cursor:pointer;display:flex;">
    Choose CSV File
    <input type="file" accept=".csv" onchange="importCSV(this)" style="display:none;">
  </label>
  <div id="import-status" style="margin-top:10px;font-size:9.5px;color:var(--dove);"></div>
</div>

<div style="background:#ffffff;padding:24px 26px;">
  <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">&#128190; Full Backup / Restore</div>
  <div style="font-size:9.5px;color:var(--dove);margin-bottom:14px;line-height:1.6;">Backup includes everything — wears, ratings, notes, layering combos, wishlist. Use to transfer between devices.</div>
  <button class="btn btn-gold" onclick="exportBackup()" style="margin-bottom:8px;width:100%;justify-content:center;">Download Full Backup</button>
  <label class="btn btn-muted" style="width:100%;justify-content:center;cursor:pointer;display:flex;">
    Restore from Backup
    <input type="file" accept=".json" onchange="importBackup(this)" style="display:none;">
  </label>
</div>
```

  </div>

  <!-- CSV FORMAT GUIDE -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);padding:24px 26px;margin-bottom:1px;">
    <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:12px;font-weight:700;">CSV Column Guide</div>
    <div style="overflow-x:auto;">
      <table style="width:100%;border-collapse:collapse;font-size:9.5px;">
        <thead>
          <tr style="border-bottom:2px solid rgba(140,100,40,.2);">
            <th style="text-align:left;padding:8px 12px;font-size:7.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--gold);font-weight:700;">Column</th>
            <th style="text-align:left;padding:8px 12px;font-size:7.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--gold);font-weight:700;">Required</th>
            <th style="text-align:left;padding:8px 12px;font-size:7.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--gold);font-weight:700;">Example</th>
            <th style="text-align:left;padding:8px 12px;font-size:7.5px;letter-spacing:.16em;text-transform:uppercase;color:var(--gold);font-weight:700;">Notes</th>
          </tr>
        </thead>
        <tbody id="csv-guide-body"></tbody>
      </table>
    </div>
  </div>

  <!-- PREVIEW -->

  <div id="import-preview" style="display:none;background:#ffffff;border:1px solid rgba(140,100,40,.15);padding:24px 26px;">
    <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:12px;font-weight:700;">Import Preview</div>
    <div id="import-preview-content"></div>
    <div style="display:flex;gap:10px;margin-top:16px;">
      <button class="btn btn-gold" id="import-confirm-btn">Confirm Import</button>
      <button class="btn btn-muted" onclick="cancelImport()">Cancel</button>
    </div>
  </div>
</div>

<!-- DUA ADVISOR PAGE -->

<div id="page-duaadvisor" class="page">
  <div class="sec-hdr">
    <span class="sec-title">✦ Dua Brand Advisor</span>
    <span class="sec-ct">AI-powered buy or skip analysis</span>
  </div>

  <!-- Input Section -->

  <div style="background:#ffffff;border:1px solid rgba(140,100,40,.2);border-left:4px solid var(--gold);padding:24px 26px;margin-bottom:1px;">
    <div style="font-size:8px;letter-spacing:.22em;text-transform:uppercase;color:var(--gold);margin-bottom:10px;font-weight:700;">Enter a Dua Fragrance Name</div>
    <div style="font-size:9.5px;color:var(--dove);margin-bottom:16px;line-height:1.6;">Type any Dua Brand fragrance — I'll research it, check it against your existing 164 bottles for redundancy, and give you a clear buy or skip verdict.</div>
    <div style="display:flex;gap:10px;flex-wrap:wrap;align-items:flex-start;">
      <div style="flex:1;min-width:200px;">
        <input type="text" id="dua-input" placeholder="e.g. Bleu de Dua Extrait, Fortune, Ottoman Breeze…"
          style="width:100%;background:#f0ebe3;border:1px solid rgba(140,100,40,.25);color:var(--parchment);padding:12px 14px;font-family:'Josefin Sans',sans-serif;font-size:11px;outline:none;font-weight:500;border-radius:0;"
          onkeydown="if(event.key==='Enter')runDuaAdvisor()">
        <div style="font-size:8.5px;color:var(--dove);margin-top:6px;">Include the full name if you know it. Be as specific as possible.</div>
      </div>
      <button class="btn btn-gold" id="dua-go-btn" onclick="runDuaAdvisor()" style="padding:12px 22px;font-size:9px;white-space:nowrap;">
        ✦ Analyze
      </button>
    </div>
  </div>

  <!-- Results Section -->

  <div id="dua-results" style="display:none;margin-top:1px;"></div>
</div>

</main>

<!-- QUICK LOG BUTTON -->

<div class="quick-log">
  <div class="ql-panel" id="ql-panel">
    <div style="font-size:8px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:10px;font-weight:700;">&#9998; Log Today's Wear</div>
    <input class="ql-search" type="text" placeholder="Search fragrance..." oninput="filterQL(this.value)" id="ql-search">
    <div class="ql-list" id="ql-list"></div>
  </div>
  <button class="ql-btn" onclick="toggleQL()" title="Quick log wear">&#9998;</button>
</div>

<!-- DETAIL MODAL -->

<div class="overlay hidden" id="det-overlay" onclick="closeDetModal(event)">
<div class="modal">
  <div class="mh">
    <div class="m-house" id="m-house"></div>
    <div class="m-name" id="m-name"></div>
    <div class="m-insp" id="m-insp"></div>
    <button class="mcl" onclick="closeDetDirect()">✕</button>
  </div>
  <div class="mb">
    <div class="row">
      <div class="field"><div class="fl">Occasion</div><div class="fv" id="m-occ"></div></div>
      <div class="field"><div class="fl">Season</div><div class="fv" id="m-sea"></div></div>
      <div class="field"><div class="fl">Wears</div><div class="fv" style="font-family:'Cormorant Garamond',serif;font-size:22px;color:var(--gold);" id="m-wears"></div></div>
    </div>

```
<div class="fl" style="margin-bottom:8px;">DNA Classification — Select Family</div>
<div class="class-grid" id="m-dna-grid"></div>

<div class="mdiv"></div>
<div class="fl" style="margin-bottom:7px;">Your Rating</div>
<div class="stars" id="m-stars"></div>

<div class="mdiv"></div>
<div class="fl" style="margin-bottom:7px;">Personal Notes</div>
<textarea class="notes" id="m-notes" placeholder="Observations, longevity, sillage notes, pairings…" onchange="saveNotes()"></textarea>

<div class="mdiv"></div>
<div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:9px;">
  <div class="fl" style="margin-bottom:0;">Layering Combos</div>
  <button class="btn btn-muted" style="font-size:7.5px;padding:4px 11px;" onclick="toggleLayerForm()">+ Add Combo</button>
</div>
<div id="m-layer-list"></div>
<div class="alf hidden" id="m-layer-form">
  <input type="text" id="lf-items" placeholder="Other fragrances to combine with (comma separated)">
  <input type="text" id="lf-ratio" placeholder="Ratio or type (e.g. 2+2, Oil base + spray)">
  <textarea id="lf-desc" placeholder="Notes on this combo — development, when to wear, tips…"></textarea>
  <div style="display:flex;gap:8px;"><button class="btn btn-gold" onclick="saveBottleLayer()">Save</button><button class="btn btn-muted" onclick="document.getElementById('m-layer-form').classList.add('hidden')">Cancel</button></div>
</div>

<div class="mdiv"></div>
<div class="fl" style="margin-bottom:7px;">Wear Log</div>
<div id="m-wear-log"></div>

<div class="btn-row">
  <button class="btn btn-gold" onclick="logWear()">✦ Log Wear</button>
  <button class="btn btn-muted" id="m-star-btn" onclick="toggleStar()">☆ Star</button>
  <button class="btn btn-danger" onclick="deleteCurrentBottle()">✕ Remove</button>
  <button class="btn btn-muted" id="m-stock-btn" onclick="cycleStock()" style="font-size:7.5px;">&#9646; Stock OK</button>
</div>
```

  </div>
</div>
</div>

<!-- ADD BOTTLE MODAL -->

<div class="overlay hidden" id="add-overlay" onclick="closeAddOverlay(event)">
<div class="add-modal">
  <div class="mh">
    <div class="m-house" style="margin-bottom:4px;">New Bottle</div>
    <div class="m-name">Add to Collection</div>
    <button class="mcl" onclick="document.getElementById('add-overlay').classList.add('hidden')">✕</button>
  </div>
  <div class="mb">
    <div class="form-row">
      <div><label class="flabel">House / Brand *</label><input type="text" id="af-house" placeholder="e.g. The Dua Brand" list="house-dl"><datalist id="house-dl"></datalist></div>
      <div><label class="flabel">Fragrance Name *</label><input type="text" id="af-name" placeholder="Full name"></div>
    </div>
    <label class="flabel">Inspiration / DNA Reference</label>
    <input type="text" id="af-insp" placeholder="e.g. Creed Aventus, Bleu de Chanel, Original">
    <div class="form-row">
      <div><label class="flabel">Occasion</label>
        <select id="af-occ"><option value="date">♥ Date / Romantic</option><option value="office">◆ Office / Formal</option><option value="evening">✦ Evening / Club</option><option value="casual" selected>■ Casual</option><option value="sport">▲ Sport</option><option value="special">★ Special</option></select>
      </div>
      <div><label class="flabel">Season</label>
        <select id="af-sea"><option value="ss">Spring · Summer</option><option value="fw">Fall · Winter</option><option value="yr">Year-Round</option></select>
      </div>
    </div>
    <div class="form-row">
      <div><label class="flabel">DNA Family</label>
        <select id="af-dna"><option value="">Unclassified</option><option>Aquatic / Marine</option><option>Fougère</option><option>Woody / Aromatic</option><option>Oriental / Amber</option><option>Oud / Resinous</option><option>Citrus / Fresh</option><option>Gourmand</option><option>Floral</option><option>Chypre</option><option>Tobacco / Smoky</option><option>Musky / Skin</option></select>
      </div>
      <div style="display:flex;align-items:flex-end;padding-bottom:9px;">
        <label style="display:flex;align-items:center;gap:7px;cursor:pointer;font-size:8px;letter-spacing:.16em;text-transform:uppercase;color:var(--dove);">
          <input type="checkbox" id="af-base" style="width:auto;margin-bottom:0;"> Layering Base
        </label>
      </div>
    </div>
    <label class="flabel">Occasion Detail (optional)</label>
    <input type="text" id="af-occ-detail" placeholder="e.g. Office / smart casual / date night">
    <div class="btn-row" style="margin-top:5px;"><button class="btn btn-gold" onclick="addBottle()">Add to Vault</button><button class="btn btn-muted" onclick="document.getElementById('add-overlay').classList.add('hidden')">Cancel</button></div>
  </div>
</div>
</div>

<!-- CONFIRM DELETE -->

<div class="overlay hidden" id="conf-overlay">
<div class="confirm-box">
  <h3>Remove Bottle?</h3>
  <p id="conf-msg"></p>
  <div class="btn-row"><button class="btn btn-danger" id="conf-yes">Remove</button><button class="btn btn-muted" onclick="document.getElementById('conf-overlay').classList.add('hidden')">Cancel</button></div>
</div>
</div>

<script>
// ============================================================
// CONFIG
// ============================================================
const DNA_FAMILIES = {
  "Aquatic / Marine":{color:"#3a7585",desc:"Fresh marine, ozonic, sea-spray accords"},
  "Fougère":{color:"#3d6038",desc:"Lavender, oakmoss, coumarin — the classic masculine pillar"},
  "Woody / Aromatic":{color:"#8a6e2e",desc:"Sandalwood, cedarwood, vetiver, warm woods"},
  "Oriental / Amber":{color:"#c9a84c",desc:"Amber, benzoin, vanilla, spice, balsam"},
  "Oud / Resinous":{color:"#7a4a28",desc:"Oud, incense, frankincense, resinous bases"},
  "Citrus / Fresh":{color:"#909830",desc:"Bergamot, lemon, neroli, grapefruit"},
  "Gourmand":{color:"#b06840",desc:"Coffee, vanilla, caramel, tonka, sweet dessert accords"},
  "Floral":{color:"#b05a80",desc:"Rose, jasmine, iris, white flowers"},
  "Chypre":{color:"#507050",desc:"Oakmoss, labdanum, bergamot — earthy elegance"},
  "Tobacco / Smoky":{color:"#6a4a3a",desc:"Tobacco leaf, smoke, leather, tar"},
  "Musky / Skin":{color:"#6b6358",desc:"White musk, skin-close, animalic warmth"},
};

const DEFAULT_DNA = {
  "#Imagine":"Aquatic / Marine","Acqua Di DUA":"Aquatic / Marine","Bet On 67":"Fougère",
  "Bleu de Casino Elixir Extrait":"Woody / Aromatic","Bleu de Dua Attar":"Woody / Aromatic",
  "Bleu de Dua Exclusive Extrait":"Woody / Aromatic","Casino Royale Nights Extrait":"Oriental / Amber",
  "D Le Attar":"Woody / Aromatic","D Le Parfum Intense":"Woody / Aromatic",
  "Desert Reflection Extrait":"Floral","Drowning in Bleu de Dua Attar":"Woody / Aromatic",
  "Drowning Bleu de Savage Fierce Extrait":"Woody / Aromatic","His Intense Aspiration":"Fougère",
  "His Loyalty":"Floral","Fierce Savage":"Woody / Aromatic","His Royalty":"Floral",
  "Error 413":"Oriental / Amber","His Aspiration Extreme Sport":"Aquatic / Marine",
  "His OG Aspiration":"Fougère","His Perspective Extrait":"Woody / Aromatic",
  "Iconic Greenwich Village":"Fougère","Imperial Blue":"Aquatic / Marine",
  "Imperiale Casino Elixir":"Aquatic / Marine","Intuition Vision":"Aquatic / Marine",
  "Jazz Maison":"Tobacco / Smoky","Mystical Amulet of Blue":"Aquatic / Marine",
  "Peace with Poseidon":"Aquatic / Marine","Poseidon's Swimming Cologne":"Aquatic / Marine",
  "River Fougere":"Fougère","Rome in Yellow Dream":"Floral","Spice It Up Metallic Musk":"Oriental / Amber",
  "Stronger With Azure Supernova 2.0":"Aquatic / Marine","The Savage Attar":"Woody / Aromatic",
  "Iconic Plums By The Fire":"Gourmand","Poseidon's Fireplace":"Woody / Aromatic",
  "Dua's SoHo":"Fougère","Gentleman's Club":"Fougère","True Self Absolute":"Woody / Aromatic",
  "Poseidon's Cotton Candy":"Gourmand","Dua's Water Primal Essence":"Aquatic / Marine",
  "Rome In Coral Fantasy":"Floral","Midnight Candy For 1 & Only":"Oriental / Amber",
  "1 & Only Jazz Club":"Tobacco / Smoky","Victorian Poseidon":"Aquatic / Marine",
  "Ottoman Breeze":"Fougère","Aphrodisiac":"Oriental / Amber","Black Widow":"Gourmand",
  "City of Dua":"Woody / Aromatic","Midnight Rendezvous":"Woody / Aromatic",
  "Gone Swimming":"Aquatic / Marine","Cola Fizz Of Tonka Beans":"Gourmand",
  "Smoky Cuba Tabac":"Tobacco / Smoky","Fortune":"Oriental / Amber",
  "Supernova Cologne Intense":"Aquatic / Marine","Wooden Lucky Charm":"Woody / Aromatic",
  "Rome In Green":"Fougère","Queen Of The Chess":"Oriental / Amber","Midnight Fig Nest":"Citrus / Fresh","Midnight Fig":"Citrus / Fresh",
  "Black Origami":"Oriental / Amber","Daring Blue For Life":"Aquatic / Marine",
  "Glacier Bold":"Aquatic / Marine","Glacier Le Noir":"Fougère","Hercules":"Tobacco / Smoky",
  "Jean Lowe Immortal":"Aquatic / Marine","Jean Lowe Vibe":"Aquatic / Marine",
  "Error 410":"Oriental / Amber",
  "Poseidon's Ocean Mist":"Aquatic / Marine",
  "Ottomans Vert Breeze":"Fougère",
  "The Mobster vs Poseidon":"Woody / Aromatic",
  "Aroma of Heaven":"Woody / Aromatic",
  "Imperialé Matrix":"Aquatic / Marine",
  "Kismet Angel":"Gourmand","Perseus":"Fougère","Salvo Elixir":"Woody / Aromatic",
  "Salvo Intense":"Woody / Aromatic","Tobacco Touch":"Gourmand","Victorioso":"Aquatic / Marine",
  "Victorioso Myth":"Aquatic / Marine","Victorioso Nero":"Aquatic / Marine",
  "Yeah Man":"Woody / Aromatic","Your Touch Amber":"Oriental / Amber",
  "Your Touch Oud":"Oud / Resinous","Your Touch Sandal":"Woody / Aromatic",
  "Opulent Dubai":"Oud / Resinous","Mashrabya":"Tobacco / Smoky",
  "Ameer Al Oudh Intense":"Woody / Aromatic","Vintage Radio":"Oriental / Amber",
  "Najdia Intense":"Aquatic / Marine","Qaed Al Fursan":"Aquatic / Marine",
  "Hayatti Gold Elixir":"Oriental / Amber","Ana Abiyedh":"Musky / Skin",
  "Teriaq Intense":"Oriental / Amber","Liam Grey":"Musky / Skin",
  "Opulent Musk":"Oriental / Amber","Bade'e Al Oud For Glory":"Oud / Resinous",
  "Bade'e Al Oud Sublime":"Floral","Bade'e Al Oud Honor & Glory":"Oud / Resinous",
  "Bade'e Al Oud Amethyst":"Floral","Khamrah Qahwa":"Gourmand",
  "Suits":"Floral","Lust Cherry":"Gourmand","Intense Peach":"Gourmand",
  "Oud Wonder":"Oud / Resinous","Ebony Fume":"Woody / Aromatic",
  "Proud of You":"Oriental / Amber","Proud of You Absolute":"Oriental / Amber",
  "La Uno Million Elixir":"Oriental / Amber","Neroli Riviera":"Citrus / Fresh",
  "Grassland":"Fougère","Linen Vetiver":"Woody / Aromatic","Vintage Green 78":"Citrus / Fresh",
  "Tobacco & Tonka Bean":"Tobacco / Smoky","Midnight Hour":"Oriental / Amber",
  "Dark Cherry & Amber":"Oriental / Amber","Metal Rain":"Aquatic / Marine",
  "Bleu de Chanel EDT":"Woody / Aromatic","Montblanc Legend Spirit":"Aquatic / Marine",
  "Nautica Voyage":"Aquatic / Marine","Dior Sauvage EDP":"Woody / Aromatic",
  "Davidoff Cool Water":"Aquatic / Marine","Valencia Uomo Intense":"Floral",
  "Valencia Uomo Fantasy":"Floral","Valencia Uomo":"Floral","Millionaire Royal":"Oriental / Amber",
  "Island Dreams":"Floral","Shiyaaka Snow":"Aquatic / Marine","Shiyaaka Blue":"Woody / Aromatic",
  "Epoque Artistique":"Aquatic / Marine","Haven Eclipse":"Woody / Aromatic",
  "Secret Embers":"Oriental / Amber","Musk Melody":"Musky / Skin",
  "Reverence Extrait":"Fougère","The Exposed Extrait":"Fougère",
  "Fattan":"Woody / Aromatic","Hawas Ice":"Aquatic / Marine","Hawas Kobra":"Aquatic / Marine",
  "Itqan Noir":"Woody / Aromatic","Reverie Aqua Pour Homme":"Aquatic / Marine",
  "Abadi Opulent":"Woody / Aromatic","Wazir":"Oriental / Amber","Raazi":"Fougère",
  "Rayees":"Fougère","Nor":"Aquatic / Marine","Limitless":"Fougère","Gladiator":"Oriental / Amber",
  "Le Parfait":"Fougère","Club de Nuit Milestone":"Aquatic / Marine",
  "Anti Social Parfum Club - Most Wanted":"Oriental / Amber",
  "Afnan Supremacy Collector's Edition":"Aquatic / Marine","Ajmal Evoke Gold":"Woody / Aromatic",
  "Al Haramain Detour Noir":"Woody / Aromatic","Crown / Al-Rehab Silver (oil)":"Aquatic / Marine",
  "Atralia Amazonas Avalanche":"Floral","French Avenue Liquid Brun":"Woody / Aromatic",
  "Game of Spades Wildcard":"Woody / Aromatic","Grandeur Iconic Built":"Woody / Aromatic",
  "Paris Corner Rifaqat":"Musky / Skin","Rayhaan Aquatica":"Aquatic / Marine",
  "Royalty by Maluma Onyx":"Oriental / Amber","Vurv Royce Black":"Oriental / Amber",
  "MIRIS No54602":"Fougère","MIRIS No56902":"Gourmand",
  "MIRIS No47319":"Oriental / Amber","MIRIS No59797":"Woody / Aromatic",
};

const SEAS = {ss:"Spring · Summer",fw:"Fall · Winter",yr:"Year-round"};
const OCC_LBL = {date:"♥ Date",office:"◆ Office",evening:"✦ Evening",casual:"■ Casual",sport:"▲ Sport",special:"★ Special"};
const OCC_CLS = {date:"td",office:"to",evening:"te",casual:"tc",sport:"ts",special:"tsp"};

// ============================================================
// DEFAULT DATA
// ============================================================
const DEFAULT_COL=[
  // THE DUA BRAND — 64 bottles
  {house:"The Dua Brand",name:"#Imagine",inspiration:"Louis Vuitton Imagination",occ_key:"casual",occ_detail:"Casual / daytime errands",s_key:"ss"},
  {house:"The Dua Brand",name:"Acqua Di DUA",inspiration:"Acqua di Giò (OG/vintage style)",occ_key:"casual",occ_detail:"Casual / beach / gym",s_key:"ss"},
  {house:"The Dua Brand",name:"Bet On 67",inspiration:"Ralph Lauren Polo 67",occ_key:"sport",occ_detail:"Casual outdoors / sport",s_key:"ss"},
  {house:"The Dua Brand",name:"Bleu de Casino Elixir Extrait",inspiration:"Bleu de Chanel + Aventus + BR540 Extrait",occ_key:"date",occ_detail:"Date night / upscale casual",s_key:"fw"},
  {house:"The Dua Brand",name:"Bleu de Dua Attar",inspiration:"Bleu de Chanel (attar style)",occ_key:"office",occ_detail:"Office / smart casual",s_key:"yr",starred:true,isBase:true},
  {house:"The Dua Brand",name:"Bleu de Dua Exclusive Extrait",inspiration:"Bleu de Chanel L'Exclusif",occ_key:"office",occ_detail:"Business formal / special occasion",s_key:"fw"},
  {house:"The Dua Brand",name:"Casino Royale Nights Extrait",inspiration:"Baccarat Rouge 540 Extrait",occ_key:"date",occ_detail:"Date night / cocktail event",s_key:"fw"},
  {house:"The Dua Brand",name:"D Le Attar",inspiration:"YSL Y Le Parfum",occ_key:"office",occ_detail:"Office / date night",s_key:"fw"},
  {house:"The Dua Brand",name:"D Le Parfum Intense",inspiration:"YSL Y EDP Intense",occ_key:"evening",occ_detail:"Evening / formal",s_key:"fw"},
  {house:"The Dua Brand",name:"Desert Reflection Extrait",inspiration:"Amouage Reflection Man",occ_key:"special",occ_detail:"Special occasion / formal",s_key:"fw"},
  {house:"The Dua Brand",name:"Drowning in Bleu de Dua Attar",inspiration:"Bleu de Chanel + Nishane Ani",occ_key:"date",occ_detail:"Date night / upscale",s_key:"fw"},
  {house:"The Dua Brand",name:"Drowning Bleu de Savage Fierce Extrait",inspiration:"Ani + Sauvage EDT + Fierce + Bleu de Chanel",occ_key:"evening",occ_detail:"Night out / clubbing",s_key:"fw"},
  {house:"The Dua Brand",name:"His Intense Aspiration",inspiration:"Allure Homme Blanche + Allure Homme Sport Eau Extreme",occ_key:"office",occ_detail:"Office / smart casual",s_key:"ss"},
  {house:"The Dua Brand",name:"His Loyalty",inspiration:"D&G Devotion Pour Homme",occ_key:"casual",occ_detail:"Casual / social",s_key:"ss"},
  {house:"The Dua Brand",name:"Fierce Savage",inspiration:"Abercrombie Fierce + Dior Sauvage EDT",occ_key:"sport",occ_detail:"Casual / gym / outdoors",s_key:"ss"},
  {house:"The Dua Brand",name:"His Royalty",inspiration:"Prada L'Homme L'Eau",occ_key:"office",occ_detail:"Office / light date",s_key:"ss"},
  {house:"The Dua Brand",name:"Error 410",inspiration:"Paco Rabanne 1 Million Absolutely Gold",occ_key:"date",occ_detail:"Date night / evening / upscale social",s_key:"fw"},
  {house:"The Dua Brand",name:"Error 413",inspiration:"1 Million Lucky",occ_key:"evening",occ_detail:"Night out / social",s_key:"fw"},
  {house:"The Dua Brand",name:"His Aspiration Extreme Sport",inspiration:"Chanel Allure Homme Sport Eau Extrême",occ_key:"sport",occ_detail:"Sport / casual / gym",s_key:"ss"},
  {house:"The Dua Brand",name:"His OG Aspiration",inspiration:"Chanel Allure Homme (1999 vintage)",occ_key:"office",occ_detail:"Office / smart casual",s_key:"fw"},
  {house:"The Dua Brand",name:"His Perspective Extrait",inspiration:"Prada Paradigme",occ_key:"office",occ_detail:"Office / date night / layering base",s_key:"yr",isBase:true},
  {house:"The Dua Brand",name:"Iconic Greenwich Village",inspiration:"Bond No. 9 Greenwich Village",occ_key:"casual",occ_detail:"Urban casual / creative social",s_key:"ss"},
  {house:"The Dua Brand",name:"Imperial Blue",inspiration:"Bleu de Chanel + Creed Millésime Impérial",occ_key:"date",occ_detail:"Upscale casual / date",s_key:"ss"},
  {house:"The Dua Brand",name:"Imperiale Casino Elixir",inspiration:"Millésime Impérial + Aventus + BR540 Extrait",occ_key:"special",occ_detail:"Special occasion / formal",s_key:"ss"},
  {house:"The Dua Brand",name:"Intuition Vision",inspiration:"Acqua di Giò Profumo",occ_key:"office",occ_detail:"Smart casual / office",s_key:"ss"},
  {house:"The Dua Brand",name:"Jazz Maison",inspiration:"Maison Margiela Jazz Club",occ_key:"evening",occ_detail:"Evening social / bar / lounge",s_key:"fw"},
  {house:"The Dua Brand",name:"Mystical Amulet of Blue",inspiration:"Ex Nihilo Blue Talisman",occ_key:"casual",occ_detail:"Casual / everyday",s_key:"ss"},
  {house:"The Dua Brand",name:"Peace with Poseidon",inspiration:"Scent of Peace + Aventus",occ_key:"casual",occ_detail:"Casual / outdoors / weekend",s_key:"ss"},
  {house:"The Dua Brand",name:"Poseidon's Swimming Cologne",inspiration:"Aventus Cologne + LV Afternoon Swim",occ_key:"casual",occ_detail:"Casual / beach / sport",s_key:"ss",isBase:true},
  {house:"The Dua Brand",name:"Poseidon's Ocean Mist",inspiration:"Creed Aventus Cologne × Nautica Voyage",occ_key:"casual",occ_detail:"Casual / office / daytime / outdoors / weekend",s_key:"ss"},
  {house:"The Dua Brand",name:"River Fougere",inspiration:"YSL Rive Gauche Pour Homme",occ_key:"office",occ_detail:"Office / smart casual / retro",s_key:"ss"},
  {house:"The Dua Brand",name:"Rome in Yellow Dream",inspiration:"Valentino Born in Roma Yellow Dream",occ_key:"date",occ_detail:"Date / upscale casual",s_key:"ss"},
  {house:"The Dua Brand",name:"Spice It Up Metallic Musk",inspiration:"Viktor & Rolf Spicebomb Metallic Musk",occ_key:"office",occ_detail:"Smart casual / office",s_key:"fw"},
  {house:"The Dua Brand",name:"Stronger With Azure Supernova 2.0",inspiration:"Stronger With You + ADG Profondo + Roja Elysium + Aventus",occ_key:"date",occ_detail:"Date night / evening",s_key:"fw"},
  {house:"The Dua Brand",name:"The Savage Attar",inspiration:"Dior Sauvage Parfum",occ_key:"date",occ_detail:"Date night / upscale casual",s_key:"yr"},
  {house:"The Dua Brand",name:"Iconic Plums By The Fire",inspiration:"Andy Warhol + By the Fireplace",occ_key:"evening",occ_detail:"Evening / cozy / lounge",s_key:"fw"},
  {house:"The Dua Brand",name:"Poseidon's Fireplace",inspiration:"Aventus + By the Fireplace",occ_key:"date",occ_detail:"Evening / lounge / date",s_key:"fw"},
  {house:"The Dua Brand",name:"Dua's SoHo",inspiration:"Bond No. 9 Soho",occ_key:"casual",occ_detail:"Urban casual / creative social",s_key:"ss"},
  {house:"The Dua Brand",name:"Gentleman's Club",inspiration:"Givenchy Gentleman Society",occ_key:"date",occ_detail:"Business casual / date",s_key:"fw"},
  {house:"The Dua Brand",name:"True Self Absolute",inspiration:"YSL MYSLF L'Absolu",occ_key:"date",occ_detail:"Date night / evening",s_key:"fw"},
  {house:"The Dua Brand",name:"Poseidon's Cotton Candy",inspiration:"Aventus + Cotton Candy De Dua",occ_key:"casual",occ_detail:"Casual / fun social / playful",s_key:"ss"},
  {house:"The Dua Brand",name:"Dua's Water Primal Essence",inspiration:"Acqua di Giò Absolu",occ_key:"office",occ_detail:"Office / casual / gym",s_key:"ss"},
  {house:"The Dua Brand",name:"Rome In Coral Fantasy",inspiration:"Valentino Born in Roma Coral Fantasy",occ_key:"date",occ_detail:"Date / warm-weather casual",s_key:"ss"},
  {house:"The Dua Brand",name:"Midnight Candy For 1 & Only",inspiration:"La Nuit de L'Homme + Candies for Men + The One",occ_key:"evening",occ_detail:"Evening / date night / club",s_key:"fw"},
  {house:"The Dua Brand",name:"1 & Only Jazz Club",inspiration:"The One + Jazz Club",occ_key:"evening",occ_detail:"Evening / lounge / date",s_key:"fw"},
  {house:"The Dua Brand",name:"Victorian Poseidon",inspiration:"Aventus + Xerjoff 1861 Renaissance",occ_key:"special",occ_detail:"Formal / special occasion",s_key:"fw"},
  {house:"The Dua Brand",name:"Ottoman Breeze",inspiration:"Nishane Hacivat",occ_key:"casual",occ_detail:"Casual / office / everyday (layering base)",s_key:"ss",isBase:true},
  {house:"The Dua Brand",name:"Ottomans Vert Breeze",inspiration:"Nishane Hacivat × Creed Green Irish Tweed",occ_key:"casual",occ_detail:"Casual / office / outdoors / weekend",s_key:"ss"},
  {house:"The Dua Brand",name:"Aphrodisiac",inspiration:"Initio Psychedelic Love",occ_key:"date",occ_detail:"Date night / intimate / evening",s_key:"fw"},
  {house:"The Dua Brand",name:"Black Widow",inspiration:"Kilian Black Phantom",occ_key:"evening",occ_detail:"Evening / date night / club",s_key:"fw"},
  {house:"The Dua Brand",name:"City of Dua",inspiration:"Louis Vuitton City of Stars",occ_key:"evening",occ_detail:"Smart casual / evening",s_key:"fw"},
  {house:"The Dua Brand",name:"Midnight Rendezvous",inspiration:"YSL La Nuit de L'Homme",occ_key:"date",occ_detail:"Date night / evening / club",s_key:"fw"},
  {house:"The Dua Brand",name:"Gone Swimming",inspiration:"Louis Vuitton Afternoon Swim",occ_key:"casual",occ_detail:"Casual / beach / poolside",s_key:"ss"},
  {house:"The Dua Brand",name:"Cola Fizz Of Tonka Beans",inspiration:"Mancera Tonka Cola",occ_key:"casual",occ_detail:"Casual / fun / social",s_key:"yr"},
  {house:"The Dua Brand",name:"Smoky Cuba Tabac",inspiration:"Alghabra Parfums Cuban Tobacco",occ_key:"evening",occ_detail:"Evening / lounge / special occasion",s_key:"fw"},
  {house:"The Dua Brand",name:"Fortune",inspiration:"Xerjoff Naxos",occ_key:"date",occ_detail:"Date night / evening / romantic",s_key:"fw"},
  {house:"The Dua Brand",name:"Supernova Cologne Intense",inspiration:"Roja Parfums Elysium Eau Intense",occ_key:"office",occ_detail:"Smart casual / office / gym",s_key:"ss"},
  {house:"The Dua Brand",name:"Wooden Lucky Charm",inspiration:"Dior Bois Talisman",occ_key:"evening",occ_detail:"Smart casual / evening",s_key:"fw"},
  {house:"The Dua Brand",name:"Rome In Green",inspiration:"Valentino Uomo Born in Roma Green Stravaganza",occ_key:"casual",occ_detail:"Casual / outdoors / weekend",s_key:"ss"},
  {house:"The Dua Brand",name:"Queen Of The Chess",inspiration:"Mind Games Queening",occ_key:"date",occ_detail:"Date / upscale casual / evening",s_key:"fw"},
  {house:"The Dua Brand",name:"Midnight Fig",inspiration:"Nest Indigo",occ_key:"evening",occ_detail:"Evening / special occasion / mysterious",s_key:"fw"},
  {house:"The Dua Brand",name:"The Mobster vs Poseidon",inspiration:"Roja Creation-E × Creed Aventus",occ_key:"date",occ_detail:"Date night / upscale casual / evening social",s_key:"fw"},
  {house:"The Dua Brand",name:"Aroma of Heaven",inspiration:"Hermès Terre d'Hermès (Vintage)",occ_key:"office",occ_detail:"Office / smart casual / daytime / outdoors",s_key:"yr"},
  {house:"The Dua Brand",name:"Imperialé Matrix",inspiration:"Creed Millésime Impérial × Xerjoff Nio",occ_key:"office",occ_detail:"Office / smart casual / daytime / upscale casual",s_key:"ss"},
  // MAISON ALHAMBRA — 19 bottles
  {house:"Maison Alhambra",name:"Black Origami",inspiration:"Tom Ford Black Orchid",occ_key:"date",occ_detail:"Evening / date night / special occasion",s_key:"fw"},
  {house:"Maison Alhambra",name:"Daring Blue For Life",inspiration:"D&G Light Blue Forever",occ_key:"casual",occ_detail:"Casual / beach / everyday",s_key:"ss"},
  {house:"Maison Alhambra",name:"Glacier Bold",inspiration:"JPG Le Beau Le Parfum",occ_key:"casual",occ_detail:"Casual / social / gym",s_key:"ss"},
  {house:"Maison Alhambra",name:"Glacier Le Noir",inspiration:"JPG Le Male Le Parfum",occ_key:"evening",occ_detail:"Date night / club / evening",s_key:"fw"},
  {house:"Maison Alhambra",name:"Hercules",inspiration:"Parfums de Marly Herod",occ_key:"evening",occ_detail:"Evening / formal / date",s_key:"fw"},
  {house:"Maison Alhambra",name:"Jean Lowe Immortal",inspiration:"Louis Vuitton L'Immensité",occ_key:"office",occ_detail:"Smart casual / office / layering base",s_key:"ss",isBase:true},
  {house:"Maison Alhambra",name:"Jean Lowe Vibe",inspiration:"Louis Vuitton Pacific Chill",occ_key:"casual",occ_detail:"Casual / beach / weekend",s_key:"ss"},
  {house:"Maison Alhambra",name:"Kismet Angel",inspiration:"Kilian Angel's Share",occ_key:"date",occ_detail:"Evening / date night / cozy lounge",s_key:"fw"},
  {house:"Maison Alhambra",name:"Perseus",inspiration:"Parfums de Marly Pegasus",occ_key:"office",occ_detail:"Office / smart casual / date",s_key:"yr"},
  {house:"Maison Alhambra",name:"Salvo Elixir",inspiration:"Dior Sauvage Elixir",occ_key:"date",occ_detail:"Date night / evening / special occasion",s_key:"fw"},
  {house:"Maison Alhambra",name:"Salvo Intense",inspiration:"Dior Sauvage EDP",occ_key:"office",occ_detail:"Casual / office / everyday",s_key:"yr"},
  {house:"Maison Alhambra",name:"Tobacco Touch",inspiration:"Tom Ford Tobacco Vanille",occ_key:"date",occ_detail:"Evening / cozy / romantic / winter date",s_key:"fw"},
  {house:"Maison Alhambra",name:"Victorioso",inspiration:"Paco Rabanne Invictus",occ_key:"sport",occ_detail:"Sport / casual / gym / daytime",s_key:"ss"},
  {house:"Maison Alhambra",name:"Victorioso Myth",inspiration:"Invictus Legend",occ_key:"date",occ_detail:"Date night / upscale casual",s_key:"fw"},
  {house:"Maison Alhambra",name:"Victorioso Nero",inspiration:"Invictus Victory / Victory Elixir",occ_key:"date",occ_detail:"Date night / evening / formal",s_key:"fw"},
  {house:"Maison Alhambra",name:"Yeah Man",inspiration:"YSL Y EDP",occ_key:"office",occ_detail:"Office / casual / everyday",s_key:"yr"},
  {house:"Maison Alhambra",name:"Your Touch Amber",inspiration:"Armani Stronger With You Amber",occ_key:"date",occ_detail:"Date night / cozy evening",s_key:"fw"},
  {house:"Maison Alhambra",name:"Your Touch Oud",inspiration:"Armani Stronger With You Oud",occ_key:"special",occ_detail:"Evening / special occasion / date",s_key:"fw"},
  {house:"Maison Alhambra",name:"Your Touch Sandal",inspiration:"Armani Stronger With You Sandalwood",occ_key:"date",occ_detail:"Smart casual / date / evening",s_key:"fw"},
  // LATTAFA — 16 bottles
  {house:"Lattafa",name:"Opulent Dubai",inspiration:"God of Fire Original DNA",occ_key:"special",occ_detail:"Special occasion / evening / statement",s_key:"fw"},
  {house:"Lattafa",name:"Mashrabya",inspiration:"Initio Smoking Hot",occ_key:"evening",occ_detail:"Evening / club / date night",s_key:"fw"},
  {house:"Lattafa",name:"Ameer Al Oudh Intense",inspiration:"Maison Margiela By the Fireplace",occ_key:"evening",occ_detail:"Cozy evening / lounge / layering",s_key:"fw",isBase:true},
  {house:"Lattafa",name:"Vintage Radio",inspiration:"Initio Paragon",occ_key:"date",occ_detail:"Date night / evening / special occasion",s_key:"fw"},
  {house:"Lattafa",name:"Najdia Intense",inspiration:"JPG Le Beau Paradise Garden",occ_key:"casual",occ_detail:"Casual / daytime / social",s_key:"ss"},
  {house:"Lattafa",name:"Qaed Al Fursan",inspiration:"Creed Aventus",occ_key:"office",occ_detail:"Office / smart casual / daytime",s_key:"ss"},
  {house:"Lattafa",name:"Hayatti Gold Elixir",inspiration:"Armani Code Profumo",occ_key:"date",occ_detail:"Date night / evening / club",s_key:"fw"},
  {house:"Lattafa",name:"Ana Abiyedh",inspiration:"White Musk Original",occ_key:"casual",occ_detail:"Casual / office / everyday / skin scent",s_key:"yr"},
  {house:"Lattafa",name:"Teriaq Intense",inspiration:"Original",occ_key:"evening",occ_detail:"Evening / statement / bold",s_key:"fw"},
  {house:"Lattafa",name:"Liam Grey",inspiration:"BDK Gris Charnel",occ_key:"date",occ_detail:"Smart casual / date / minimalist chic",s_key:"fw"},
  {house:"Lattafa",name:"Opulent Musk",inspiration:"BR540 x Initio Instant Crush",occ_key:"date",occ_detail:"Date night / social / evening",s_key:"yr"},
  {house:"Lattafa",name:"Bade'e Al Oud For Glory",inspiration:"Initio Oud for Greatness",occ_key:"special",occ_detail:"Special occasion / evening / statement",s_key:"fw"},
  {house:"Lattafa",name:"Bade'e Al Oud Sublime",inspiration:"Kayali Eden Juicy Apple",occ_key:"casual",occ_detail:"Casual / fun / social / daytime",s_key:"ss"},
  {house:"Lattafa",name:"Bade'e Al Oud Honor & Glory",inspiration:"Original / house blend",occ_key:"evening",occ_detail:"Evening / statement / bold",s_key:"fw"},
  {house:"Lattafa",name:"Bade'e Al Oud Amethyst",inspiration:"Initio Atomic Rose",occ_key:"date",occ_detail:"Date night / floral evening / romantic",s_key:"fw"},
  {house:"Lattafa",name:"Khamrah Qahwa",inspiration:"Original",occ_key:"evening",occ_detail:"Cozy / evening / lounge / cold weather treat",s_key:"fw",starred:true},
  // FRAGRANCE WORLD — 9 bottles
  {house:"Fragrance World",name:"Suits",inspiration:"YSL Tuxedo",occ_key:"special",occ_detail:"Formal / evening / special occasion",s_key:"fw"},
  {house:"Fragrance World",name:"Lust Cherry",inspiration:"Tom Ford Lost Cherry",occ_key:"date",occ_detail:"Date night / evening / romantic",s_key:"fw"},
  {house:"Fragrance World",name:"Intense Peach",inspiration:"Tom Ford Bitter Peach",occ_key:"evening",occ_detail:"Evening / bold social / date",s_key:"fw"},
  {house:"Fragrance World",name:"Oud Wonder",inspiration:"Tom Ford Oud Wood",occ_key:"office",occ_detail:"Smart casual / office / date",s_key:"fw"},
  {house:"Fragrance World",name:"Ebony Fume",inspiration:"Tom Ford Ebene Fume",occ_key:"special",occ_detail:"Evening / formal / special occasion",s_key:"fw"},
  {house:"Fragrance World",name:"Proud of You",inspiration:"Armani Stronger With You",occ_key:"office",occ_detail:"Office / casual / everyday",s_key:"fw"},
  {house:"Fragrance World",name:"Proud of You Absolute",inspiration:"Armani Stronger With You Absolutely",occ_key:"date",occ_detail:"Date night / evening / upscale",s_key:"fw"},
  {house:"Fragrance World",name:"La Uno Million Elixir",inspiration:"Paco Rabanne 1 Million Elixir",occ_key:"evening",occ_detail:"Date night / club / evening",s_key:"fw"},
  {house:"Fragrance World",name:"Neroli Riviera",inspiration:"Tom Ford Neroli Portofino",occ_key:"casual",occ_detail:"Casual / beach / vacation / daytime",s_key:"ss"},
  // BANANA REPUBLIC — 7 bottles
  {house:"Banana Republic",name:"Grassland",inspiration:"Creed Green Irish Tweed (style)",occ_key:"office",occ_detail:"Smart casual / office / daytime",s_key:"ss"},
  {house:"Banana Republic",name:"Linen Vetiver",inspiration:"Original",occ_key:"office",occ_detail:"Office / minimalist casual / summer work",s_key:"ss"},
  {house:"Banana Republic",name:"Vintage Green 78",inspiration:"Original",occ_key:"casual",occ_detail:"Casual / weekend / outdoors",s_key:"ss"},
  {house:"Banana Republic",name:"Tobacco & Tonka Bean",inspiration:"Original",occ_key:"date",occ_detail:"Cozy evening / lounge / casual date",s_key:"fw"},
  {house:"Banana Republic",name:"Midnight Hour",inspiration:"Original",occ_key:"evening",occ_detail:"Evening / date / social",s_key:"fw"},
  {house:"Banana Republic",name:"Dark Cherry & Amber",inspiration:"Original",occ_key:"date",occ_detail:"Date night / cozy evening",s_key:"fw"},
  {house:"Banana Republic",name:"Metal Rain",inspiration:"Original",occ_key:"casual",occ_detail:"Casual / outdoors / fresh air vibe",s_key:"ss"},
  // DESIGNER ORIGINALS — 5 bottles
  {house:"Designer Originals",name:"Bleu de Chanel EDT",inspiration:"Original",occ_key:"office",occ_detail:"Versatile / office / casual / date",s_key:"yr"},
  {house:"Designer Originals",name:"Montblanc Legend Spirit",inspiration:"Original",occ_key:"casual",occ_detail:"Casual / sport / everyday",s_key:"ss"},
  {house:"Designer Originals",name:"Nautica Voyage",inspiration:"Original",occ_key:"casual",occ_detail:"Casual / fresh / everyday / gym",s_key:"ss"},
  {house:"Designer Originals",name:"Dior Sauvage EDP",inspiration:"Original",occ_key:"office",occ_detail:"Office / casual / date night",s_key:"yr"},
  {house:"Designer Originals",name:"Davidoff Cool Water",inspiration:"Original",occ_key:"sport",occ_detail:"Casual / sport / gym / beach",s_key:"ss"},
  // VALENCIA / MILLIONAIRE — 4 bottles
  {house:"Valencia / Millionaire",name:"Valencia Uomo Intense",inspiration:"Valentino Uomo Intense",occ_key:"date",occ_detail:"Date night / evening / romantic",s_key:"fw"},
  {house:"Valencia / Millionaire",name:"Valencia Uomo Fantasy",inspiration:"Valentino Born in Roma Coral Fantasy",occ_key:"casual",occ_detail:"Casual / daytime / warm weather",s_key:"ss"},
  {house:"Valencia / Millionaire",name:"Valencia Uomo",inspiration:"Valentino Born in Roma",occ_key:"casual",occ_detail:"Casual / smart casual / daytime",s_key:"ss"},
  {house:"Valencia / Millionaire",name:"Millionaire Royal",inspiration:"Paco Rabanne 1 Million Royal",occ_key:"date",occ_detail:"Date night / club / evening",s_key:"fw"},
  // KHADLAJ — 4 bottles
  {house:"Khadlaj",name:"Island Dreams",inspiration:"Louis Vuitton Symphony",occ_key:"date",occ_detail:"Upscale casual / date / evening",s_key:"ss"},
  {house:"Khadlaj",name:"Shiyaaka Snow",inspiration:"Louis Vuitton Météore",occ_key:"office",occ_detail:"Smart casual / office / daytime",s_key:"ss"},
  {house:"Khadlaj",name:"Shiyaaka Blue",inspiration:"Bleu de Chanel (style)",occ_key:"office",occ_detail:"Office / casual / everyday",s_key:"yr"},
  {house:"Khadlaj",name:"Epoque Artistique",inspiration:"Invictus Victory / Victory Elixir",occ_key:"date",occ_detail:"Date night / evening / formal",s_key:"fw"},
  // MOD FRAGRANCES — 5 bottles
  {house:"Mod Fragrances",name:"Haven Eclipse",inspiration:"Xerjoff Torino 22",occ_key:"date",occ_detail:"Smart casual / date / evening",s_key:"fw"},
  {house:"Mod Fragrances",name:"Secret Embers",inspiration:"Initio Side Effect",occ_key:"date",occ_detail:"Date night / evening / seductive",s_key:"fw"},
  {house:"Mod Fragrances",name:"Musk Melody",inspiration:"Initio Musk Therapy",occ_key:"casual",occ_detail:"Casual / skin-close / everyday",s_key:"yr"},
  {house:"Mod Fragrances",name:"Reverence Extrait",inspiration:"Parfums de Marly Percival",occ_key:"office",occ_detail:"Smart casual / office / date",s_key:"ss"},
  {house:"Mod Fragrances",name:"The Exposed Extrait",inspiration:"Mind Games En Prise",occ_key:"evening",occ_detail:"Evening / bold / statement",s_key:"fw"},
  // RASASI — 3 bottles
  {house:"Rasasi",name:"Fattan",inspiration:"Terre d'Hermès",occ_key:"office",occ_detail:"Office / casual / everyday",s_key:"yr"},
  {house:"Rasasi",name:"Hawas Ice",inspiration:"Original",occ_key:"sport",occ_detail:"Sport / gym / casual / fresh",s_key:"ss"},
  {house:"Rasasi",name:"Hawas Kobra",inspiration:"Louis Vuitton Imagination",occ_key:"casual",occ_detail:"Casual / daytime / social",s_key:"ss"},
  // ZIMAYA — 3 bottles
  {house:"Zimaya",name:"Itqan Noir",inspiration:"YSL MYSLF",occ_key:"date",occ_detail:"Smart casual / date / evening",s_key:"fw"},
  {house:"Zimaya",name:"Reverie Aqua Pour Homme",inspiration:"Valentino Born in Roma Intense",occ_key:"office",occ_detail:"Casual / office / daytime",s_key:"ss"},
  {house:"Zimaya",name:"Abadi Opulent",inspiration:"YSL Y Elixir",occ_key:"date",occ_detail:"Date night / upscale casual / evening",s_key:"fw"},
  // YOM & LAYL — 6 bottles
  {house:"Yom & Layl",name:"Wazir",inspiration:"Mind Games Queening",occ_key:"date",occ_detail:"Date / upscale casual / evening",s_key:"fw"},
  {house:"Yom & Layl",name:"Raazi",inspiration:"Mind Games J'Adoube",occ_key:"evening",occ_detail:"Smart casual / social / evening",s_key:"fw"},
  {house:"Yom & Layl",name:"Rayees",inspiration:"Mind Games Grand Masters",occ_key:"office",occ_detail:"Office / smart casual / daytime",s_key:"ss"},
  {house:"Yom & Layl",name:"Nor",inspiration:"Mind Games Lionora",occ_key:"casual",occ_detail:"Casual / fresh / daytime",s_key:"ss"},
  {house:"Yom & Layl",name:"Limitless",inspiration:"Mind Games Blockade",occ_key:"evening",occ_detail:"Evening / bold / statement",s_key:"fw"},
  {house:"Yom & Layl",name:"Gladiator",inspiration:"Argos Triumph of Bacchus",occ_key:"special",occ_detail:"Special occasion / evening / grand statement",s_key:"fw"},
  // ARMAF — 2 bottles
  {house:"Armaf",name:"Le Parfait",inspiration:"Creed Aventus x Green Irish Tweed",occ_key:"office",occ_detail:"Office / smart casual / daytime",s_key:"ss"},
  {house:"Armaf",name:"Club de Nuit Milestone",inspiration:"Creed Millésime Impérial",occ_key:"casual",occ_detail:"Smart casual / beach / summer date",s_key:"ss"},
  // SINGLES — 13 bottles
  {house:"Anti Social Parfum Club",name:"Anti Social Parfum Club - Most Wanted",inspiration:"Azzaro The Most Wanted",occ_key:"date",occ_detail:"Date night / casual evening / social",s_key:"fw"},
  {house:"Afnan",name:"Afnan Supremacy Collector's Edition",inspiration:"Creed Aventus Absolu",occ_key:"office",occ_detail:"Smart casual / office / date",s_key:"ss"},
  {house:"Ajmal",name:"Ajmal Evoke Gold",inspiration:"Prada L'Homme",occ_key:"office",occ_detail:"Office / smart casual / everyday",s_key:"yr"},
  {house:"Al Haramain",name:"Al Haramain Detour Noir",inspiration:"Parfums de Marly Layton",occ_key:"date",occ_detail:"Date night / office / versatile dresser",s_key:"fw"},
  {house:"Al-Rehab",name:"Crown / Al-Rehab Silver (oil)",inspiration:"Creed Silver Mountain Water",occ_key:"casual",occ_detail:"Casual / fresh / gym / daytime",s_key:"ss"},
  {house:"Atralia",name:"Atralia Amazonas Avalanche",inspiration:"Dior Homme Intense",occ_key:"date",occ_detail:"Date night / evening / formal",s_key:"fw"},
  {house:"French Avenue",name:"French Avenue Liquid Brun",inspiration:"Parfums de Marly Althair",occ_key:"date",occ_detail:"Smart casual / date / evening",s_key:"fw"},
  {house:"Game of Spades",name:"Game of Spades Wildcard",inspiration:"Bond No. 9 Lafayette Street",occ_key:"evening",occ_detail:"Urban social / evening / creative",s_key:"fw"},
  {house:"Grandeur",name:"Grandeur Iconic Built",inspiration:"YSL Bleu Electrique",occ_key:"evening",occ_detail:"Club / night out / bold evening",s_key:"fw"},
  {house:"Paris Corner",name:"Paris Corner Rifaqat",inspiration:"YSL Babycat",occ_key:"casual",occ_detail:"Casual / cozy / skin-close everyday",s_key:"fw"},
  {house:"Rayhaan",name:"Rayhaan Aquatica",inspiration:"Creed Virgin Island Water",occ_key:"casual",occ_detail:"Beach / vacation / casual summer",s_key:"ss"},
  {house:"Royalty by Maluma",name:"Royalty by Maluma Onyx",inspiration:"1 Million Privé-adjacent",occ_key:"date",occ_detail:"Date night / club / evening",s_key:"fw"},
  {house:"Vurv",name:"Vurv Royce Black",inspiration:"1 Million Privé-adjacent",occ_key:"date",occ_detail:"Date night / club / evening",s_key:"fw"},
  // MIRIS OILS — 4 bottles
  {house:"MIRIS Oils",name:"MIRIS No54602",inspiration:"Nishane Hacivat",occ_key:"casual",occ_detail:"Casual / office / everyday / layering",s_key:"ss",isBase:true},
  {house:"MIRIS Oils",name:"MIRIS No56902",inspiration:"Kilian Apple Brandy on the Rocks",occ_key:"date",occ_detail:"Cozy evening / social / casual date",s_key:"fw"},
  {house:"MIRIS Oils",name:"MIRIS No47319",inspiration:"JPG Ultra Male",occ_key:"evening",occ_detail:"Night out / club / date",s_key:"fw"},
  {house:"MIRIS Oils",name:"MIRIS No59797",inspiration:"Carolina Herrera Bad Boy Cobalt Parfum Electrique",occ_key:"date",occ_detail:"Date night / evening / bold",s_key:"fw"},
];
const DEFAULT_LAYERS=[
  {items:["Ottoman Breeze","His Perspective Extrait"],ratio:"2 + 2",desc:"Hacivat's green freshness married to Paradigme's powdery woods — an elevated office signature that outperforms either alone."},
  {items:["Poseidon's Swimming Cologne","His Perspective Extrait"],ratio:"2 + 2",desc:"Aquatic chroma with a powdery musc anchor. The Afternoon Swim DNA turns brighter against Paradigme — beach-to-business in a single wear."},
  {items:["Jean Lowe Immortal","Ameer Al Oudh Intense"],ratio:"2 : 1",desc:"L'Immensité's mineral-aquatic shimmer wrapped in By the Fireplace's smoked wood. 2:1 keeps aquatic brightness while oud grounds the sillage."},
  {items:["Midnight Rendezvous","Aphrodisiac","Wazir"],ratio:"Trio",desc:"La Nuit de L'Homme base, Psychedelic Love heat, Wazir oil as skin anchor — a bold indoor evening statement."},
  {items:["MIRIS No54602","His Perspective Extrait"],ratio:"Oil + Spray",desc:"MIRIS oil as skin-prep base before His Perspective Extrait — locks in Hacivat DNA and extends projection significantly on warm days."},
  {items:["Ottoman Breeze","Poseidon's Swimming Cologne"],ratio:"2 + 2",desc:"Double-stacking the Hacivat/Aventus Cologne axis to create a saturated aquatic-fougère summer statement."},
];

// ============================================================
// DB
// ============================================================
let DB={col:[],layers:[],st:{}};

function uid(){return Math.random().toString(36).slice(2,9);}

function loadDB(){
  try{
    const s=JSON.parse(localStorage.getItem('vault3')||'null');
    if(s&&s.col&&s.col.length){DB=s;return;}
  }catch{}
  DB.col=DEFAULT_COL.map(f=>({...f}));
  DB.layers=DEFAULT_LAYERS.map(l=>({...l,id:uid()}));
  DB.st={};
  DB.col.forEach(f=>{
    DB.st[f.name]={};
    if(DEFAULT_DNA[f.name])DB.st[f.name].dna=DEFAULT_DNA[f.name];
    if(f.starred)DB.st[f.name].starred=true;
  });
  DB.wishlist = [];
  saveDB();
}
function saveDB(){localStorage.setItem('vault3',JSON.stringify(DB));}
function gst(n){if(!DB.st[n])DB.st[n]={};return DB.st[n];}
function esc(s){return(s+'').replace(/\\/g,'\\\\').replace(/'/g,"\\'").replace(/"/g,'&quot;');}
function today(){return new Date().toLocaleDateString('en-US',{year:'numeric',month:'short',day:'numeric'});}
function season(k){return{ss:"Spring · Summer",fw:"Fall · Winter",yr:"Year-round"}[k]||k;}

// ============================================================
// NAV
// ============================================================
function showPage(id,btn){
  document.querySelectorAll('.page').forEach(p=>p.classList.remove('active'));
  document.querySelectorAll('.nav-tab').forEach(t=>t.classList.remove('active'));
  document.getElementById('page-'+id).classList.add('active');
  if(btn)btn.classList.add('active');
  ({analytics:renderAnalytics,rotation:renderRotation,layering:renderLayering,classification:renderClassification,starred:renderStarred,weather:renderWeatherPage,insights:renderInsights,wishlist:renderWishlist,search:initSearch,importexport:renderImportExport,duaadvisor:initDuaAdvisor})[id]?.();
  if(id==='collection') buildMorningRec();
  updateStats();
}

// ============================================================
// GRID
// ============================================================
function filtered(){
  const q=document.getElementById('search').value.trim().toLowerCase();
  const fh=document.getElementById('fh').value,fs=document.getElementById('fs').value,
        fo=document.getElementById('fo').value,fd=document.getElementById('fd').value;
  return DB.col.filter(f=>{
    if(fh&&f.house!==fh)return false;
    if(fs&&f.s_key!==fs)return false;
    if(fo&&f.occ_key!==fo)return false;
    if(fd&&(gst(f.name).dna||'')!==fd)return false;
    if(q&&!(f.name+f.inspiration+f.house+f.occ_detail).toLowerCase().includes(q))return false;
    return true;
  });
}

function renderGrid(){
  const list=filtered();
  document.getElementById('grid-count').textContent=list.length+' fragrance'+(list.length!==1?'s':'');
  const g=document.getElementById('grid');
  if(!list.length){g.innerHTML='<div class="empty-st"><em>No results</em>Try a different filter</div>';return;}
  g.innerHTML=list.map(f=>{
    const st=gst(f.name),isS=st.starred||f.starred,dna=st.dna||'';
    const dcol=dna?DNA_FAMILIES[dna]?.color:'';
    const dtag=dna?`<span class="tag" style="border-color:${dcol}33;color:${dcol};font-size:6.5px;">${dna}</span>`:'';
    const btag=f.isBase?`<span class="tag tbase">BASE</span>`:'';
    return `<div class="card ${f.s_key}${isS?' starred':''}" onclick="openBottlePage('${esc(f.name)}')">
      <span class="card-star">★</span>
      <div class="card-house">${f.house}</div>
      <div class="card-name">${f.name}</div>
      <div class="card-insp">${f.inspiration}</div>
      <div class="card-tags"><span class="tag ${OCC_CLS[f.occ_key]}">${OCC_LBL[f.occ_key]}</span><span class="tag tsea">${season(f.s_key)}</span>${dtag}${btag}</div>
      <button class="card-del" onclick="event.stopPropagation();confirmDel('${esc(f.name)}')">✕</button>
    </div>`;
  }).join('');
}

function populateHouses(){
  const houses=[...new Set(DB.col.map(f=>f.house))].sort();
  const sel=document.getElementById('fh');
  sel.innerHTML='<option value="">All Houses</option>';
  houses.forEach(h=>{const o=document.createElement('option');o.value=h;o.textContent=h;sel.appendChild(o);});
  const dl=document.getElementById('house-dl');
  dl.innerHTML='';
  houses.forEach(h=>{const o=document.createElement('option');o.value=h;dl.appendChild(o);});
}

// ============================================================
// MODAL
// ============================================================
let CUR=null;

function openModal(name){
  const f=DB.col.find(x=>x.name===name);
  if(!f)return;
  CUR=name;
  const st=gst(name);
  document.getElementById('m-house').textContent=f.house;
  document.getElementById('m-name').textContent=f.name;
  document.getElementById('m-insp').textContent='← '+f.inspiration;
  document.getElementById('m-occ').textContent=f.occ_detail;
  document.getElementById('m-sea').textContent=season(f.s_key);
  document.getElementById('m-wears').textContent=(st.wears||[]).length||'—';
  document.getElementById('m-notes').value=st.notes||'';
  renderDNAGrid(st.dna||'');
  renderStarsEl(st.rating||0);
  renderLayerList();
  renderWearLog();
  const sb=document.getElementById('m-star-btn');
  const starred=st.starred||f.starred;
  sb.textContent=starred?'★ Starred':'☆ Star';
  sb.style.color=starred?'var(--gold)':'';
  renderStockBtn();
  document.getElementById('det-overlay').classList.remove('hidden');
  document.getElementById('m-layer-form').classList.add('hidden');
}

function renderDNAGrid(cur){
  document.getElementById('m-dna-grid').innerHTML=Object.keys(DNA_FAMILIES).map(fam=>{
    const col=DNA_FAMILIES[fam].color;
    const isSel=cur===fam;
    return `<div class="cpill${isSel?' sel':''}" style="${isSel?`border-color:${col};color:${col};background:${col}18;`:''}" onclick="setDNA('${esc(fam)}')">${fam}</div>`;
  }).join('');
}

function renderStarsEl(r){
  document.getElementById('m-stars').innerHTML=[1,2,3,4,5].map(i=>`<span class="star${r>=i?' lit':''}" onclick="setRating(${i})">★</span>`).join('');
}

function renderLayerList(){
  const st=gst(CUR);
  const personal=st.layers||[];
  const global=DB.layers.filter(c=>c.items.some(x=>x.toLowerCase()===CUR.toLowerCase()||x.toLowerCase().includes(CUR.toLowerCase())));
  let html='';
  if(global.length) html+=global.map(c=>`<div class="lc-row"><div style="flex:1"><div class="lc-names">${c.items.join(' + ')}</div><div class="lc-ratio">${c.ratio} · <span style="color:var(--gold-dim);">Global Combo</span></div><div class="lc-desc">${c.desc}</div></div></div>`).join('');
  if(personal.length) html+=personal.map((c,i)=>`<div class="lc-row"><div style="flex:1"><div class="lc-names">${c.items.join(' + ')}</div><div class="lc-ratio">${c.ratio} · <span style="color:var(--aqua);">Personal</span></div><div class="lc-desc">${c.desc}</div></div><button class="lc-del" onclick="delBottleLayer(${i})">✕</button></div>`).join('');
  if(!html) html='<div style="font-size:9.5px;color:var(--dove);padding:6px 0;font-style:italic;">No combos yet.</div>';
  document.getElementById('m-layer-list').innerHTML=html;
}

function renderWearLog(){
  const st=gst(CUR),wears=st.wears||[];
  const el=document.getElementById('m-wear-log');
  if(!wears.length){el.innerHTML='<div class="wear-entry"><span style="font-style:italic;color:var(--dove);">No wears logged yet.</span></div>';return;}
  el.innerHTML=[...wears].reverse().slice(0,8).map(d=>`<div class="wear-entry"><span class="wear-date">${d}</span><span style="font-size:7.5px;letter-spacing:.1em;color:var(--gold-dim);">WORN</span></div>`).join('');
}

function closeDetModal(e){if(e.target===document.getElementById('det-overlay'))closeDetDirect();}
function closeDetDirect(){document.getElementById('det-overlay').classList.add('hidden');CUR=null;renderGrid();updateStats();}










function toggleLayerForm(){document.getElementById('m-layer-form').classList.toggle('hidden');}

function saveBottleLayer(){
  const items=document.getElementById('lf-items').value.trim();
  const ratio=document.getElementById('lf-ratio').value.trim();
  const desc=document.getElementById('lf-desc').value.trim();
  if(!items)return;
  const st=gst(CUR);if(!st.layers)st.layers=[];
  const all=[CUR,...items.split(',').map(s=>s.trim()).filter(Boolean)];
  st.layers.push({items:all,ratio:ratio||'—',desc:desc||''});
  saveDB();
  ['lf-items','lf-ratio','lf-desc'].forEach(id=>document.getElementById(id).value='');
  document.getElementById('m-layer-form').classList.add('hidden');
  renderLayerList();
}

function delBottleLayer(idx){
  const st=gst(CUR);st.layers.splice(idx,1);saveDB();renderLayerList();
}

function deleteCurrentBottle(){
  if(!CUR)return;
  closeDetDirect();
  setTimeout(()=>confirmDel(CUR),60);
}

// ============================================================
// ADD / REMOVE
// ============================================================
function openAddModal(){
  document.getElementById('add-overlay').classList.remove('hidden');
  ['af-house','af-name','af-insp','af-occ-detail'].forEach(id=>document.getElementById(id).value='');
  document.getElementById('af-base').checked=false;
}
function closeAddOverlay(e){if(e.target===document.getElementById('add-overlay'))document.getElementById('add-overlay').classList.add('hidden');}

function addBottle(){
  const house=document.getElementById('af-house').value.trim();
  const name=document.getElementById('af-name').value.trim();
  const insp=document.getElementById('af-insp').value.trim()||'Original';
  const occ_key=document.getElementById('af-occ').value;
  const s_key=document.getElementById('af-sea').value;
  const dna=document.getElementById('af-dna').value;
  const isBase=document.getElementById('af-base').checked;
  const occ_detail=document.getElementById('af-occ-detail').value.trim()||'Casual / everyday';
  if(!house||!name){alert('House and name are required.');return;}
  if(DB.col.find(f=>f.name.toLowerCase()===name.toLowerCase())){alert('A bottle with this name already exists.');return;}
  DB.col.push({house,name,inspiration:insp,occ_key,occ_detail,s_key,isBase});
  if(dna)gst(name).dna=dna;
  saveDB();
  document.getElementById('add-overlay').classList.add('hidden');
  populateHouses();populateSugSelect();renderGrid();updateStats();
}

function confirmDel(name){
  document.getElementById('conf-msg').textContent=`Remove "${name}" from your vault? This cannot be undone.`;
  document.getElementById('conf-overlay').classList.remove('hidden');
  document.getElementById('conf-yes').onclick=()=>{
    DB.col=DB.col.filter(f=>f.name!==name);
    delete DB.st[name];
    saveDB();
    document.getElementById('conf-overlay').classList.add('hidden');
    populateHouses();populateSugSelect();renderGrid();updateStats();
    const active=document.querySelector('.page.active');
    if(active?.id==='page-starred')renderStarred();
  };
}

// ============================================================
// STATS
// ============================================================
function updateStats(){
  document.getElementById('s-total').textContent=DB.col.length;
  document.getElementById('s-houses').textContent=new Set(DB.col.map(f=>f.house)).size;
  document.getElementById('s-worn').textContent=Object.values(DB.st).reduce((s,st)=>s+(st.wears||[]).length,0);
  document.getElementById('s-starred').textContent=DB.col.filter(f=>gst(f.name).starred||f.starred).length;
}

// ============================================================
// DNA CLASSIFICATION
// ============================================================
let activeDNA=null;
function renderClassification(){
  const fams={};
  Object.keys(DNA_FAMILIES).forEach(f=>fams[f]=[]);fams['Unclassified']=[];
  DB.col.forEach(f=>{const d=gst(f.name).dna||'';(fams[d]||fams['Unclassified']).push(f);});
  const allF=[...Object.keys(DNA_FAMILIES),'Unclassified'];
  document.getElementById('dna-families').innerHTML=allF.map(fam=>{
    const items=fams[fam]||[];
    const col=DNA_FAMILIES[fam]?.color||'var(--dove)';
    const desc=DNA_FAMILIES[fam]?.desc||'';
    const preview=items.slice(0,4).map(f=>f.name).join(', ')+(items.length>4?` +${items.length-4} more`:'');
    return `<div class="dnaf" style="border-left:4px solid ${col};cursor:pointer;" onclick="toggleDNA('${esc(fam)}')">
      <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:6px;">
        <div class="dnaf-name" style="color:${col};">${fam}</div>
        <div style="font-size:20px;color:${col};opacity:.5;">›</div>
      </div>
      <div class="dnaf-ct">${items.length} bottle${items.length!==1?'s':''}</div>
      <div style="font-size:8px;color:var(--dove);margin-top:4px;line-height:1.5;">${desc}</div>
      ${items.length?`<div class="dnaf-list" style="margin-top:6px;border-top:1px solid rgba(140,100,40,.08);padding-top:6px;">${preview}</div>`:'<div style="font-size:8.5px;color:rgba(140,100,40,.3);margin-top:6px;font-style:italic;">None yet — classify your bottles</div>'}
    </div>`;
  }).join('');
  document.getElementById('dna-panel').classList.remove('open');
}

function toggleDNA(fam){
  activeDNA = fam;
  showDNAFull(fam);
}

function showDNAFull(fam) {
  // Build the family groups
  const fams = {};
  Object.keys(DNA_FAMILIES).forEach(f => fams[f] = []);
  fams['Unclassified'] = [];
  DB.col.forEach(f => {
    const d = gst(f.name).dna || '';
    (fams[d] || fams['Unclassified']).push(f);
  });

  const items = fams[fam] || [];
  const col = DNA_FAMILIES[fam]?.color || 'var(--dove)';
  const desc = DNA_FAMILIES[fam]?.desc || '';

  // Switch to bottle page style — reuse page-bottle area as a temporary DNA detail view
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));

  // Use a dedicated DNA detail page
  let detailPage = document.getElementById('page-dna-detail');
  if (!detailPage) {
    detailPage = document.createElement('div');
    detailPage.id = 'page-dna-detail';
    detailPage.className = 'page';
    document.querySelector('main').appendChild(detailPage);
  }
  detailPage.classList.add('active');

  detailPage.innerHTML = `
    <div style="display:flex;align-items:center;gap:14px;margin-bottom:20px;flex-wrap:wrap;">
      <button class="btn btn-muted" onclick="backToDNA()" style="font-size:8px;">&#8592; All Families</button>
      <div style="width:12px;height:12px;border-radius:50%;background:${col};flex-shrink:0;"></div>
      <div style="font-family:'Cormorant Garamond',serif;font-size:22px;color:${col};font-weight:600;">${fam}</div>
      <div style="font-size:8.5px;letter-spacing:.14em;text-transform:uppercase;color:var(--dove);margin-left:4px;">${items.length} bottle${items.length !== 1 ? 's' : ''}</div>
    </div>
    <div style="background:#ffffff;border:1px solid rgba(140,100,40,.1);border-left:4px solid ${col};padding:14px 18px;margin-bottom:16px;">
      <div style="font-size:10.5px;color:var(--cream);line-height:1.6;font-weight:400;">${desc}</div>
    </div>
    ${items.length === 0
      ? '<div class="empty-st"><em>No bottles yet</em>Open any bottle and set its DNA classification to add it here</div>'
      : '<div class="grid">' + items.map(f => {
          const st = gst(f.name);
          const isS = st.starred || f.starred;
          const fDNA = st.dna || DEFAULT_DNA[f.name] || '';
          const dnaCol = DNA_FAMILIES[fDNA]?.color || '';
          return '<div class="card ' + f.s_key + (isS ? ' starred' : '') + '" onclick="openBottlePage(\'' + esc(f.name) + '\')">' +
            '<span class="card-star">★</span>' +
            '<div class="card-house">' + f.house + '</div>' +
            '<div class="card-name">' + f.name + '</div>' +
            '<div class="card-insp">' + f.inspiration + '</div>' +
            '<div class="card-tags">' +
              '<span class="tag ' + OCC_CLS[f.occ_key] + '">' + OCC_LBL[f.occ_key] + '</span>' +
              '<span class="tag tsea">' + season(f.s_key) + '</span>' +
              (f.isBase ? '<span class="tag tbase">BASE</span>' : '') +
            '</div>' +
          '</div>';
        }).join('') + '</div>'
    }
  `;
}

function backToDNA() {
  activeDNA = null;
  showPage('classification', document.querySelector('.nav-tab[onclick*="classification"]'));
}

function showDNAPanel(fam, fams) {
  // Legacy — now handled by showDNAFull
}

// ============================================================
// LAYERING SUGGESTER
// ============================================================
let sugSpray = 2;

function renderSprayDots() {
  const max = 6;
  document.getElementById('spray-num').textContent = sugSpray;
  document.getElementById('spray-dots').innerHTML = Array.from({length: max}, (_,i) =>
    `<div class="spray-dot${i < sugSpray ? ' active' : ''}"></div>`
  ).join('');
}

function changeSpray(d) {
  sugSpray = Math.max(1, Math.min(6, sugSpray + d));
  renderSprayDots();
}

function populateSugSelect() {
  const sel = document.getElementById('sug-frag');
  const cur = sel.value;
  sel.innerHTML = '<option value="">Select a fragrance to layer\u2026</option>';
  [...DB.col].sort((a,b) => a.name.localeCompare(b.name)).forEach(f => {
    const o = document.createElement('option');
    o.value = f.name;
    o.textContent = f.name + ' \u2014 ' + f.house;
    sel.appendChild(o);
  });
  if(cur) sel.value = cur;
}

function runSuggester() {
  const fragName = document.getElementById('sug-frag').value;
  if (!fragName) { alert('Please select a fragrance first.'); return; }
  const frag = DB.col.find(f => f.name === fragName);
  if (!frag) return;

  const resultsEl = document.getElementById('sug-results');
  resultsEl.className = 'sug-results open';
  resultsEl.innerHTML = '<div class="sug-loading"><em>Analyzing your vault…</em></div>';

  setTimeout(() => {
    try {
      const suggestions = buildSuggestions(fragName, frag);
      renderSuggestions(suggestions, fragName, frag);
    } catch(e) {
      resultsEl.innerHTML = `<div class="sug-err"><strong>Error:</strong> ${e.message}</div>`;
    }
  }, 400);
}

// DNA pairing compatibility map — which families layer well together
const DNA_COMPAT = {
  "Aquatic / Marine":    ["Fougère","Woody / Aromatic","Citrus / Fresh","Musky / Skin","Chypre"],
  "Fougère":             ["Aquatic / Marine","Woody / Aromatic","Citrus / Fresh","Musky / Skin","Oriental / Amber"],
  "Woody / Aromatic":    ["Fougère","Aquatic / Marine","Oriental / Amber","Tobacco / Smoky","Musky / Skin"],
  "Oriental / Amber":    ["Gourmand","Woody / Aromatic","Tobacco / Smoky","Oud / Resinous","Floral"],
  "Oud / Resinous":      ["Oriental / Amber","Woody / Aromatic","Tobacco / Smoky","Floral","Musky / Skin"],
  "Citrus / Fresh":      ["Aquatic / Marine","Fougère","Musky / Skin","Floral","Chypre"],
  "Gourmand":            ["Oriental / Amber","Tobacco / Smoky","Woody / Aromatic","Musky / Skin","Floral"],
  "Floral":              ["Oriental / Amber","Citrus / Fresh","Musky / Skin","Oud / Resinous","Chypre"],
  "Chypre":              ["Floral","Citrus / Fresh","Woody / Aromatic","Aquatic / Marine","Musky / Skin"],
  "Tobacco / Smoky":     ["Oriental / Amber","Gourmand","Oud / Resinous","Woody / Aromatic","Musky / Skin"],
  "Musky / Skin":        ["Aquatic / Marine","Floral","Citrus / Fresh","Fougère","Gourmand"],
};

// Application order logic by DNA pairing
function getOrder(baseDNA, partnerDNA) {
  const heavy = ["Oud / Resinous","Oriental / Amber","Tobacco / Smoky","Gourmand","Woody / Aromatic"];
  const light  = ["Aquatic / Marine","Citrus / Fresh","Fougère","Musky / Skin","Floral"];
  const baseHeavy = heavy.includes(baseDNA);
  const partHeavy = heavy.includes(partnerDNA);
  if (baseHeavy && !partHeavy) return "Apply the partner first as a fresh top layer, then the base on pulse points.";
  if (!baseHeavy && partHeavy) return "Apply the base first to skin, then layer the partner on top for depth.";
  if (heavy.includes(partnerDNA)) return "Apply partner to wrists first, then base on chest and neck.";
  return "Apply base to skin first, then mist the partner lightly over the top.";
}

// Pairing notes by DNA combination
function getPairingNote(baseName, baseDNA, partnerName, partnerDNA, partnerInsp) {
  const pairs = {
    "Aquatic / Marine+Fougère": `The aquatic-fougère axis is a proven pairing — the marine freshness of ${baseName} opens up the lavender and herbal structure of ${partnerName}, creating an elevated beach-to-office signature with excellent longevity.`,
    "Aquatic / Marine+Woody / Aromatic": `${partnerName}'s woody base anchors the volatile marine top notes of ${baseName}, giving the combo far more staying power than either alone. The result is a refined aquatic with sandalwood depth.`,
    "Aquatic / Marine+Musky / Skin": `Layering ${partnerName}'s close skin musk under ${baseName} creates a skin-scent effect where the aquatic notes feel like they're emanating from the body itself — intimate and effortless.`,
    "Aquatic / Marine+Citrus / Fresh": `Both fragrances share a clean, transparent character — ${baseName} adds marine depth while ${partnerName} brings citrus brightness, compounding into a vivid, ultra-fresh signature.`,
    "Fougère+Aquatic / Marine": `The fougère backbone of ${baseName} gains luminous transparency when layered with ${partnerName}'s aquatic character, mimicking a luxury niche accord at a fraction of the cost.`,
    "Fougère+Woody / Aromatic": `${baseName}'s herbal-lavender structure sits perfectly on ${partnerName}'s woody base — coumarin and cedarwood are natural companions that deepen the fougère family.`,
    "Fougère+Oriental / Amber": `Adding ${partnerName}'s warm amber depth beneath ${baseName} transforms the classic fougère into an evening-ready accord — the aromatic herbs become richer and more animalic.`,
    "Woody / Aromatic+Fougère": `${partnerName} acts as a freshening agent on top of ${baseName}'s woody base — the lavender and oakmoss lift the heavier woods and extend the opening significantly.`,
    "Woody / Aromatic+Aquatic / Marine": `The woody backbone of ${baseName} gives ${partnerName}'s marine notes something solid to cling to — this is the classic structure of many designer aquatics, here assembled by hand.`,
    "Woody / Aromatic+Oriental / Amber": `${baseName} and ${partnerName} share a warm, resinous undercurrent — combined they create a rich, ambery wood accord with excellent projection and a long dry-down.`,
    "Woody / Aromatic+Musky / Skin": `${partnerName} softens the harder edges of ${baseName}, pulling the woody accord closer to skin and making it feel more personal — a superb office-to-evening transition.`,
    "Oriental / Amber+Gourmand": `Both ${baseName} and ${partnerName} occupy the warm-sweet spectrum — layered, they create an indulgent gourmand-oriental that's especially powerful in cold weather.`,
    "Oriental / Amber+Woody / Aromatic": `${partnerName}'s cedarwood and vetiver add a drying, angular counterpoint to ${baseName}'s sweetness, preventing it from reading as heavy while amplifying the sillage trail.`,
    "Oriental / Amber+Tobacco / Smoky": `The combination of ${baseName}'s amber warmth and ${partnerName}'s tobacco character creates a sophisticated, slow-burning evening accord reminiscent of a jazz club after midnight.`,
    "Oriental / Amber+Oud / Resinous": `${baseName} and ${partnerName} are natural companions in Middle Eastern perfumery — the amber sweetness lifts and softens the oud, creating a luxurious, long-lasting resinous accord.`,
    "Gourmand+Oriental / Amber": `${partnerName}'s amber structure gives ${baseName}'s sweet notes a sophisticated framework, elevating the gourmand from dessert to evening occasion.`,
    "Gourmand+Tobacco / Smoky": `${partnerName}'s tobacco smokiness adds a savory, mature counterpoint to ${baseName}'s sweetness — together they read as a dark, complex confection rather than simply sweet.`,
    "Gourmand+Woody / Aromatic": `The woody dryness of ${partnerName} tempers the sweetness of ${baseName}, creating a balanced gourmand-wood accord suitable from afternoon into evening.`,
    "Tobacco / Smoky+Oriental / Amber": `${baseName}'s tobacco character is amplified by ${partnerName}'s resinous warmth — a deeply satisfying, long-lasting evening combination.`,
    "Tobacco / Smoky+Gourmand": `${partnerName} wraps ${baseName}'s smoky character in sweetness, creating the olfactive equivalent of vanilla pipe tobacco — intimate and highly original.`,
    "Oud / Resinous+Oriental / Amber": `${partnerName}'s amber sweetness rounds out the rough edges of ${baseName}'s oud, creating a more approachable, wearable luxury accord without losing the depth.`,
    "Oud / Resinous+Floral": `A classic Middle Eastern pairing — ${partnerName}'s florals bloom over ${baseName}'s resinous base, creating an opulent, multi-dimensional accord.`,
    "Musky / Skin+Aquatic / Marine": `${partnerName} gives ${baseName}'s skin musk an airy, outdoors quality — the combination reads as effortlessly clean without being sterile.`,
    "Musky / Skin+Floral": `${baseName}'s soft musk backdrop amplifies ${partnerName}'s floral character, making the blooms feel more intimate and natural against skin.`,
    "Floral+Oriental / Amber": `${partnerName}'s warm amber elevates ${baseName}'s florals into evening-worthy territory — the sweetness deepens the petals and extends the sillage considerably.`,
    "Citrus / Fresh+Aquatic / Marine": `Both fragrances share transparent, luminous DNA — together they create a saturated, sparkling accord that's the olfactive equivalent of sunlight on water.`,
    "Citrus / Fresh+Fougère": `The citrus brightness of ${baseName} and the herbal freshness of ${partnerName} are natural allies — this combination is the backbone of countless classic barbershop and sport fragrances.`,
  };
  const key = baseDNA + '+' + partnerDNA;
  const reverseKey = partnerDNA + '+' + baseDNA;
  return pairs[key] || pairs[reverseKey] || 
    `${baseName} and ${partnerName} share complementary aromatic profiles — their combination creates an accord greater than either alone, with the ${baseDNA.toLowerCase()} character of the base harmonizing naturally with the ${partnerDNA.toLowerCase()} partner. The layering adds dimension and longevity, with the two fragrances blending at the skin level over the first hour of wear.`;
}

function getOccasionLabel(occ_key, season) {
  const map = {date:'Date Night', office:'Office / Day', evening:'Evening Out', casual:'Casual Wear', sport:'Active / Sport', special:'Special Occasion'};
  return map[occ_key] || 'Versatile';
}

// Weather state
let WEATHER = null;

// fetchWeather defined below with full weather page support

function getWeatherDesc(code) {
  if (code === 0) return {icon:'☀️', desc:'Clear'};
  if (code <= 2) return {icon:'⛅', desc:'Partly Cloudy'};
  if (code === 3) return {icon:'☁️', desc:'Overcast'};
  if (code <= 49) return {icon:'🌫️', desc:'Foggy'};
  if (code <= 57) return {icon:'🌧️', desc:'Drizzle'};
  if (code <= 67) return {icon:'🌧️', desc:'Rain'};
  if (code <= 77) return {icon:'❄️', desc:'Snow'};
  if (code <= 82) return {icon:'🌦️', desc:'Showers'};
  if (code <= 99) return {icon:'⛈️', desc:'Thunderstorm'};
  return {icon:'🌡️', desc:'Mixed'};
}

function getWeatherScentNote(temp, humid, code) {
  const rain = code >= 50;
  const cold = temp < 45;
  const cool = temp >= 45 && temp < 62;
  const warm = temp >= 62 && temp < 78;
  const hot  = temp >= 78;
  const highHumid = humid > 65;

  if (cold) return {label:'Heavy Sillage Day', color:'#c9a84c', tip:'Cold air suppresses projection — go heavier, more sprays, richer DNA families.'};
  if (cool && rain) return {label:'Cozy Indoor Mood', color:'#8a6e2e', tip:'Rain + cool temps call for warm gourmand and woody combos that bloom indoors.'};
  if (cool) return {label:'Transitional Weather', color:'#3d6038', tip:'Cool and crisp — fougères and woody aromatics shine. Good layering day.'};
  if (warm && highHumid) return {label:'High Humidity — Go Light', color:'#3a7585', tip:'Humidity amplifies sillage — use fewer sprays and lean toward aquatics or citrus.'};
  if (warm) return {label:'Perfect Layering Conditions', color:'#3d6038', tip:'Ideal temp for layering — skin warmth activates both fragrances evenly.'};
  if (hot && highHumid) return {label:'Beast Mode Warning', color:'#b05a42', tip:'Heat and humidity = heavy projection. 1-2 sprays max. Aquatics and citrus only.'};
  if (hot) return {label:'Light Touch Day', color:'#3a7585', tip:'Heat amplifies everything — go fresh, aquatic, and light. Skip heavy orientals.'};
  if (rain) return {label:'Rain Amplifies Sillage', color:'#507050', tip:'Moisture in air boosts projection significantly — reduce spray count by 1.'};
  return {label:'Good Conditions', color:'#6b6358', tip:'Moderate conditions — standard spray counts apply.'};
}

function getWeatherSeasonKey(temp) {
  if (temp < 55) return 'fw';
  if (temp > 72) return 'ss';
  return 'yr';
}

function buildSuggestions(fragName, frag) {
  const baseDNA = gst(fragName).dna || DEFAULT_DNA[fragName] || '';
  const compat = DNA_COMPAT[baseDNA] || Object.keys(DNA_FAMILIES);

  // Occasion + label setup
  const occFilter = document.getElementById('sug-occ')?.value || '';
  const occLabels = {date:'Date Night',office:'Office / Day',evening:'Evening Out',casual:'Casual Wear',sport:'Active / Sport',special:'Special Occasion'};

  // Weather-preferred DNA families
  const temp = WEATHER?.temp;
  let weatherFavored = [];
  let weatherPenalized = [];
  if (temp !== undefined) {
    if (temp < 45) { weatherFavored = ["Oud / Resinous","Oriental / Amber","Tobacco / Smoky","Gourmand","Woody / Aromatic"]; weatherPenalized = ["Aquatic / Marine","Citrus / Fresh"]; }
    else if (temp < 62) { weatherFavored = ["Woody / Aromatic","Fougère","Oriental / Amber","Gourmand"]; weatherPenalized = []; }
    else if (temp < 75) { weatherFavored = ["Fougère","Aquatic / Marine","Woody / Aromatic","Citrus / Fresh","Musky / Skin"]; weatherPenalized = ["Oud / Resinous","Tobacco / Smoky"]; }
    else { weatherFavored = ["Aquatic / Marine","Citrus / Fresh","Musky / Skin","Fougère"]; weatherPenalized = ["Oud / Resinous","Oriental / Amber","Tobacco / Smoky","Gourmand"]; }
  }

  // Weather-preferred season
  const wxSeason = temp !== undefined ? getWeatherSeasonKey(temp) : null;

  const scored = DB.col
    .filter(f => f.name !== fragName)
    .map(f => {
      const fDNA = gst(f.name).dna || DEFAULT_DNA[f.name] || '';
      let score = 0;
      const compatIdx = compat.indexOf(fDNA);
      if (fDNA === baseDNA) score += 3;
      else if (compatIdx === 0) score += 10;
      else if (compatIdx === 1) score += 8;
      else if (compatIdx === 2) score += 6;
      else if (compatIdx >= 3) score += 4;
      if (f.isBase) score += 4;
      if (f.s_key === frag.s_key) score += 2;
      if (f.occ_key === frag.occ_key) score += 1;
      // Occasion filter bonus — strongly favor matching occasion
      if (occFilter && f.occ_key === occFilter) score += 8;
      if (occFilter && f.occ_key !== occFilter && occFilter !== '') score -= 3;
      // Weather scoring
      if (weatherFavored.includes(fDNA)) score += 6;
      if (weatherPenalized.includes(fDNA)) score -= 5;
      if (wxSeason && f.s_key === wxSeason) score += 3;
      score += Math.random() * 2;
      return {f, fDNA, score};
    })
    .sort((a, b) => b.score - a.score);

  const seen = new Set();
  seen.add(baseDNA);
  const picks = [];
  for (const s of scored) {
    if (picks.length >= 4) break;
    if (!seen.has(s.fDNA)) { seen.add(s.fDNA); picks.push(s); }
  }
  for (const s of scored) {
    if (picks.length >= 4) break;
    if (!picks.includes(s)) picks.push(s);
  }

  const heavyDNA = ["Oud / Resinous","Oriental / Amber","Tobacco / Smoky","Gourmand"];
  // Adjust spray count for weather: hot = fewer, cold = more
  function partnerSprays(dna) {
    let base = heavyDNA.includes(dna) ? Math.max(1, sugSpray - 1) : Math.min(4, sugSpray + 1);
    if (temp !== undefined) {
      if (temp > 78) base = Math.max(1, base - 1);
      if (temp < 45) base = Math.min(5, base + 1);
    }
    return base;
  }

  const occasions = ['Date Night','Office / Day','Evening Out','Weekend Casual'];

  return picks.slice(0,4).map((s, i) => ({
    partner: s.f.name,
    partnerSprays: partnerSprays(s.fDNA),
    order: getOrder(baseDNA, s.fDNA),
    occasion: occFilter ? (occLabels[occFilter] || occasions[i]) : (occasions[i] || getOccasionLabel(s.f.occ_key, s.f.s_key)),
    note: getPairingNote(fragName, baseDNA, s.f.name, s.fDNA, s.f.inspiration),
    partnerDNA: s.fDNA,
  }));
}

function renderSuggestions(suggestions, fragName, frag) {
  const resultsEl = document.getElementById('sug-results');
  const dna = gst(fragName).dna || DEFAULT_DNA[fragName] || '';
  const dnaCol = dna ? (DNA_FAMILIES[dna]?.color||'var(--gold)') : 'var(--gold)';

  const dots = (n,col) => Array.from({length:Math.min(n,6)},()=>`<span style="display:inline-block;width:6px;height:6px;border-radius:50%;background:${col};margin-right:2px;opacity:.85;"></span>`).join('');
  const labels = ['I','II','III','IV'];

  const cards = suggestions.map((s,i) => {
    const pDNA = gst(s.partner).dna || DEFAULT_DNA[s.partner] || '';
    const pCol = pDNA ? (DNA_FAMILIES[pDNA]?.color||'var(--dove)') : 'var(--dove)';
    return `<div class="sug-card" style="border-color:${pCol}55;">
      <div class="sug-card-title" style="color:${pCol};">Pairing ${labels[i]} &mdash; ${s.occasion}</div>
      <div class="sug-combo-row">
        <span class="sug-frag">${fragName}</span>
        <span class="sug-sprays" style="border-color:${dnaCol}44;color:${dnaCol};">${sugSpray} spray${sugSpray!==1?'s':''}&nbsp;${dots(sugSpray,dnaCol)}</span>
      </div>
      <div class="sug-combo-row">
        <span class="sug-plus">+</span>
        <span class="sug-frag">${s.partner}</span>
        <span class="sug-sprays" style="border-color:${pCol}44;color:${pCol};">${s.partnerSprays} spray${s.partnerSprays!==1?'s':''}&nbsp;${dots(s.partnerSprays,pCol)}</span>
      </div>
      ${pDNA?`<div style="font-size:7px;letter-spacing:.13em;text-transform:uppercase;color:${pCol};margin:5px 0 3px;opacity:.75;">Partner DNA: ${pDNA}</div>`:''}
      <div class="sug-note">${s.note}</div>
      <div class="sug-occasion" style="margin-top:7px;font-style:italic;">${s.order}</div>
      <button class="btn btn-muted" style="margin-top:11px;font-size:7px;padding:4px 10px;" onclick="saveSugCombo('${esc(fragName)}',${sugSpray},'${esc(s.partner)}',${s.partnerSprays},'${esc(s.note)}','${esc(s.occasion)}',this)">Save to Vault</button>
    </div>`;
  }).join('');

  resultsEl.innerHTML = `<div class="sug-chosen" style="margin-top:4px;">
    <span class="sug-chosen-name">${fragName}</span>
    <span class="sug-arrow">&rarr;</span>
    <span class="sug-chosen-spray">${sugSpray} spray${sugSpray!==1?'s':''} &nbsp;&middot;&nbsp; ${suggestions.length} pairings found</span>
  </div><div class="sug-cards">${cards}</div>`;
}

function saveSugCombo(base, bSprays, partner, pSprays, note, occasion, btn) {
  DB.layers.push({id:uid(),items:[base,partner],ratio:`${bSprays} + ${pSprays} sprays`,desc:`${occasion} — ${note}`});
  saveDB();
  renderLayering();
  btn.textContent='Saved \u2713';
  btn.style.color='var(--forest)';
  btn.style.borderColor='var(--forest)';
  setTimeout(()=>{btn.textContent='Save to Vault';btn.style.color='';btn.style.borderColor='';},2200);
}

// ============================================================
// LAYERING LAB
// ============================================================
function renderLayering(){
  const personal=[];
  Object.entries(DB.st).forEach(([name,st])=>(st.layers||[]).forEach(c=>personal.push({...c,_from:name})));
  const all=[...DB.layers,...personal];
  document.getElementById('lab-ct').textContent=all.length+' combo'+(all.length!==1?'s':'');
  const bases=DB.col.filter(f=>f.isBase);
  const baseSection=`<div class="lcard" style="grid-column:1/-1;border:1px solid rgba(201,168,76,.13);">
    <div class="atitle">Layering Bases — Your Anchor Fragrances</div>
    <div style="display:flex;flex-wrap:wrap;gap:7px;">${bases.map(f=>`<div style="padding:5px 11px;border:1px solid rgba(201,168,76,.2);font-family:'Cormorant Garamond',serif;font-size:13px;color:var(--cream);">${f.name} <span style="font-size:7.5px;color:var(--gold-dim);">${f.house.replace('The ','')}</span></div>`).join('')}</div>
  </div>`;
  const comboHtml=all.map(c=>`<div class="lcard">
    <div class="atitle">${c._from?'Personal Combo':'Established Combo'}</div>
    <div class="lcomb">${c.items.map((it,i)=>`<span class="litem">${it}</span>${i<c.items.length-1?'<span class="lplus">+</span>':''}`).join('')}<span class="lratio">${c.ratio}</span></div>
    <div class="ldesc">${c.desc}</div>
    ${!c._from?`<button class="btn btn-danger" style="margin-top:9px;font-size:7px;padding:4px 10px;" onclick="delGlobalLayer('${esc(c.id)}')">Remove</button>`:''}
  </div>`).join('');
  document.getElementById('lab-grid').innerHTML=baseSection+comboHtml;
}

function toggleGLForm(){document.getElementById('gl-form').classList.toggle('hidden');}

function saveGlobalLayer(){
  const items=document.getElementById('gl-items').value.trim();
  const ratio=document.getElementById('gl-ratio').value.trim();
  const desc=document.getElementById('gl-desc').value.trim();
  if(!items)return;
  DB.layers.push({id:uid(),items:items.split(',').map(s=>s.trim()).filter(Boolean),ratio:ratio||'—',desc:desc||''});
  saveDB();
  ['gl-items','gl-ratio','gl-desc'].forEach(id=>document.getElementById(id).value='');
  document.getElementById('gl-form').classList.add('hidden');
  renderLayering();
}

function delGlobalLayer(id){DB.layers=DB.layers.filter(c=>c.id!==id);saveDB();renderLayering();}

// ============================================================
// ANALYTICS
// ============================================================
function renderAnalytics(){
  const houses={};DB.col.forEach(f=>houses[f.house]=(houses[f.house]||0)+1);
  const hS=Object.entries(houses).sort((a,b)=>b[1]-a[1]);const mH=hS[0]?.[1]||1;
  document.getElementById('ch-houses').innerHTML=hS.map(([h,n])=>`<div class="br"><div class="blbl" title="${h}">${h}</div><div class="btrack"><div class="bfill" style="width:${(n/mH*100).toFixed(1)}%"></div></div><div class="bnum">${n}</div></div>`).join('');

  const sea={'Spring · Summer':0,'Fall · Winter':0,'Year-round':0};
  DB.col.forEach(f=>{const s=season(f.s_key);sea[s]=(sea[s]||0)+1;});
  const sCols=['#3a7585','#c9a84c','#6b6358'];const sKeys=Object.keys(sea);const tot=DB.col.length;
  let off=25;
  document.getElementById('donut-s').innerHTML=`<circle cx="18" cy="18" r="15.9" fill="transparent" stroke="rgba(201,168,76,.07)" stroke-width="3.5"/>` +
    sKeys.map((k,i)=>{const p=sea[k]/tot*100;const path=`<circle cx="18" cy="18" r="15.9" fill="transparent" stroke="${sCols[i]}" stroke-width="3.5" stroke-dasharray="${p} ${100-p}" stroke-dashoffset="${-off}"/>`;off-=p;return path;}).join('');
  document.getElementById('legend-s').innerHTML=sKeys.map((k,i)=>`<div class="li"><div class="ldot" style="background:${sCols[i]}"></div>${k} · ${sea[k]}</div>`).join('');

  const occs={date:0,office:0,evening:0,casual:0,sport:0,special:0};
  DB.col.forEach(f=>occs[f.occ_key]=(occs[f.occ_key]||0)+1);
  const mO=Math.max(...Object.values(occs));
  document.getElementById('ch-occ').innerHTML=Object.entries(occs).sort((a,b)=>b[1]-a[1]).map(([k,n])=>`<div class="br"><div class="blbl">${OCC_LBL[k]}</div><div class="btrack"><div class="bfill" style="width:${(n/mO*100).toFixed(1)}%"></div></div><div class="bnum">${n}</div></div>`).join('');

  const dnaC={};DB.col.forEach(f=>{const d=gst(f.name).dna||'Unclassified';dnaC[d]=(dnaC[d]||0)+1;});
  const dS=Object.entries(dnaC).sort((a,b)=>b[1]-a[1]);const mD=dS[0]?.[1]||1;
  document.getElementById('ch-dna').innerHTML=dS.map(([k,n])=>{const col=DNA_FAMILIES[k]?.color||'var(--dove)';return`<div class="br"><div class="blbl" title="${k}">${k}</div><div class="btrack"><div class="bfill" style="width:${(n/mD*100).toFixed(1)}%;background:linear-gradient(90deg,${col}77,${col})"></div></div><div class="bnum">${n}</div></div>`;}).join('');

  const wears=Object.values(DB.st).reduce((s,st)=>s+(st.wears||[]).length,0);
  const starred=DB.col.filter(f=>gst(f.name).starred||f.starred).length;
  document.getElementById('a-total').textContent=DB.col.length;
  document.getElementById('a-overview').innerHTML=`${new Set(DB.col.map(f=>f.house)).size} houses represented<br>${DB.col.filter(f=>f.isBase).length} layering bases<br>${starred} starred bottles<br>${wears} total wears logged<br>${DB.layers.length} global layering combos`;

  const insp={};DB.col.forEach(f=>{const k=f.inspiration.split(' + ')[0].split(' /')[0].trim();if(k!=='Original')insp[k]=(insp[k]||0)+1;});
  const iS=Object.entries(insp).sort((a,b)=>b[1]-a[1]).slice(0,8);const mI=iS[0]?.[1]||1;
  document.getElementById('ch-insp').innerHTML=iS.map(([k,n])=>`<div class="br"><div class="blbl" title="${k}">${k}</div><div class="btrack"><div class="bfill" style="width:${(n/mI*100).toFixed(1)}%"></div></div><div class="bnum">${n}</div></div>`).join('');
}

// ============================================================
// ROTATION
// ============================================================
function renderRotation(){
  const now=new Date();
  const items=DB.col.map(f=>{const st=gst(f.name);const ws=st.wears||[];const last=ws.length?new Date(ws[ws.length-1]):null;const days=last?Math.floor((now-last)/86400000):9999;return{f,days,last};}).sort((a,b)=>b.days-a.days);
  document.getElementById('rot-list').innerHTML=items.map((it,i)=>{
    const{f,days,last}=it;
    const cls=days===9999?'n':days>30?'s':days>14?'w':'f';
    const label=days===9999?'—':days+'d';
    const ls=last?last.toLocaleDateString('en-US',{month:'short',day:'numeric',year:'numeric'}):'Never worn';
    return`<div class="ritem" onclick="openBottlePage('${esc(f.name)}')"><div class="rrank">${i+1}</div><div style="flex:1"><div class="rname">${f.name}</div><div class="rmeta">${f.house} · ${season(f.s_key)}</div></div><div style="text-align:right"><span class="rdays ${cls}">${label}</span><div style="font-size:8.5px;color:var(--dove);">${ls}</div></div></div>`;
  }).join('');
}

// ============================================================
// STARRED
// ============================================================
function renderStarred(){
  const list=DB.col.filter(f=>gst(f.name).starred||f.starred);
  document.getElementById('starred-ct').textContent=list.length+' bottle'+(list.length!==1?'s':'');
  const g=document.getElementById('starred-grid');
  if(!list.length){g.innerHTML='<div class="empty-st"><em>None starred yet</em>Open any bottle and tap ☆ Star</div>';return;}
  g.innerHTML=list.map(f=>`<div class="card ${f.s_key} starred" onclick="openBottlePage('${esc(f.name)}')"><span class="card-star">★</span><div class="card-house">${f.house}</div><div class="card-name">${f.name}</div><div class="card-insp">${f.inspiration}</div><div class="card-tags"><span class="tag ${OCC_CLS[f.occ_key]}">${OCC_LBL[f.occ_key]}</span><span class="tag tsea">${season(f.s_key)}</span></div></div>`).join('');
}

// ============================================================
// WEATHER PAGE
// ============================================================
function renderWeatherPage() {
  // If weather already loaded, render immediately; otherwise wait
  if (WEATHER) {
    renderWxContent();
  } else {
    // fetchWeather will render when done
    fetchWeather(true);
  }
}

// Override fetchWeather to optionally render weather page after
async function fetchWeather(renderPage) {
  const bar = document.getElementById('weather-bar');
  try {
    const res = await fetch('https://api.open-meteo.com/v1/forecast?latitude=38.8799&longitude=-77.1068&current=temperature_2m,weathercode,relative_humidity_2m,windspeed_10m,apparent_temperature&daily=temperature_2m_max,temperature_2m_min,weathercode,precipitation_probability_max&temperature_unit=fahrenheit&windspeed_unit=mph&forecast_days=1&timezone=America/New_York');
    const data = await res.json();
    const c = data.current;
    const d = data.daily;
    const temp = Math.round(c.temperature_2m);
    const feels = Math.round(c.apparent_temperature);
    const humid = c.relative_humidity_2m;
    const wind = Math.round(c.windspeed_10m);
    const code = c.weathercode;
    const hi = Math.round(d.temperature_2m_max[0]);
    const lo = Math.round(d.temperature_2m_min[0]);
    const precip = d.precipitation_probability_max[0];

    const wx = getWeatherDesc(code);
    WEATHER = {temp, feels, humid, wind, code, hi, lo, precip, ...wx};

    const scentNote = getWeatherScentNote(temp, humid, code);

    // Update mini weather bar in layering tab
    if(bar) bar.innerHTML = `
      <span class="weather-icon">${wx.icon}</span>
      <div class="weather-info">
        <span class="weather-temp">${temp}°F</span>
        <span class="weather-desc">${wx.desc} &middot; ${humid}% humidity &middot; ${wind} mph</span>
        <div class="weather-note">${scentNote.tip}</div>
      </div>
      <span class="weather-badge" style="border-color:${scentNote.color};color:${scentNote.color};">${scentNote.label}</span>
    `;

    if(renderPage) renderWxContent();
  } catch(e) {
    if(bar) bar.innerHTML = '<span style="font-size:9px;color:var(--dove);">Weather unavailable</span>';
  }
}

function renderWxContent() {
  if (!WEATHER) return;
  const {temp, feels, humid, wind, code, hi, lo, precip, icon, desc} = WEATHER;
  const scentNote = getWeatherScentNote(temp, humid, code);

  document.getElementById('wx-loading').style.display = 'none';
  document.getElementById('wx-content').style.display = 'block';
  document.getElementById('wx-icon-big').textContent = icon;
  document.getElementById('wx-temp-big').textContent = temp + '°F';
  document.getElementById('wx-desc-big').textContent = desc;
  document.getElementById('wx-meta').innerHTML = `Feels like ${feels}° &middot; Hi ${hi}° / Lo ${lo}° &middot; ${humid}% humidity &middot; ${wind} mph wind &middot; ${precip}% chance of rain`;
  document.getElementById('wx-badge-wrap').innerHTML = `<span style="display:inline-block;padding:6px 14px;border:1px solid ${scentNote.color};color:${scentNote.color};font-size:8px;letter-spacing:.16em;text-transform:uppercase;">${scentNote.label}</span>`;
  document.getElementById('wx-scent-tip').textContent = scentNote.tip;

  // Spray recommendation
  let sprays, sprayNote;
  if (temp > 85) { sprays = '1 – 2'; sprayNote = 'Heat amplifies heavily — go minimal'; }
  else if (temp > 75 && humid > 65) { sprays = '2'; sprayNote = 'Humidity boosts sillage significantly'; }
  else if (temp > 72) { sprays = '2 – 3'; sprayNote = 'Ideal projection conditions'; }
  else if (temp > 55) { sprays = '3 – 4'; sprayNote = 'Good conditions — standard application'; }
  else if (temp > 40) { sprays = '4 – 5'; sprayNote = 'Cool air dampens projection — layer up'; }
  else { sprays = '5 – 6'; sprayNote = 'Cold suppresses scent — apply generously'; }
  document.getElementById('wx-sprays').textContent = sprays;
  document.getElementById('wx-spray-note').textContent = sprayNote;

  // DNA best/avoid
  let best = [], avoid = [];
  if (temp < 45) { best = ['Oud / Resinous','Oriental / Amber','Tobacco / Smoky','Gourmand']; avoid = ['Aquatic / Marine','Citrus / Fresh']; }
  else if (temp < 62) { best = ['Woody / Aromatic','Fougère','Oriental / Amber','Gourmand']; avoid = ['Oud / Resinous']; }
  else if (temp < 75) { best = ['Fougère','Aquatic / Marine','Woody / Aromatic','Citrus / Fresh']; avoid = ['Oud / Resinous','Tobacco / Smoky']; }
  else { best = ['Aquatic / Marine','Citrus / Fresh','Musky / Skin','Fougère']; avoid = ['Oud / Resinous','Oriental / Amber','Tobacco / Smoky','Gourmand']; }

  document.getElementById('wx-dna-best').innerHTML = best.map(d => {
    const col = DNA_FAMILIES[d]?.color || 'var(--gold)';
    return `<span style="color:${col};">✓ ${d}</span>`;
  }).join('<br>');
  document.getElementById('wx-dna-avoid').innerHTML = avoid.length ? avoid.map(d => `<span>✕ ${d}</span>`).join('<br>') : '<span style="color:var(--forest);">All families work today</span>';

  document.getElementById('wx-feels').innerHTML = `
    Humidity: ${humid}%<br>
    Wind: ${wind} mph<br>
    Rain chance: ${precip}%<br>
    ${humid > 65 ? '<span style="color:var(--rose);">High humidity — reduce sprays</span>' : precip > 50 ? '<span style="color:var(--aqua);">Rain likely — sillage boosted</span>' : '<span style="color:var(--forest);">Good wear conditions</span>'}
  `;

  // Render today's picks
  renderWxPicks(best);
  showWxOcc('date', document.querySelector('.wx-occ-btn.active'));
}

function scoreBottleForWeather(f) {
  if (!WEATHER) return 0;
  const {temp, humid, code} = WEATHER;
  const fDNA = gst(f.name).dna || DEFAULT_DNA[f.name] || '';
  let score = 0;

  // Temperature-based DNA scoring
  if (temp < 45) {
    if (['Oud / Resinous','Oriental / Amber','Tobacco / Smoky','Gourmand'].includes(fDNA)) score += 10;
    if (['Aquatic / Marine','Citrus / Fresh'].includes(fDNA)) score -= 6;
    if (f.s_key === 'fw') score += 4;
  } else if (temp < 62) {
    if (['Woody / Aromatic','Fougère','Oriental / Amber'].includes(fDNA)) score += 8;
    if (f.s_key === 'fw' || f.s_key === 'yr') score += 3;
  } else if (temp < 75) {
    if (['Fougère','Aquatic / Marine','Woody / Aromatic','Citrus / Fresh','Musky / Skin'].includes(fDNA)) score += 8;
    if (f.s_key === 'ss' || f.s_key === 'yr') score += 3;
  } else {
    if (['Aquatic / Marine','Citrus / Fresh','Musky / Skin','Fougère'].includes(fDNA)) score += 10;
    if (['Oud / Resinous','Oriental / Amber','Tobacco / Smoky','Gourmand'].includes(fDNA)) score -= 6;
    if (f.s_key === 'ss') score += 4;
  }
  // Humidity penalty for heavy sillage
  if (humid > 70 && ['Oud / Resinous','Oriental / Amber','Gourmand'].includes(fDNA)) score -= 3;
  // Rain bonus for aquatics
  if (code >= 50 && ['Aquatic / Marine','Fougère'].includes(fDNA)) score += 3;
  // Starred bonus
  if (gst(f.name).starred || f.starred) score += 2;
  score += Math.random() * 1.5;
  return score;
}

function renderWxPicks(bestDNA) {
  const scored = DB.col.map(f => ({f, score: scoreBottleForWeather(f)})).sort((a,b) => b.score - a.score);
  const picks = scored.slice(0, 12).map(s => s.f);
  document.getElementById('wx-picks-meta').textContent = picks.length + ' top picks for today';
  document.getElementById('wx-picks-grid').innerHTML = picks.map(f => cardHTML(f)).join('');
}

function showWxOcc(occ, btn) {
  document.querySelectorAll('.wx-occ-btn').forEach(b => b.classList.remove('active'));
  if(btn) btn.classList.add('active');
  const scored = DB.col
    .filter(f => f.occ_key === occ)
    .map(f => ({f, score: scoreBottleForWeather(f)}))
    .sort((a,b) => b.score - a.score);
  const picks = scored.slice(0, 8).map(s => s.f);
  document.getElementById('wx-occ-grid').innerHTML = picks.length
    ? picks.map(f => cardHTML(f)).join('')
    : '<div class="empty-st"><em>No bottles found</em>for this occasion</div>';
}

function cardHTML(f) {
  const st = gst(f.name), isS = st.starred || f.starred, dna = st.dna || DEFAULT_DNA[f.name] || '';
  const dcol = dna ? DNA_FAMILIES[dna]?.color : '';
  const dtag = dna ? `<span class="tag" style="border-color:${dcol}33;color:${dcol};font-size:6.5px;">${dna}</span>` : '';
  const btag = f.isBase ? `<span class="tag tbase">BASE</span>` : '';
  return `<div class="card ${f.s_key}${isS?' starred':''}" onclick="openBottlePage('${esc(f.name)}')">
    <span class="card-star">★</span>
    <div class="card-house">${f.house}</div>
    <div class="card-name">${f.name}</div>
    <div class="card-insp">${f.inspiration}</div>
    <div class="card-tags"><span class="tag ${OCC_CLS[f.occ_key]}">${OCC_LBL[f.occ_key]}</span><span class="tag tsea">${season(f.s_key)}</span>${dtag}${btag}</div>
  </div>`;
}

// ============================================================
// STOCK CYCLING  (OK → Low → Empty → OK)
// ============================================================
// cycleStock defined below


function renderStockBtn() {
  if (!CUR) return;
  const st = gst(CUR);
  const labels = {'ok':'&#9646; Stock OK','low':'&#9888; Running Low','empty':'&#10006; Empty / Gone'};
  const colors = {'ok':'var(--forest)','low':'var(--rose)','empty':'#999'};
  const s = st.stock || 'ok';
  const btn = document.getElementById('m-stock-btn');
  if (btn) { btn.innerHTML = labels[s]; btn.style.color = colors[s]; btn.style.borderColor = colors[s]; }
}

// ============================================================
// QUICK LOG
// ============================================================
let qlOpen = false;

function toggleQL() {
  qlOpen = !qlOpen;
  const panel = document.getElementById('ql-panel');
  panel.classList.toggle('open', qlOpen);
  if (qlOpen) {
    filterQL('');
    setTimeout(() => document.getElementById('ql-search').focus(), 100);
  }
}

function filterQL(q) {
  const list = document.getElementById('ql-list');
  const matches = DB.col.filter(f => !q || f.name.toLowerCase().includes(q.toLowerCase()) || f.house.toLowerCase().includes(q.toLowerCase())).slice(0, 12);
  list.innerHTML = matches.map(f => `
    <div class="ql-item" onclick="quickLogWear('${esc(f.name)}')">
      <div class="ql-item-house">${f.house}</div>
      <div>${f.name}</div>
    </div>`).join('');
}

function quickLogWear(name) {
  const st = gst(name);
  if (!st.wears) st.wears = [];
  st.wears.push(today());
  saveDB();
  updateStats();
  toggleQL();
  // Flash confirmation
  const btn = document.querySelector('.ql-btn');
  btn.textContent = '✓';
  btn.style.background = 'var(--forest)';
  setTimeout(() => { btn.textContent = '✎'; btn.style.background = 'var(--gold)'; }, 1500);
}

// ============================================================
// WISHLIST
// ============================================================
function addWishlistItem() {
  const name = document.getElementById('wl-name').value.trim();
  const house = document.getElementById('wl-house').value.trim();
  const type = document.getElementById('wl-type').value;
  const note = document.getElementById('wl-note').value.trim();
  if (!name) { alert('Please enter a fragrance name.'); return; }
  if (!DB.wishlist) DB.wishlist = [];
  DB.wishlist.push({ id: uid(), name, house, type, note, added: today() });
  saveDB();
  ['wl-name','wl-house','wl-note'].forEach(id => document.getElementById(id).value = '');
  renderWishlist();
}

function deleteWishlistItem(id) {
  DB.wishlist = (DB.wishlist || []).filter(w => w.id !== id);
  saveDB();
  renderWishlist();
}

function renderWishlist() {
  const items = DB.wishlist || [];
  const typeConfig = {
    want: { label: '★ Want to Buy', color: 'var(--gold)' },
    destash: { label: '✕ Destash', color: 'var(--rose)' },
    decant: { label: '◎ Want Decant', color: 'var(--aqua)' },
    low: { label: '⚠ Running Low', color: '#b07020' },
  };
  const grid = document.getElementById('wl-grid');
  if (!items.length) {
    grid.innerHTML = '<div class="empty-st"><em>Nothing here yet</em>Add bottles you want, need to destash, or are running low on</div>';
    return;
  }
  // Group by type
  const groups = { want: [], destash: [], decant: [], low: [] };
  items.forEach(w => (groups[w.type] || groups.want).push(w));
  grid.innerHTML = Object.entries(groups).flatMap(([type, list]) =>
    list.map(w => {
      const cfg = typeConfig[type] || typeConfig.want;
      return `<div class="wl-card">
        <span class="wl-badge" style="border-color:${cfg.color};color:${cfg.color};">${cfg.label}</span>
        <div class="wl-name">${w.name}</div>
        <div class="wl-house">${w.house || 'Unknown House'}</div>
        ${w.note ? `<div class="wl-note">${w.note}</div>` : ''}
        <div style="font-size:8px;color:var(--dove);margin-top:6px;font-weight:500;">Added ${w.added}</div>
        <button class="wl-del" onclick="deleteWishlistItem('${w.id}')">✕</button>
      </div>`;
    })
  ).join('');
}

// ============================================================
// INSIGHTS
// ============================================================
function buildGapHTML(gaps, sparse, dnaCount, allFams) {
  let html = '';
  if (gaps.length > 0) {
    html += '<div style="font-size:9px;color:var(--dove);margin-bottom:8px;font-weight:500;">Missing families:</div>';
    html += gaps.map(f => {
      const col2 = DNA_FAMILIES[f]?.color || 'var(--dove)';
      return '<span class="gap-pill" style="border-color:' + col2 + ';color:' + col2 + ';">' + f + '</span>';
    }).join('');
  }
  if (sparse.length > 0) {
    html += '<div style="font-size:9px;color:var(--dove);margin:10px 0 8px;font-weight:500;">Underrepresented (1-2 bottles):</div>';
    html += sparse.map(f => {
      const col2 = DNA_FAMILIES[f]?.color || 'var(--dove)';
      return '<span class="gap-pill" style="border-color:' + col2 + '55;color:' + col2 + ';">' + f + ' (' + (dnaCount[f]||0) + ')</span>';
    }).join('');
  }
  const top3 = allFams.sort((a,b) => (dnaCount[b]||0) - (dnaCount[a]||0)).slice(0,3).map(f => f + ' (' + (dnaCount[f]||0) + ')').join(', ');
  html += '<div style="margin-top:12px;font-size:9px;color:var(--dove);line-height:1.7;font-weight:500;">Your heaviest: ' + top3 + '</div>';
  return html;
}

function renderInsights() {
  const grid = document.getElementById('ins-grid');
  const allSt = DB.st;
  const col = DB.col;

  // Top 10 rated
  const rated = col.map(f => ({ f, r: gst(f.name).rating || 0 })).filter(x => x.r > 0).sort((a,b) => b.r - a.r).slice(0, 10);

  // Most worn
  const worn = col.map(f => ({ f, w: (gst(f.name).wears||[]).length })).sort((a,b) => b.w - a.w).slice(0, 10);

  // Never worn
  const neverWorn = col.filter(f => !(gst(f.name).wears||[]).length);

  // Season alerts — it's spring, flag unplayed SS bottles
  const month = new Date().getMonth();
  const isSS = month >= 2 && month <= 8;
  const seasonKey = isSS ? 'ss' : 'fw';
  const seasonName = isSS ? 'Spring · Summer' : 'Fall · Winter';
  const seasonUnworn = col.filter(f => f.s_key === seasonKey && !(gst(f.name).wears||[]).length);

  // Redundancy — group by inspiration base
  const inspGroups = {};
  col.forEach(f => {
    const base = f.inspiration.split('×')[0].split('+')[0].split('x ')[0].trim();
    if (!inspGroups[base]) inspGroups[base] = [];
    inspGroups[base].push(f);
  });
  const redundant = Object.entries(inspGroups).filter(([k,v]) => v.length >= 3).sort((a,b) => b[1].length - a[1].length).slice(0, 6);

  // DNA gaps
  const dnaCount = {};
  col.forEach(f => { const d = gst(f.name).dna || DEFAULT_DNA[f.name] || ''; dnaCount[d] = (dnaCount[d]||0)+1; });
  const allFams = Object.keys(DNA_FAMILIES);
  const gaps = allFams.filter(f => (dnaCount[f]||0) === 0);
  const sparse = allFams.filter(f => (dnaCount[f]||0) >= 1 && (dnaCount[f]||0) <= 2);

  // Value estimate (rough: avg $45 per bottle for your collection mix)
  const avgPrice = 42;
  const totalValue = col.length * avgPrice;
  const retailValue = col.length * 95; // if bought designer

  // Stock alerts
  const lowStock = col.filter(f => gst(f.name).stock === 'low');
  const emptyStock = col.filter(f => gst(f.name).stock === 'empty');

  // Destash candidates from wishlist
  const destashList = (DB.wishlist||[]).filter(w => w.type === 'destash');

  // Build wear calendar for this month
  const now = new Date();
  const calHTML = buildCalendar(now.getFullYear(), now.getMonth());

  grid.innerHTML = `
    <!-- Streak + morning stats -->
    <div class="ins-card" style="grid-column:1/-1;display:grid;grid-template-columns:repeat(auto-fit,minmax(160px,1fr));gap:1px;background:rgba(140,100,40,.1);padding:0;">
      <div style="background:#ffffff;padding:20px 22px;">
        <div class="ins-card-title">&#128293; Current Streak</div>
        <div class="streak-num" id="ins-streak">0</div>
        <div class="ins-sub">consecutive days logged</div>
      </div>
      <div style="background:#ffffff;padding:20px 22px;">
        <div class="ins-card-title">&#128293; Longest Streak</div>
        <div class="streak-num" id="ins-best-streak">0</div>
        <div class="ins-sub">best streak ever</div>
      </div>
      <div style="background:#ffffff;padding:20px 22px;">
        <div class="ins-card-title">&#128200; Cost Per Wear</div>
        <div id="ins-best-cpw" style="font-family:'Cormorant Garamond',serif;font-size:28px;color:var(--gold);font-weight:600;"></div>
        <div class="ins-sub" id="ins-best-cpw-name"></div>
      </div>
      <div style="background:#ffffff;padding:20px 22px;">
        <div class="ins-card-title">&#128200; Worst Cost Per Wear</div>
        <div id="ins-worst-cpw" style="font-family:'Cormorant Garamond',serif;font-size:28px;color:var(--rose);font-weight:600;"></div>
        <div class="ins-sub" id="ins-worst-cpw-name"></div>
      </div>
    </div>

    <!-- Stats overview -->
    <div class="ins-card" style="grid-column:1/-1">
      <div class="ins-card-title">Collection Overview</div>
      <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:1px;background:rgba(140,100,40,.1);">
        ${[
          ['164', 'Bottles'],
          [new Set(col.map(f=>f.house)).size, 'Houses'],
          [Object.values(allSt).reduce((s,st)=>s+(st.wears||[]).length,0), 'Total Wears'],
          [rated.length, 'Rated'],
          [neverWorn.length, 'Never Worn'],
          [col.filter(f=>f.isBase).length, 'Layering Bases'],
        ].map(([n,l]) => `<div style="background:#ffffff;padding:14px 16px;"><div class="ins-big">${n}</div><div class="ins-sub">${l}</div></div>`).join('')}
      </div>
      <div style="margin-top:14px;display:flex;align-items:center;gap:10px;flex-wrap:wrap;">
        <span style="font-size:9px;color:var(--dove);font-weight:500;">Estimated collection value:</span>
        <span style="font-family:'Cormorant Garamond',serif;font-size:20px;color:var(--gold);font-weight:600;">~$${totalValue.toLocaleString()}</span>
        <span style="font-size:8.5px;color:var(--dove);">paid · ~$${retailValue.toLocaleString()} retail equivalent</span>
      </div>
    </div>

    <!-- Season alerts -->
    <div class="ins-card">
      <div class="ins-card-title">&#9888; ${seasonName} Alerts</div>
      ${seasonUnworn.length === 0
        ? '<div style="font-size:10px;color:var(--forest);font-weight:500;">&#10003; All seasonal bottles worn this season!</div>'
        : `<div style="font-size:10px;color:var(--rose);font-weight:600);margin-bottom:10px;">${seasonUnworn.length} ${seasonName} bottles not yet worn this season</div>
          ${seasonUnworn.slice(0,6).map(f=>`<div class="ins-list-item"><div class="ins-list-name">${f.name}</div><div class="ins-list-meta">${f.house.replace('The ','')}</div></div>`).join('')}
          ${seasonUnworn.length > 6 ? `<div style="font-size:8.5px;color:var(--dove);margin-top:6px;">+${seasonUnworn.length-6} more</div>` : ''}`
      }
    </div>

    <!-- Stock alerts -->
    <div class="ins-card">
      <div class="ins-card-title">&#9646; Stock Status</div>
      ${emptyStock.length === 0 && lowStock.length === 0
        ? '<div style="font-size:10px;color:var(--forest);font-weight:500;">&#10003; No stock issues flagged. Open any bottle and tap the stock button to track levels.</div>'
        : [...emptyStock.map(f=>`<div class="ins-list-item"><span style="color:#999;font-size:8px;font-weight:700;margin-right:8px;">EMPTY</span><div class="ins-list-name">${f.name}</div></div>`),
           ...lowStock.map(f=>`<div class="ins-list-item"><span style="color:var(--rose);font-size:8px;font-weight:700;margin-right:8px;">LOW</span><div class="ins-list-name">${f.name}</div></div>`)].join('')
      }
      <div style="margin-top:10px;font-size:8.5px;color:var(--dove);">Open any bottle modal → tap stock button to flag low or empty</div>
    </div>

    <!-- Wear calendar -->
    <div class="ins-card">
      <div class="ins-card-title">&#128197; Wear Calendar — ${now.toLocaleString('default',{month:'long',year:'numeric'})}</div>
      ${calHTML}
    </div>

    <!-- Top rated -->
    <div class="ins-card">
      <div class="ins-card-title">&#11088; Your Top Rated</div>
      ${rated.length === 0
        ? '<div style="font-size:10px;color:var(--dove);">No ratings yet — open any bottle and tap the stars.</div>'
        : rated.map((x,i) => `<div class="ins-list-item"><div class="ins-list-rank">${i+1}</div><div class="ins-list-name">${x.f.name}<div style="font-size:8px;color:var(--dove);">${x.f.house.replace('The ','')}</div></div><div class="ins-list-meta">${'★'.repeat(x.r)}${'☆'.repeat(5-x.r)}</div></div>`).join('')
      }
    </div>

    <!-- Most worn -->
    <div class="ins-card">
      <div class="ins-card-title">&#128138; Most Worn</div>
      ${worn.filter(x=>x.w>0).length === 0
        ? '<div style="font-size:10px;color:var(--dove);">No wears logged yet — use the ✎ button to quickly log wears.</div>'
        : worn.filter(x=>x.w>0).map((x,i) => `<div class="ins-list-item"><div class="ins-list-rank">${i+1}</div><div class="ins-list-name">${x.f.name}<div style="font-size:8px;color:var(--dove);">${x.f.house.replace('The ','')}</div></div><div class="ins-list-meta">${x.w} wear${x.w!==1?'s':''}</div></div>`).join('')
      }
    </div>

    <!-- Never worn -->
    <div class="ins-card">
      <div class="ins-card-title">&#128065; Dust Collectors — Never Worn</div>
      <div style="font-size:10px;color:var(--rose);font-weight:600;margin-bottom:10px;">${neverWorn.length} bottles never worn</div>
      ${neverWorn.slice(0,8).map(f=>`<div class="ins-list-item"><div class="ins-list-name">${f.name}</div><div class="ins-list-meta">${f.house.replace('The ','')}</div></div>`).join('')}
      ${neverWorn.length > 8 ? `<div style="font-size:8.5px;color:var(--dove);margin-top:6px;">+${neverWorn.length-8} more</div>` : ''}
    </div>

    <!-- Redundancy detector -->
    <div class="ins-card">
      <div class="ins-card-title">&#9888; Redundancy Clusters</div>
      <div style="font-size:9px;color:var(--dove);margin-bottom:12px;font-weight:500;">Bottles sharing the same inspiration DNA</div>
      ${redundant.map(([insp, bottles]) => `
        <div class="redundancy-item">
          <div class="redundancy-insp">${insp} (${bottles.length})</div>
          <div class="redundancy-bottles">${bottles.map(f=>f.name).join(', ')}</div>
        </div>`).join('')}
    </div>

    <!-- DNA gaps -->
    <div class="ins-card">
      <div class="ins-card-title">&#9675; DNA Gap Analysis</div>
      <div id="ins-dna-gap-content"></div>
    </div>

        <!-- Destash list from wishlist -->
    <div class="ins-card">
      <div class="ins-card-title">&#10060; Destash List</div>
      ${destashList.length === 0
        ? '<div style="font-size:10px;color:var(--dove);">Nothing flagged for destash. Go to Wishlist tab to add.</div>'
        : destashList.map(w=>`<div class="ins-list-item"><div class="ins-list-name">${w.name}<div style="font-size:8px;color:var(--dove);">${w.house}</div></div>${w.note?`<div class="ins-list-meta" style="max-width:120px;white-space:normal;text-align:right;">${w.note}</div>`:''}</div>`).join('')
      }
    </div>
  `;
}

function buildCalendar(year, month) {
  const now = new Date();
  const firstDay = new Date(year, month, 1).getDay();
  const daysInMonth = new Date(year, month+1, 0).getDate();

  // Collect all wear dates this month
  const wearDates = new Set();
  const wearMap = {}; // date → bottle names
  Object.entries(DB.st).forEach(([name, st]) => {
    (st.wears||[]).forEach(d => {
      const dt = new Date(d);
      if (dt.getFullYear() === year && dt.getMonth() === month) {
        const day = dt.getDate();
        wearDates.add(day);
        if (!wearMap[day]) wearMap[day] = [];
        wearMap[day].push(name);
      }
    });
  });

  const days = ['S','M','T','W','T','F','S'];
  let html = '<div style="display:grid;grid-template-columns:repeat(7,1fr);gap:2px;margin-bottom:8px;">';
  html += days.map(d=>`<div style="font-size:7.5px;letter-spacing:.1em;text-transform:uppercase;color:var(--gold);text-align:center;padding:3px 0;font-weight:700;">${d}</div>`).join('');
  html += '</div><div style="display:grid;grid-template-columns:repeat(7,1fr);gap:2px;">';

  for (let i = 0; i < firstDay; i++) html += '<div></div>';
  for (let d = 1; d <= daysInMonth; d++) {
    const isToday = d === now.getDate() && year === now.getFullYear() && month === now.getMonth();
    const hasWear = wearDates.has(d);
    const title = wearMap[d]?.join(', ') || '';
    html += `<div title="${title}" style="aspect-ratio:1;display:flex;align-items:center;justify-content:center;font-size:9.5px;font-weight:600;border-radius:2px;cursor:default;
      background:${hasWear?'var(--gold)':'var(--ash)'};
      color:${hasWear?'#fff':'var(--dove)'};
      border:${isToday?'2px solid var(--gold-dim)':'none'};
      opacity:${hasWear||isToday?1:0.6};">${d}</div>`;
  }
  html += '</div>';
  if (wearDates.size === 0) html += '<div style="font-size:9px;color:var(--dove);margin-top:8px;">No wears logged this month. Use the ✎ button to log.</div>';
  return html;
}

// ============================================================
// BOTTLE PROFILE PAGE
// ============================================================
let prevPage = 'collection';

function openBottlePage(name) {
  const f = DB.col.find(x => x.name === name);
  if (!f) return;
  CUR = name;
  const st = gst(name);

  // Track which page we came from
  const active = document.querySelector('.page.active');
  prevPage = active ? active.id.replace('page-','') : 'collection';

  // Switch to bottle page
  document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.nav-tab').forEach(t => t.classList.remove('active'));
  document.getElementById('page-bottle').classList.add('active');

  // Breadcrumb
  document.getElementById('bp-breadcrumb').textContent = f.house + ' / ' + f.name;

  // Header
  document.getElementById('bp-house').textContent = f.house;
  document.getElementById('bp-name').textContent = f.name;
  document.getElementById('bp-insp').textContent = '← ' + f.inspiration;

  // Tags
  const dna = st.dna || DEFAULT_DNA[f.name] || '';
  const dnaCol = dna ? (DNA_FAMILIES[dna]?.color || 'var(--gold)') : 'var(--gold)';
  document.getElementById('bp-tags').innerHTML = `
    <span class="tag ${OCC_CLS[f.occ_key]}">${OCC_LBL[f.occ_key]}</span>
    <span class="tag tsea">${season(f.s_key)}</span>
    ${dna ? '<span class="tag" style="border-color:' + dnaCol + '44;color:' + dnaCol + ';font-size:7px;">' + dna + '</span>' : ''}
    ${f.isBase ? '<span class="tag tbase">LAYERING BASE</span>' : ''}
  `;

  // Stats
  const wears = st.wears || [];
  document.getElementById('bp-wears').textContent = wears.length || '0';
  const lastWorn = wears.length ? wears[wears.length-1] : null;
  document.getElementById('bp-lastworn').textContent = lastWorn || 'Never worn';

  // Stars
  const r = st.rating || 0;
  document.getElementById('bp-stars').innerHTML = [1,2,3,4,5].map(i =>
    '<span class="star' + (r>=i?' lit':'') + '" onclick="setRating(' + i + ')">★</span>'
  ).join('');

  // DNA label + grid
  document.getElementById('bp-dna-label').textContent = dna || 'Unclassified';
  document.getElementById('bp-dna-label').style.color = dnaCol;
  document.getElementById('bp-dna-grid').innerHTML = Object.keys(DNA_FAMILIES).map(fam => {
    const col = DNA_FAMILIES[fam].color;
    const isSel = dna === fam;
    const selStyle2 = isSel ? 'border-color:'+col+';color:'+col+';background:'+col+'18;' : ''; const selCls2 = isSel ? ' sel' : ''; return '<div class="cpill'+selCls2+'" style="'+selStyle2+'" onclick="setDNA(\'' + esc(fam) + '\')">'+fam+'</div>';
  }).join('');

  // Notes
  document.getElementById('bp-notes').value = st.notes || '';

  // Star + stock buttons
  const starred = st.starred || f.starred;
  const sb = document.getElementById('bp-star-btn');
  sb.textContent = starred ? '★ Starred' : '☆ Star';
  sb.style.color = starred ? 'var(--gold)' : '';
  renderBPStockBtn();

  // Wear calendar (current month for this bottle)
  renderBPCalendar(name);

  // Wear log
  renderBPWearLog(name);

  // Layering combos — reuse existing IDs but point to bp-layer-list
  CUR = name;
  renderBPLayerList();

  // Similar bottles
  renderSimilar(f, dna);

  // New features
  renderCustomTags();
  renderBottlePhoto();
  renderCPW();

  // Pre-fill value input
  const valInp = document.getElementById('bp-value');
  if (valInp) valInp.value = st.value || '';

  // Clear SOTD
  const sotd = document.getElementById('sotd-preview');
  if (sotd) sotd.innerHTML = '';
}

function closeBottlePage() {
  CUR = null;
  showPage(prevPage, null);
  // Re-highlight correct nav tab
  const tabs = document.querySelectorAll('.nav-tab');
  tabs.forEach(t => {
    if (t.getAttribute('onclick') && t.getAttribute('onclick').includes("'" + prevPage + "'")) {
      t.classList.add('active');
    }
  });
}

function renderBPStockBtn() {
  const st = gst(CUR);
  const labels = {ok:'&#9646; Stock OK', low:'&#9888; Running Low', empty:'&#10006; Empty'};
  const colors = {ok:'var(--forest)', low:'var(--rose)', empty:'#999'};
  const s = st.stock || 'ok';
  const btn = document.getElementById('bp-stock-btn');
  if (btn) { btn.innerHTML = labels[s]; btn.style.color = colors[s]; btn.style.borderColor = colors[s]; }
  // Also update modal stock btn if visible
  const mb = document.getElementById('m-stock-btn');
  if (mb) { mb.innerHTML = labels[s]; mb.style.color = colors[s]; mb.style.borderColor = colors[s]; }
}

// Override cycleStock to update bp stock btn too
function cycleStock() {
  if (!CUR) return;
  const st = gst(CUR);
  const states = ['ok','low','empty'];
  const labels = {ok:'&#9646; Stock OK', low:'&#9888; Running Low', empty:'&#10006; Empty'};
  const colors = {ok:'var(--forest)', low:'var(--rose)', empty:'#999'};
  const cur = st.stock || 'ok';
  const next = states[(states.indexOf(cur) + 1) % states.length];
  st.stock = next;
  saveDB();
  renderBPStockBtn();
}

// Override toggleStar to update bp star btn
function toggleStar() {
  if (!CUR) return;
  const st = gst(CUR);
  st.starred = !st.starred;
  saveDB();
  const sb = document.getElementById('bp-star-btn') || document.getElementById('m-star-btn');
  if (sb) { sb.textContent = st.starred ? '★ Starred' : '☆ Star'; sb.style.color = st.starred ? 'var(--gold)' : ''; }
  updateStats();
}

// Override logWear to refresh bp page
function logWear() {
  if (!CUR) return;
  const st = gst(CUR);
  if (!st.wears) st.wears = [];
  st.wears.push(today());
  saveDB();
  document.getElementById('bp-wears').textContent = st.wears.length;
  renderBPCalendar(CUR);
  renderBPWearLog(CUR);
  updateStats();
}

// Override saveNotes to work with bp-notes
function saveNotes() {
  if (!CUR) return;
  const n1 = document.getElementById('m-notes');
  const n2 = document.getElementById('bp-notes');
  gst(CUR).notes = (n2 && n2.style.display!=='none' ? n2 : n1)?.value || '';
  saveDB();
}

// Override setDNA to update bp page
function setDNA(fam) {
  if (!CUR) return;
  gst(CUR).dna = fam;
  saveDB();
  // Update both grids
  ['m-dna-grid','bp-dna-grid'].forEach(id => {
    const el = document.getElementById(id);
    if (!el) return;
    el.innerHTML = Object.keys(DNA_FAMILIES).map(f2 => {
      const col = DNA_FAMILIES[f2].color;
      const isSel = fam === f2;
      const _sc = isSel?' sel':''; const _ss = isSel?'border-color:'+col+';color:'+col+';background:'+col+'18;':''; return '<div class="cpill'+_sc+'" style="'+_ss+'" onclick="setDNA(\'' + esc(f2) + '\')">' + f2 + '</div>';
    }).join('');
  });
  const dnaLabel = document.getElementById('bp-dna-label');
  if (dnaLabel) { dnaLabel.textContent = fam; dnaLabel.style.color = DNA_FAMILIES[fam]?.color || 'var(--gold)'; }
}

// Override setRating for bp page
function setRating(r) {
  if (!CUR) return;
  gst(CUR).rating = r;
  saveDB();
  ['m-stars','bp-stars'].forEach(function(id) {
    const el = document.getElementById(id);
    if (!el) return;
    let html = '';
    for (let i=1;i<=5;i++) {
      html += '<span class="star' + (r>=i?' lit':'') + '" onclick="setRating(' + i + ')">&#9733;</span>';
    }
    el.innerHTML = html;
  });
}

function renderBPCalendar(name) {
  const st = gst(name);
  const wears = st.wears || [];
  const now = new Date();
  const year = now.getFullYear(), month = now.getMonth();
  const firstDay = new Date(year, month, 1).getDay();
  const daysInMonth = new Date(year, month+1, 0).getDate();

  // Which days this bottle was worn this month
  const wornDays = new Set();
  wears.forEach(d => {
    const dt = new Date(d);
    if (dt.getFullYear()===year && dt.getMonth()===month) wornDays.add(dt.getDate());
  });

  const dayNames = ['S','M','T','W','T','F','S'];
  let html = '<div style="display:grid;grid-template-columns:repeat(7,1fr);gap:2px;margin-bottom:6px;">';
  html += dayNames.map(d => '<div style="font-size:7px;letter-spacing:.1em;text-transform:uppercase;color:var(--gold);text-align:center;font-weight:700;">' + d + '</div>').join('');
  html += '</div><div style="display:grid;grid-template-columns:repeat(7,1fr);gap:2px;">';
  for (let i=0;i<firstDay;i++) html += '<div></div>';
  for (let d=1;d<=daysInMonth;d++) {
    const isToday = d===now.getDate();
    const worn = wornDays.has(d);
    html += '<div style="aspect-ratio:1;display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:600;border-radius:2px;background:' + (worn?'var(--gold)':'var(--ash)') + ';color:' + (worn?'#fff':'var(--dove)') + ';border:' + (isToday?'2px solid var(--gold-dim)':'none') + ';opacity:' + (worn||isToday?1:0.55) + ';">' + d + '</div>';
  }
  html += '</div>';
  if (wornDays.size === 0) html += '<div style="font-size:9px;color:var(--dove);margin-top:8px;">Not worn this month yet.</div>';

  const el = document.getElementById('bp-calendar');
  if (el) el.innerHTML = '<div style="font-size:8px;letter-spacing:.14em;color:var(--dove);margin-bottom:8px;font-weight:600;">' + now.toLocaleString('default',{month:'long',year:'numeric'}) + '</div>' + html;
}

function renderBPWearLog(name) {
  const st = gst(name);
  const wears = st.wears || [];
  const el = document.getElementById('bp-wear-log');
  if (!el) return;
  if (!wears.length) { el.innerHTML = '<div style="font-size:9.5px;color:var(--dove);font-style:italic;">No wears logged yet.</div>'; return; }
  el.innerHTML = '<div style="font-size:8px;letter-spacing:.14em;color:var(--dove);margin-bottom:8px;font-weight:600;">ALL WEARS (' + wears.length + ')</div>' +
    [...wears].reverse().map(d =>
      '<div class="bp-wear-entry"><span class="bp-wear-date">' + d + '</span><span style="font-size:7.5px;color:var(--gold);letter-spacing:.1em;">WORN</span></div>'
    ).join('');
}

function renderBPLayerList() {
  const st = gst(CUR);
  const personal = st.layers || [];
  const global = DB.layers.filter(c => c.items.some(x => x.toLowerCase() === CUR.toLowerCase() || x.toLowerCase().includes(CUR.toLowerCase())));
  let html = '';
  if (global.length) html += global.map(c => '<div class="lc-row"><div style="flex:1"><div class="lc-names">' + c.items.join(' + ') + '</div><div class="lc-ratio">' + c.ratio + ' · <span style="color:var(--gold-dim);">Global Combo</span></div><div class="lc-desc">' + c.desc + '</div></div></div>').join('');
  if (personal.length) html += personal.map((c,i) => '<div class="lc-row"><div style="flex:1"><div class="lc-names">' + c.items.join(' + ') + '</div><div class="lc-ratio">' + c.ratio + ' · <span style="color:var(--aqua);">Personal</span></div><div class="lc-desc">' + c.desc + '</div></div><button class="lc-del" onclick="delBottleLayer(' + i + ')">✕</button></div>').join('');
  if (!html) html = '<div style="font-size:9.5px;color:var(--dove);font-style:italic;">No combos yet. Add one above.</div>';
  const el = document.getElementById('bp-layer-list');
  if (el) el.innerHTML = html;
  // Also sync old modal layer list if exists
  const oldEl = document.getElementById('m-layer-list');
  if (oldEl) oldEl.innerHTML = html;
}

function renderSimilar(frag, dna) {
  const similar = DB.col.filter(f => {
    if (f.name === frag.name) return false;
    const fDNA = gst(f.name).dna || DEFAULT_DNA[f.name] || '';
    return fDNA === dna || f.occ_key === frag.occ_key || f.s_key === frag.s_key;
  }).slice(0, 6);
  const el = document.getElementById('bp-similar');
  if (!el) return;
  el.innerHTML = similar.map(f => cardHTML(f)).join('');
}

// ============================================================
// SEARCH
// ============================================================
function initSearch() {
  const input = document.getElementById('srch-input');
  if (input) { input.focus(); runSearch(input.value || ''); }
}

function runSearch(q) {
  const meta = document.getElementById('srch-meta');
  const grid = document.getElementById('srch-grid');
  const query = (q || '').trim().toLowerCase();

  if (!query) {
    meta.textContent = 'Type to search all 164 bottles by name, house, inspiration, DNA or occasion';
    grid.innerHTML = '';
    return;
  }

  const results = DB.col.filter(f => {
    const dna = (gst(f.name).dna || DEFAULT_DNA[f.name] || '').toLowerCase();
    return (
      f.name.toLowerCase().includes(query) ||
      f.house.toLowerCase().includes(query) ||
      f.inspiration.toLowerCase().includes(query) ||
      f.occ_detail.toLowerCase().includes(query) ||
      dna.includes(query) ||
      season(f.s_key).toLowerCase().includes(query)
    );
  });

  meta.textContent = results.length + ' result' + (results.length !== 1 ? 's' : '') + ' for "' + q + '"';
  grid.innerHTML = results.length
    ? results.map(f => cardHTML(f)).join('')
    : '<div class="empty-st"><em>No results</em>Try a different term</div>';
}

// ============================================================
// ============================================================
// SORT + CUSTOM TAGS FILTER
// ============================================================
function populateTagFilter() {
  const allTags = new Set();
  Object.values(DB.st).forEach(st => (st.customTags||[]).forEach(t => allTags.add(t)));
  const sel = document.getElementById('ftag');
  if (!sel) return;
  const cur = sel.value;
  sel.innerHTML = '<option value="">All Tags</option>';
  [...allTags].sort().forEach(t => {
    const o = document.createElement('option');
    o.value = t; o.textContent = t; sel.appendChild(o);
  });
  if (cur) sel.value = cur;
}

// ============================================================
// MORNING RECOMMENDATION
// ============================================================
let morningPickName = null;
let morningPickIdx = 0;

function buildMorningRec() {
  const rec = document.getElementById('morning-rec');
  if (!rec) return;
  const month = new Date().getMonth();
  const isSS = month >= 2 && month <= 8;
  const wxSeason = isSS ? 'ss' : 'fw';
  const temp = WEATHER ? WEATHER.temp : null;

  let weatherFavored = [];
  if (temp !== null) {
    if (temp < 45) weatherFavored = ["Oud / Resinous","Oriental / Amber","Tobacco / Smoky","Gourmand","Woody / Aromatic"];
    else if (temp < 62) weatherFavored = ["Woody / Aromatic","Fougère","Oriental / Amber","Gourmand"];
    else if (temp < 75) weatherFavored = ["Fougère","Aquatic / Marine","Woody / Aromatic","Citrus / Fresh","Musky / Skin"];
    else weatherFavored = ["Aquatic / Marine","Citrus / Fresh","Musky / Skin","Fougère"];
  }

  const now = new Date();
  const todayStr = now.toLocaleDateString('en-US',{year:'numeric',month:'short',day:'numeric'});

  const scored = DB.col.map(f => {
    const st = gst(f.name);
    const dna = st.dna || DEFAULT_DNA[f.name] || '';
    let score = 0;
    // Not worn today already
    if ((st.wears||[]).includes(todayStr)) return {f, score: -99};
    // Season match
    if (f.s_key === wxSeason || f.s_key === 'yr') score += 5;
    // Weather DNA match
    if (weatherFavored.includes(dna)) score += 8;
    // Hasn't been worn recently
    const lastWorn = (st.wears||[]).length ? new Date((st.wears||[])[st.wears.length-1]) : null;
    const daysSince = lastWorn ? Math.floor((now-lastWorn)/86400000) : 999;
    if (daysSince > 14) score += 4;
    if (daysSince > 30) score += 3;
    // Rating bonus
    if (st.rating >= 4) score += 3;
    if (st.rating >= 5) score += 2;
    // Randomness
    score += Math.random() * 3;
    return {f, score, dna};
  }).filter(x => x.score > -99).sort((a,b) => b.score - a.score);

  if (!scored.length) return;

  const pick = scored[morningPickIdx % scored.length];
  morningPickName = pick.f.name;
  const f = pick.f;
  const st = gst(f.name);
  const wears = (st.wears||[]).length;

  document.getElementById('mr-house').textContent = f.house;
  document.getElementById('mr-name').textContent = f.name;

  let reason = '';
  if (WEATHER) {
    const sn = getWeatherScentNote(WEATHER.temp, WEATHER.humid, WEATHER.code);
    reason = sn.label + ' today — ' + f.name + ' is ideal for these conditions. ';
  }
  if (wears === 0) reason += 'Never worn — time to give it a try.';
  else {
    const lastWorn = st.wears[st.wears.length-1];
    reason += 'Last worn ' + lastWorn + '.';
  }
  document.getElementById('mr-reason').textContent = reason;

  // Spray count
  let sprays = 3;
  if (WEATHER) {
    if (WEATHER.temp > 80) sprays = 2;
    else if (WEATHER.temp < 45) sprays = 5;
  }
  document.getElementById('mr-sprays').textContent = sprays;

  // Weather badge
  if (WEATHER) {
    const sn = getWeatherScentNote(WEATHER.temp, WEATHER.humid, WEATHER.code);
    document.getElementById('mr-weather-badge').innerHTML = '<span style="font-size:7.5px;letter-spacing:.14em;text-transform:uppercase;padding:2px 8px;border:1px solid '+sn.color+';color:'+sn.color+';">'+sn.label+'</span>';
  }

  rec.style.display = 'block';
}

function refreshMorningRec() {
  morningPickIdx++;
  buildMorningRec();
}

function logMorningWear() {
  if (!morningPickName) return;
  const st = gst(morningPickName);
  if (!st.wears) st.wears = [];
  st.wears.push(today());
  saveDB();
  updateStats();
  const btn = document.querySelector('#morning-rec .btn-gold');
  if (btn) { btn.textContent = '✓ Logged!'; btn.style.color='var(--forest)'; }
}

// ============================================================
// CUSTOM TAGS
// ============================================================
function renderCustomTags() {
  if (!CUR) return;
  const st = gst(CUR);
  const tags = st.customTags || [];
  const el = document.getElementById('bp-custom-tags');
  if (!el) return;
  el.innerHTML = tags.map((t,i) =>
    '<span class="ctag">' + t + '<button class="ctag-del" onclick="removeCustomTag('+i+')">✕</button></span>'
  ).join('') || '<span style="font-size:9px;color:var(--dove);">No tags yet</span>';
}

function addCustomTag() {
  if (!CUR) return;
  const input = document.getElementById('bp-tag-input');
  const val = (input.value||'').trim().toLowerCase();
  if (!val) return;
  const st = gst(CUR);
  if (!st.customTags) st.customTags = [];
  if (!st.customTags.includes(val)) {
    st.customTags.push(val);
    saveDB();
    populateTagFilter();
  }
  input.value = '';
  renderCustomTags();
}

function removeCustomTag(idx) {
  if (!CUR) return;
  const st = gst(CUR);
  (st.customTags||[]).splice(idx,1);
  saveDB();
  renderCustomTags();
  populateTagFilter();
}

// ============================================================
// BOTTLE PHOTO
// ============================================================
function addBottlePhoto(input) {
  if (!CUR || !input.files[0]) return;
  const reader = new FileReader();
  reader.onload = function(e) {
    const st = gst(CUR);
    st.photo = e.target.result;
    saveDB();
    renderBottlePhoto();
  };
  reader.readAsDataURL(input.files[0]);
  input.value = '';
}

function removeBottlePhoto() {
  if (!CUR) return;
  const st = gst(CUR);
  delete st.photo;
  saveDB();
  renderBottlePhoto();
}

function renderBottlePhoto() {
  if (!CUR) return;
  const st = gst(CUR);
  const el = document.getElementById('bp-photo-preview');
  const delBtn = document.getElementById('bp-photo-del');
  if (!el) return;
  if (st.photo) {
    el.innerHTML = '<img src="'+st.photo+'" style="width:100%;max-height:160px;object-fit:cover;border-radius:2px;">';
    if (delBtn) delBtn.style.display='inline-flex';
  } else {
    el.innerHTML = '<div style="font-size:9px;color:var(--dove);">No photo yet</div>';
    if (delBtn) delBtn.style.display='none';
  }
}

// ============================================================
// COST PER WEAR
// ============================================================
function saveBottleValue() {
  if (!CUR) return;
  const val = parseFloat(document.getElementById('bp-value').value) || 0;
  gst(CUR).value = val;
  saveDB();
  renderCPW();
}

function renderCPW() {
  if (!CUR) return;
  const st = gst(CUR);
  const el = document.getElementById('bp-cpw');
  if (!el) return;
  const val = st.value || 0;
  const wears = (st.wears||[]).length;
  if (!val) { el.textContent = 'Enter value above to calculate'; el.className=''; return; }
  if (!wears) { el.textContent = 'No wears logged yet'; el.className=''; return; }
  const cpw = val / wears;
  let cls = cpw < 3 ? 'cpw-good' : cpw < 10 ? 'cpw-ok' : 'cpw-bad';
  el.innerHTML = '<span class="'+cls+'">$'+cpw.toFixed(2)+' per wear</span><div style="font-size:8.5px;color:var(--dove);margin-top:3px;">$'+val+' value / '+wears+' wears</div>';
  // Update value input
  const inp = document.getElementById('bp-value');
  if (inp && !inp.value) inp.value = val || '';
}

// ============================================================
// SOTD — SCENT OF THE DAY CARD
// ============================================================
function generateSOTD() {
  if (!CUR) return;
  const f = DB.col.find(x => x.name === CUR);
  if (!f) return;
  const st = gst(CUR);
  const now = new Date();
  const dateStr = now.toLocaleDateString('en-US',{weekday:'long',month:'long',day:'numeric',year:'numeric'});
  const dna = st.dna || DEFAULT_DNA[CUR] || '';
  const wxStr = WEATHER ? WEATHER.temp + '°F · ' + WEATHER.desc : '';

  const el = document.getElementById('sotd-preview');
  if (!el) return;
  el.innerHTML = '<div class="sotd-card" id="sotd-card-inner">'+
    '<div class="sotd-date">Scent of the Day</div>'+
    '<div style="font-size:22px;margin-bottom:6px;">'+
      (st.photo ? '<img src="'+st.photo+'" style="width:60px;height:60px;object-fit:cover;border-radius:50%;border:2px solid rgba(140,100,40,.3);">' : '&#x1F9F4;')+
    '</div>'+
    '<div class="sotd-name">'+CUR+'</div>'+
    '<div class="sotd-house">'+f.house+'</div>'+
    '<div style="height:1px;background:rgba(140,100,40,.15);margin:10px 0;"></div>'+
    '<div class="sotd-meta">'+
      (dna ? '<div>'+dna+'</div>' : '')+
      (wxStr ? '<div>'+wxStr+'</div>' : '')+
      '<div>'+dateStr+'</div>'+
      ((st.wears||[]).length ? '<div>'+(st.wears.length)+' wears logged</div>' : '')+
    '</div>'+
    (st.rating ? '<div style="font-size:14px;margin-top:8px;color:var(--gold);">'+'★'.repeat(st.rating)+'☆'.repeat(5-st.rating)+'</div>' : '')+
  '</div>'+
  '<div style="font-size:8.5px;color:var(--dove);margin-top:8px;">Screenshot to share &#128248;</div>';
}

// ============================================================
// STREAK CALCULATION
// ============================================================
function calcStreak() {
  // Gather all wear dates across collection
  const allDates = new Set();
  Object.values(DB.st).forEach(st => {
    (st.wears||[]).forEach(d => {
      try { allDates.add(new Date(d).toDateString()); } catch(e) {}
    });
  });

  const sorted = [...allDates].map(d => new Date(d)).sort((a,b) => b-a);
  if (!sorted.length) return {current:0, best:0};

  const now = new Date();
  const todayStr = now.toDateString();
  const yesterdayStr = new Date(now-86400000).toDateString();

  // Check if streak is active (wore today or yesterday)
  let current = 0;
  let check = sorted[0].toDateString() === todayStr || sorted[0].toDateString() === yesterdayStr ? sorted[0] : null;
  if (check) {
    current = 1;
    for (let i = 1; i < sorted.length; i++) {
      const diff = Math.round((check - sorted[i]) / 86400000);
      if (diff === 1) { current++; check = sorted[i]; }
      else break;
    }
  }

  // Best streak ever
  let best = 1, run = 1;
  for (let i = 1; i < sorted.length; i++) {
    const diff = Math.round((sorted[i-1] - sorted[i]) / 86400000);
    if (diff === 1) { run++; if (run > best) best = run; }
    else run = 1;
  }

  return {current, best};
}

function calcAllCPW() {
  return DB.col.map(f => {
    const st = gst(f.name);
    const val = st.value || 0;
    const wears = (st.wears||[]).length;
    if (!val || !wears) return null;
    return {name:f.name, cpw: val/wears, val, wears};
  }).filter(Boolean).sort((a,b) => a.cpw - b.cpw);
}

// ============================================================
// ============================================================
// DUA ADVISOR
// ============================================================
function initDuaAdvisor() {
  // Focus the input when tab opens
  setTimeout(() => {
    const inp = document.getElementById('dua-input');
    if (inp) inp.focus();
  }, 100);
}

function runDuaAdvisor() {
  const query = (document.getElementById('dua-input').value || '').trim();
  if (!query) { alert('Please enter a fragrance name.'); return; }

  const btn = document.getElementById('dua-go-btn');
  btn.textContent = 'Analyzing…';
  btn.disabled = true;

  const resultsEl = document.getElementById('dua-results');
  resultsEl.style.display = 'block';
  resultsEl.innerHTML = '<div style="background:#ffffff;border:1px solid rgba(140,100,40,.15);padding:32px;text-align:center;"><div style="font-family:Cormorant Garamond,serif;font-size:18px;color:var(--gold);animation:pulse 1.4s ease-in-out infinite;">Analyzing ' + query + '…</div></div>';

  setTimeout(function() {
    try {
      const result = analyzeDuaFragrance(query);
      renderDuaResult(result, query);
    } catch(e) {
      resultsEl.innerHTML = '<div style="background:#ffffff;border:1px solid rgba(176,90,66,.2);padding:20px;color:var(--rose);font-size:10px;">Error: ' + e.message + '</div>';
    }
    btn.textContent = '✦ Analyze';
    btn.disabled = false;
  }, 600);
}

// ============================================================
// DUA BRAND KNOWLEDGE BASE
// ============================================================
const DUA_CATALOG = {
  // Aquatic / Marine cluster
  "poseidon's swimming cologne": {fullName:"Poseidon's Swimming Cologne",inspiration:"Creed Aventus Cologne + LV Afternoon Swim",dna:"Aquatic / Marine",keyNotes:"pineapple, sea salt, musk, vetiver",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Layer 2 sprays with His Perspective Extrait for a premium aquatic signature."},
  "poseidon's ocean mist": {fullName:"Poseidon's Ocean Mist",inspiration:"Creed Aventus Cologne × Nautica Voyage",dna:"Aquatic / Marine",keyNotes:"sea breeze, citrus, white musk, woods",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Best on warm days — the marine accord opens beautifully in heat."},
  "acqua di dua": {fullName:"Acqua Di DUA",inspiration:"Acqua di Giò (vintage)",dna:"Aquatic / Marine",keyNotes:"marine, bergamot, rosemary, white musk",priceRange:"$35 - $50",occasion:"casual",season:"ss",sprays:3,tip:"A faithful vintage-style interpretation — great beach and gym scent."},
  "gone swimming": {fullName:"Gone Swimming",inspiration:"LV Afternoon Swim",dna:"Aquatic / Marine",keyNotes:"sea salt, amber, vetiver, iris",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Apply to chest and wrists — longevity is excellent for an aquatic."},
  "jean lowe immortal": {fullName:"Jean Lowe Immortal",inspiration:"LV L'Immensité",dna:"Aquatic / Marine",keyNotes:"ginger, vetiver, woods, sea notes",priceRange:"$38 - $55",occasion:"office",season:"ss",sprays:3,tip:"A layering base — 2 sprays under Ameer Al Oudh Intense is a proven combo."},
  "victorian poseidon": {fullName:"Victorian Poseidon",inspiration:"Aventus + Xerjoff 1861 Renaissance",dna:"Aquatic / Marine",keyNotes:"pineapple, birch, leather, sea accord",priceRange:"$45 - $65",occasion:"special",season:"fw",sprays:3,tip:"Formal and polished — save for special occasions."},
  // Fougère cluster
  "ottoman breeze": {fullName:"Ottoman Breeze",inspiration:"Nishane Hacivat",dna:"Fougère",keyNotes:"bergamot, iris, patchouli, woody musk",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"The ultimate layering base — pairs with almost anything in your collection."},
  "ottomans vert breeze": {fullName:"Ottomans Vert Breeze",inspiration:"Nishane Hacivat × Creed Green Irish Tweed",dna:"Fougère",keyNotes:"green herbs, violet leaf, woods, iris",priceRange:"$40 - $58",occasion:"casual",season:"ss",sprays:3,tip:"Greener and crisper than Ottoman Breeze — great for outdoor daytime."},
  "his perspective extrait": {fullName:"His Perspective Extrait",inspiration:"Prada Paradigme",dna:"Woody / Aromatic",keyNotes:"geranium, iris, sandalwood, vetiver",priceRange:"$45 - $65",occasion:"office",season:"yr",sprays:2,tip:"Use 2 sprays max — this is a powerhouse extrait. Perfect layering anchor."},
  "river fougere": {fullName:"River Fougere",inspiration:"YSL Rive Gauche Pour Homme",dna:"Fougère",keyNotes:"lavender, woods, tonka, oakmoss",priceRange:"$35 - $50",occasion:"office",season:"ss",sprays:3,tip:"A retro-cool fougère — great for days when you want something classic."},
  "gentleman's club": {fullName:"Gentleman's Club",inspiration:"Givenchy Gentleman Society",dna:"Fougère",keyNotes:"iris, vetiver, pear, woods",priceRange:"$38 - $55",occasion:"date",season:"fw",sprays:3,tip:"Sophisticated and modern — perfect business dinner fragrance."},
  // Oriental / Amber cluster
  "casino royale nights extrait": {fullName:"Casino Royale Nights Extrait",inspiration:"Baccarat Rouge 540 Extrait",dna:"Oriental / Amber",keyNotes:"saffron, amberwood, cedar, jasmine",priceRange:"$55 - $80",occasion:"date",season:"fw",sprays:2,tip:"2 sprays is all you need — this beast projects for hours."},
  "fortune": {fullName:"Fortune",inspiration:"Xerjoff Naxos",dna:"Oriental / Amber",keyNotes:"bergamot, honey, tobacco, vanilla",priceRange:"$45 - $65",occasion:"date",season:"fw",sprays:3,tip:"Sweet and powerful — wear this on cold evenings for maximum impact."},
  "aphrodisiac": {fullName:"Aphrodisiac",inspiration:"Initio Psychedelic Love",dna:"Oriental / Amber",keyNotes:"musks, vanilla, iris, patchouli",priceRange:"$45 - $65",occasion:"date",season:"fw",sprays:2,tip:"Layer with Midnight Rendezvous for a seductive evening combo."},
  "bleu de casino elixir extrait": {fullName:"Bleu de Casino Elixir Extrait",inspiration:"Bleu de Chanel + Aventus + BR540 Extrait",dna:"Woody / Aromatic",keyNotes:"labdanum, sandalwood, pineapple, cedar",priceRange:"$55 - $80",occasion:"date",season:"fw",sprays:2,tip:"The ultimate Dua statement piece — save for special evenings out."},
  "midnight candy for 1 & only": {fullName:"Midnight Candy For 1 & Only",inspiration:"La Nuit de L'Homme + Candies for Men + The One",dna:"Oriental / Amber",keyNotes:"cardamom, vanilla, amber, cedar",priceRange:"$40 - $58",occasion:"evening",season:"fw",sprays:3,tip:"An irresistible evening scent — confident and sweet without being cloying."},
  "error 413": {fullName:"Error 413",inspiration:"1 Million Lucky",dna:"Oriental / Amber",keyNotes:"hazelnut, amber, grapefruit, patchouli",priceRange:"$35 - $52",occasion:"evening",season:"fw",sprays:3,tip:"Crowd-pleasing and fun — great for social nights out."},
  "error 410": {fullName:"Error 410",inspiration:"Paco Rabanne 1 Million Absolutely Gold",dna:"Oriental / Amber",keyNotes:"gold accord, amber, leather, patchouli",priceRange:"$38 - $55",occasion:"date",season:"fw",sprays:3,tip:"More refined than Error 413 — a step up for upscale occasions."},
  "queen of the chess": {fullName:"Queen Of The Chess",inspiration:"Mind Games Queening",dna:"Oriental / Amber",keyNotes:"oud, rose, amber, patchouli",priceRange:"$45 - $65",occasion:"date",season:"fw",sprays:2,tip:"A complex oriental — give it 20 minutes to fully develop on skin."},
  "city of dua": {fullName:"City of Dua",inspiration:"LV City of Stars",dna:"Woody / Aromatic",keyNotes:"tobacco, cedar, vetiver, amber",priceRange:"$45 - $65",occasion:"evening",season:"fw",sprays:3,tip:"A sophisticated smoky wood — excellent for smart evening events."},
  "stronger with azure supernova 2.0": {fullName:"Stronger With Azure Supernova 2.0",inspiration:"Stronger With You + ADG Profondo + Roja Elysium + Aventus",dna:"Aquatic / Marine",keyNotes:"chestnut, marine, white musk, cedar",priceRange:"$45 - $65",occasion:"date",season:"fw",sprays:3,tip:"Complex and layered — this one rewards patience as it develops."},
  // Gourmand cluster
  "khamrah qahwa": {fullName:"Khamrah Qahwa",inspiration:"Original",dna:"Gourmand",keyNotes:"coffee, oud, vanilla, musk",priceRange:"$35 - $52",occasion:"evening",season:"fw",sprays:3,tip:"Wear this when you want compliments — it is a crowd magnet."},
  "black widow": {fullName:"Black Widow",inspiration:"Kilian Black Phantom",dna:"Gourmand",keyNotes:"rum, coffee, dark chocolate, musk",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:2,tip:"Seductive and dark — pairs beautifully with Aphrodisiac for date night."},
  "poseidon's cotton candy": {fullName:"Poseidon's Cotton Candy",inspiration:"Aventus + Cotton Candy De Dua",dna:"Gourmand",keyNotes:"cotton candy, pineapple, musk, woods",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Playful and fun — great for casual summer social events."},
  "iconic plums by the fire": {fullName:"Iconic Plums By The Fire",inspiration:"Andy Warhol + By the Fireplace",dna:"Gourmand",keyNotes:"smoked wood, plum, vanilla, marshmallow",priceRange:"$40 - $58",occasion:"evening",season:"fw",sprays:3,tip:"Perfect winter cozy scent — lounge, fireplace, or date night indoors."},
  "cola fizz of tonka beans": {fullName:"Cola Fizz Of Tonka Beans",inspiration:"Mancera Tonka Cola",dna:"Gourmand",keyNotes:"cola, tonka bean, vanilla, citrus",priceRange:"$35 - $52",occasion:"casual",season:"yr",sprays:3,tip:"A unique crowd-pleaser — year-round versatility is a strength."},
  // Tobacco / Smoky
  "smoky cuba tabac": {fullName:"Smoky Cuba Tabac",inspiration:"Alghabra Cuban Tobacco",dna:"Tobacco / Smoky",keyNotes:"tobacco, rum, vanilla, cedar",priceRange:"$40 - $58",occasion:"evening",season:"fw",sprays:3,tip:"A rare tobacco in your collection — fills a genuine gap."},
  "1 & only jazz club": {fullName:"1 & Only Jazz Club",inspiration:"The One + Jazz Club",dna:"Tobacco / Smoky",keyNotes:"tobacco, ginger, rum, white musk",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"Sophisticated lounge scent — perfect for jazz bars and dinner."},
  "jazz maison": {fullName:"Jazz Maison",inspiration:"Maison Margiela Jazz Club",dna:"Tobacco / Smoky",keyNotes:"tobacco, vetiver, rum, amber",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"Similar DNA to 1 & Only Jazz Club — check for redundancy before buying."},
  // Woody / Aromatic
  "bleu de dua attar": {fullName:"Bleu de Dua Attar",inspiration:"Bleu de Chanel",dna:"Woody / Aromatic",keyNotes:"cedar, labdanum, sandalwood, grapefruit",priceRange:"$45 - $65",occasion:"office",season:"yr",sprays:2,tip:"Your anchor piece — attar concentration means 2 sprays lasts all day."},
  "d le attar": {fullName:"D Le Attar",inspiration:"YSL Y Le Parfum",dna:"Woody / Aromatic",keyNotes:"ginger, sage, fenugreek, cedar",priceRange:"$45 - $65",occasion:"office",season:"fw",sprays:2,tip:"Attar concentration — extremely long-lasting, apply sparingly."},
  "the savage attar": {fullName:"The Savage Attar",inspiration:"Dior Sauvage Parfum",dna:"Woody / Aromatic",keyNotes:"ambroxan, lavender, vetiver, pepper",priceRange:"$45 - $65",occasion:"date",season:"yr",sprays:2,tip:"Attar of Sauvage Parfum — incredibly potent, 2 sprays is the max."},
  "midnight rendezvous": {fullName:"Midnight Rendezvous",inspiration:"YSL La Nuit de L'Homme",dna:"Woody / Aromatic",keyNotes:"cardamom, cedar, lavender, vetiver",priceRange:"$38 - $55",occasion:"date",season:"fw",sprays:3,tip:"Layer with Aphrodisiac for one of the best date night combos in your vault."},
  "wooden lucky charm": {fullName:"Wooden Lucky Charm",inspiration:"Dior Bois Talisman",dna:"Woody / Aromatic",keyNotes:"vetiver, woods, amber, musk",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"A sophisticated woody for smart casual to evening events."},
  "true self absolute": {fullName:"True Self Absolute",inspiration:"YSL MYSLF L'Absolu",dna:"Woody / Aromatic",keyNotes:"bergamot, fenugreek, woods, cedar",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:3,tip:"A strong, confident masculine — great for dates and dinners."},
  "aroma of heaven": {fullName:"Aroma of Heaven",inspiration:"Hermès Terre d'Hermès (vintage)",dna:"Woody / Aromatic",keyNotes:"vetiver, orange, pepper, flint",priceRange:"$38 - $55",occasion:"office",season:"yr",sprays:3,tip:"A versatile all-day woody — excellent office and daytime choice."},
  // Floral
  "desert reflection extrait": {fullName:"Desert Reflection Extrait",inspiration:"Amouage Reflection Man",dna:"Floral",keyNotes:"neroli, rose, sandalwood, musk",priceRange:"$55 - $80",occasion:"special",season:"fw",sprays:2,tip:"A luxury floral — reserve for formal occasions and special events."},
  "rome in yellow dream": {fullName:"Rome in Yellow Dream",inspiration:"Valentino Born in Roma Yellow Dream",dna:"Floral",keyNotes:"iris, vanilla, woody notes, jasmine",priceRange:"$38 - $55",occasion:"date",season:"ss",sprays:3,tip:"A warm floral — perfect for spring dates and outdoor events."},
  // Fresh
  "intuition vision": {fullName:"Intuition Vision",inspiration:"Acqua di Giò Profumo",dna:"Aquatic / Marine",keyNotes:"incense, marine, woody notes, patchouli",priceRange:"$38 - $55",occasion:"office",season:"ss",sprays:3,tip:"The refined office aquatic — more gravitas than typical marine frags."},
  "supernova cologne intense": {fullName:"Supernova Cologne Intense",inspiration:"Roja Elysium Eau Intense",dna:"Aquatic / Marine",keyNotes:"citrus, woods, musk, sea notes",priceRange:"$45 - $65",occasion:"office",season:"ss",sprays:3,tip:"Office and gym versatility — clean and powerful simultaneously."},
  "imperiale casino elixir": {fullName:"Imperiale Casino Elixir",inspiration:"Millésime Impérial + Aventus + BR540 Extrait",dna:"Aquatic / Marine",keyNotes:"melon, sea salt, musk, woods",priceRange:"$55 - $80",occasion:"special",season:"ss",sprays:2,tip:"A premium summer special occasion scent — save this for events."},
  "imperiale matrix": {fullName:"Imperialé Matrix",inspiration:"Creed Millésime Impérial × Xerjoff Nio",dna:"Aquatic / Marine",keyNotes:"sea breeze, musk, cedar, bergamot",priceRange:"$45 - $65",occasion:"office",season:"ss",sprays:3,tip:"A sophisticated daytime marine — elevated above typical aquatics."},
  "the mobster vs poseidon": {fullName:"The Mobster vs Poseidon",inspiration:"Roja Creation-E × Creed Aventus",dna:"Woody / Aromatic",keyNotes:"birch, apple, tobacco, sea",priceRange:"$50 - $72",occasion:"date",season:"fw",sprays:3,tip:"Complex and polarizing — check how it develops on your skin before committing."},
  "midnight fig": {fullName:"Midnight Fig",inspiration:"Nest Indigo",dna:"Citrus / Fresh",keyNotes:"fig, violet, musk, ambers",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"One of few citrus/fresh in your collection — a genuine gap-filler."},

  // ---- ALL REMAINING DUA COLLECTION BOTTLES ----
  "#imagine": {fullName:"#Imagine",inspiration:"Louis Vuitton Imagination",dna:"Aquatic / Marine",keyNotes:"aldehydes, woods, musk, sea",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"A surprisingly unique take on the LV Imagination DNA — more linear but excellent longevity."},
  "bet on 67": {fullName:"Bet On 67",inspiration:"Ralph Lauren Polo 67",dna:"Fougère",keyNotes:"lavender, oakmoss, herbs, woods",priceRange:"$35 - $50",occasion:"sport",season:"ss",sprays:3,tip:"A retro sport fougère — great for outdoor casual days."},
  "bleu de dua exclusive extrait": {fullName:"Bleu de Dua Exclusive Extrait",inspiration:"Bleu de Chanel L'Exclusif",dna:"Woody / Aromatic",keyNotes:"labdanum, cedarwood, sandalwood, incense",priceRange:"$55 - $80",occasion:"office",season:"fw",sprays:2,tip:"The most formal Bleu de Dua — reserve for business formal and special occasions."},
  "d le parfum intense": {fullName:"D Le Parfum Intense",inspiration:"YSL Y EDP Intense",dna:"Woody / Aromatic",keyNotes:"sage, cedar, ginger, fenugreek",priceRange:"$40 - $58",occasion:"evening",season:"fw",sprays:3,tip:"More intense and smoky than D Le Attar — excellent for evening wear."},
  "drowning in bleu de dua attar": {fullName:"Drowning in Bleu de Dua Attar",inspiration:"Bleu de Chanel + Nishane Ani",dna:"Woody / Aromatic",keyNotes:"cedar, musk, sandalwood, floral",priceRange:"$50 - $72",occasion:"date",season:"fw",sprays:2,tip:"An attar — incredibly potent. Two sprays will last 12+ hours."},
  "drowning bleu de savage fierce extrait": {fullName:"Drowning Bleu de Savage Fierce Extrait",inspiration:"Ani + Sauvage EDT + Fierce + BdC",dna:"Woody / Aromatic",keyNotes:"ambroxan, woods, musk, pepper",priceRange:"$55 - $80",occasion:"evening",season:"fw",sprays:2,tip:"A powerhouse extrait — wear sparingly. Best for club nights and bold evening events."},
  "his intense aspiration": {fullName:"His Intense Aspiration",inspiration:"Allure Homme Blanche + AHS Eau Extreme",dna:"Fougère",keyNotes:"white woods, citrus, aldehydes, musk",priceRange:"$38 - $55",occasion:"office",season:"ss",sprays:3,tip:"A sophisticated clean fougère — versatile office and daytime choice."},
  "his loyalty": {fullName:"His Loyalty",inspiration:"D&G Devotion Pour Homme",dna:"Floral",keyNotes:"neroli, iris, woods, musk",priceRange:"$35 - $50",occasion:"casual",season:"ss",sprays:3,tip:"A light floral masculine — good for warm casual days."},
  "fierce savage": {fullName:"Fierce Savage",inspiration:"Abercrombie Fierce + Dior Sauvage EDT",dna:"Woody / Aromatic",keyNotes:"ambroxan, woods, pepper, musk",priceRange:"$35 - $50",occasion:"sport",season:"ss",sprays:3,tip:"A bold sporty woody — great for gym and outdoor casual."},
  "his royalty": {fullName:"His Royalty",inspiration:"Prada L'Homme L'Eau",dna:"Floral",keyNotes:"iris, vetiver, woods, citrus",priceRange:"$35 - $50",occasion:"office",season:"ss",sprays:3,tip:"Light and elegant — a refined office daytime choice for warm months."},
  "his aspiration extreme sport": {fullName:"His Aspiration Extreme Sport",inspiration:"Chanel Allure Homme Sport Eau Extrême",dna:"Aquatic / Marine",keyNotes:"neroli, cedar, vetiver, white musk",priceRange:"$38 - $55",occasion:"sport",season:"ss",sprays:3,tip:"A refined sporty aquatic — transitions well from gym to casual daytime."},
  "his og aspiration": {fullName:"His OG Aspiration",inspiration:"Chanel Allure Homme (1999 vintage)",dna:"Fougère",keyNotes:"aldehydes, woods, vanilla, musk",priceRange:"$38 - $55",occasion:"office",season:"fw",sprays:3,tip:"A vintage-style fougère — sophisticated and office-appropriate."},
  "iconic greenwich village": {fullName:"Iconic Greenwich Village",inspiration:"Bond No. 9 Greenwich Village",dna:"Fougère",keyNotes:"bergamot, leather, woods, iris",priceRange:"$40 - $58",occasion:"casual",season:"ss",sprays:3,tip:"An urban creative scent — great for social daytime events."},
  "imperial blue": {fullName:"Imperial Blue",inspiration:"Bleu de Chanel + Creed Millésime Impérial",dna:"Aquatic / Marine",keyNotes:"melon, sea breeze, cedar, musk",priceRange:"$40 - $58",occasion:"date",season:"ss",sprays:3,tip:"A premium summer date scent — marine and luxurious."},
  "mystical amulet of blue": {fullName:"Mystical Amulet of Blue",inspiration:"Ex Nihilo Blue Talisman",dna:"Aquatic / Marine",keyNotes:"sea spray, iris, musk, woods",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"A niche-inspired aquatic — more refined than typical marine fragrances."},
  "peace with poseidon": {fullName:"Peace with Poseidon",inspiration:"Scent of Peace + Aventus",dna:"Aquatic / Marine",keyNotes:"pineapple, sea, musk, woods",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Pineapple-forward aquatic — very wearable for outdoors and weekend casual."},
  "spice it up metallic musk": {fullName:"Spice It Up Metallic Musk",inspiration:"Viktor & Rolf Spicebomb Metallic Musk",dna:"Oriental / Amber",keyNotes:"pepper, metallic musk, amber, wood",priceRange:"$38 - $55",occasion:"office",season:"fw",sprays:3,tip:"A modern spicy musk — very office-appropriate for fall and winter."},
  "poseidon's fireplace": {fullName:"Poseidon's Fireplace",inspiration:"Aventus + By the Fireplace",dna:"Woody / Aromatic",keyNotes:"smoked wood, pineapple, musk, vanilla",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:3,tip:"A unique combo — the Aventus DNA grounds the smoky fireside accord beautifully."},
  "dua's soho": {fullName:"Dua's SoHo",inspiration:"Bond No. 9 Soho",dna:"Fougère",keyNotes:"herbs, iris, leather, musk",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Urban and creative — excellent for gallery openings, social events."},
  "true self absolute": {fullName:"True Self Absolute",inspiration:"YSL MYSLF L'Absolu",dna:"Woody / Aromatic",keyNotes:"bergamot, fenugreek, woods, cedar",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:3,tip:"A strong confident masculine — great for dates and dinners."},
  "dua's water primal essence": {fullName:"Dua's Water Primal Essence",inspiration:"Acqua di Giò Absolu",dna:"Aquatic / Marine",keyNotes:"incense, sea, patchouli, woody",priceRange:"$38 - $55",occasion:"office",season:"ss",sprays:3,tip:"The darker, moodier side of ADG — more presence than Acqua Di DUA."},
  "rome in coral fantasy": {fullName:"Rome In Coral Fantasy",inspiration:"Valentino Born in Roma Coral Fantasy",dna:"Floral",keyNotes:"peach, jasmine, musk, vanilla",priceRange:"$38 - $55",occasion:"date",season:"ss",sprays:3,tip:"Fruity floral — best for warm weather dates and brunch."},
  "1 & only jazz club": {fullName:"1 & Only Jazz Club",inspiration:"The One + Jazz Club",dna:"Tobacco / Smoky",keyNotes:"tobacco, ginger, rum, white musk",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"Sophisticated lounge scent — perfect for jazz bars and dinner."},
  "rome in green": {fullName:"Rome In Green",inspiration:"Valentino Born in Roma Green Stravaganza",dna:"Fougère",keyNotes:"herbs, vetiver, woods, citrus",priceRange:"$38 - $55",occasion:"casual",season:"ss",sprays:3,tip:"Fresh and green — excellent outdoor and weekend casual scent."},

  // ---- POPULAR DUA FRAGRANCES NOT YET IN YOUR COLLECTION ----
  "his intensified aspiration": {fullName:"His Intensified Aspiration",inspiration:"Chanel Allure Homme Intense",dna:"Oriental / Amber",keyNotes:"vanilla, cedar, cardamom, musk",priceRange:"$38 - $55",occasion:"date",season:"fw",sprays:3,tip:"Richer and warmer than His Aspiration variants — excellent date night choice."},
  "his obsession": {fullName:"His Obsession",inspiration:"Calvin Klein Obsession pour Homme",dna:"Oriental / Amber",keyNotes:"bergamot, oakmoss, amber, vanilla",priceRange:"$35 - $50",occasion:"date",season:"fw",sprays:3,tip:"A classic retro oriental — powerful and long-lasting."},
  "poseidon's oud": {fullName:"Poseidon's Oud",inspiration:"Creed Aventus + Oud DNA",dna:"Oud / Resinous",keyNotes:"oud, pineapple, musk, resin",priceRange:"$45 - $65",occasion:"evening",season:"fw",sprays:2,tip:"Fills your Oud gap while staying in the Aventus DNA family you love."},
  "the pasha": {fullName:"The Pasha",inspiration:"Cartier Pasha de Cartier",dna:"Fougère",keyNotes:"mint, woods, musk, amber",priceRange:"$35 - $50",occasion:"office",season:"ss",sprays:3,tip:"A classic fougère with mint freshness — excellent office choice for spring."},
  "midnight oud": {fullName:"Midnight Oud",inspiration:"Roja Dove Amber Aoud",dna:"Oud / Resinous",keyNotes:"oud, amber, rose, saffron",priceRange:"$45 - $65",occasion:"evening",season:"fw",sprays:2,tip:"A genuine oud oriental — fills your Oud/Resinous gap meaningfully."},
  "celestial": {fullName:"Celestial",inspiration:"Initio High Frequency",dna:"Musky / Skin",keyNotes:"musk, sandalwood, iris, white florals",priceRange:"$40 - $58",occasion:"casual",season:"yr",sprays:3,tip:"A clean, refined skin scent — adds the Musky/Skin DNA you are light on."},
  "adventure seeker": {fullName:"Adventure Seeker",inspiration:"Davidoff Adventure",dna:"Citrus / Fresh",keyNotes:"grapefruit, woods, musk, herbs",priceRange:"$35 - $50",occasion:"sport",season:"ss",sprays:3,tip:"A fresh citrus sporty — good if you want more Citrus/Fresh options."},
  "amber elixir": {fullName:"Amber Elixir",inspiration:"Amouage Interlude",dna:"Oriental / Amber",keyNotes:"oud, amber, frankincense, oregano",priceRange:"$45 - $65",occasion:"special",season:"fw",sprays:2,tip:"A complex oriental powerhouse — special occasions only."},
  "his creed": {fullName:"His Creed",inspiration:"Creed Original Vetiver",dna:"Woody / Aromatic",keyNotes:"vetiver, grapefruit, sandalwood, white musk",priceRange:"$38 - $55",occasion:"office",season:"ss",sprays:3,tip:"A refined vetiver — excellent all-day office wear for warm months."},
  "bleu savage": {fullName:"Bleu Savage",inspiration:"Bleu de Chanel + Dior Sauvage",dna:"Woody / Aromatic",keyNotes:"ambroxan, cedar, labdanum, grapefruit",priceRange:"$38 - $55",occasion:"office",season:"yr",sprays:3,tip:"Two of the most popular DNA families combined — extremely versatile."},
  "noir leather": {fullName:"Noir Leather",inspiration:"Tom Ford Noir Extreme",dna:"Oriental / Amber",keyNotes:"leather, amber, saffron, rose",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:2,tip:"A dark, seductive leather oriental — powerful date night choice."},
  "the explorer": {fullName:"The Explorer",inspiration:"Montblanc Explorer",dna:"Woody / Aromatic",keyNotes:"bergamot, vetiver, leather, woods",priceRange:"$35 - $50",occasion:"casual",season:"yr",sprays:3,tip:"Approachable and versatile — good everyday option if you need more yr bottles."},
  "rose oud": {fullName:"Rose Oud",inspiration:"Montale Rose Oud",dna:"Oud / Resinous",keyNotes:"rose, oud, musk, patchouli",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:2,tip:"A classic rose oud — fills both your Oud and Floral gaps simultaneously."},
  "santal royale": {fullName:"Santal Royale",inspiration:"Santal 33 (Le Labo)",dna:"Woody / Aromatic",keyNotes:"sandalwood, leather, cardamom, violet",priceRange:"$40 - $58",occasion:"casual",season:"yr",sprays:3,tip:"A creamy sandalwood — very wearable and crowd-pleasing."},
  "oud royale": {fullName:"Oud Royale",inspiration:"Kilian Black Oud",dna:"Oud / Resinous",keyNotes:"oud, rose, amber, incense",priceRange:"$45 - $65",occasion:"special",season:"fw",sprays:2,tip:"A rich royal oud — fills your Oud/Resinous gap with maximum impact."},
  "poseidon's elixir": {fullName:"Poseidon's Elixir",inspiration:"Creed Aventus Elixir",dna:"Aquatic / Marine",keyNotes:"pineapple, amber, musk, woods",priceRange:"$50 - $72",occasion:"date",season:"yr",sprays:2,tip:"Aventus Elixir DNA — richer and more amber-forward than the original."},
  "blue seduction": {fullName:"Blue Seduction",inspiration:"Antonio Banderas Blue Seduction",dna:"Aquatic / Marine",keyNotes:"apple, violet, woods, musk",priceRange:"$30 - $45",occasion:"casual",season:"ss",sprays:3,tip:"A budget-friendly fresh aquatic — good casual wear without overthinking."},
  "oud for kings": {fullName:"Oud For Kings",inspiration:"Initio Oud for Greatness",dna:"Oud / Resinous",keyNotes:"oud, violet, musk, woods",priceRange:"$45 - $65",occasion:"special",season:"fw",sprays:2,tip:"Bold and massive — you already have Bade'e Al Oud For Glory nearby, check for redundancy."},
  "l'homme intense": {fullName:"L'Homme Intense",inspiration:"YSL L'Homme Intense",dna:"Woody / Aromatic",keyNotes:"basil, ginger, cedar, vetiver",priceRange:"$38 - $55",occasion:"office",season:"fw",sprays:3,tip:"A classic YSL-style woody aromatic — refined and office-appropriate."},
  "beach day": {fullName:"Beach Day",inspiration:"Escada Into the Sun",dna:"Citrus / Fresh",keyNotes:"coconut, citrus, sea salt, musk",priceRange:"$35 - $50",occasion:"casual",season:"ss",sprays:3,tip:"A true beach scent — adds Citrus/Fresh variety to your collection."},
  "velvet oud": {fullName:"Velvet Oud",inspiration:"Mancera Velvet Vanilla",dna:"Gourmand",keyNotes:"oud, vanilla, sandalwood, caramel",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:2,tip:"A sweet, smooth gourmand oud hybrid — unique combination in your collection."},
  "tobacco oud": {fullName:"Tobacco Oud",inspiration:"Tom Ford Tobacco Oud",dna:"Tobacco / Smoky",keyNotes:"tobacco, oud, amber, spice",priceRange:"$45 - $65",occasion:"evening",season:"fw",sprays:2,tip:"A premium tobacco oud — fills both Tobacco and Oud gaps simultaneously."},
  "his absolute": {fullName:"His Absolute",inspiration:"Chanel Allure Homme Edition Blanche",dna:"Fougère",keyNotes:"aldehydes, vetiver, cedar, musk",priceRange:"$40 - $58",occasion:"office",season:"ss",sprays:3,tip:"A sophisticated clean fougère — excellent office choice for spring and summer."},
  "amber wood": {fullName:"Amber Wood",inspiration:"Amouage Jubilation XXV",dna:"Oriental / Amber",keyNotes:"frankincense, amber, myrrh, patchouli",priceRange:"$45 - $65",occasion:"special",season:"fw",sprays:2,tip:"A complex luxury oriental — powerful and long-lasting, save for special occasions."},
  "night out": {fullName:"Night Out",inspiration:"Paco Rabanne 1 Million Prive",dna:"Oriental / Amber",keyNotes:"cinnamon, leather, amber, tobacco",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"Check against your existing 1 Million-adjacent bottles before buying."},
  "dua's noir": {fullName:"Dua's Noir",inspiration:"YSL La Nuit de L'Homme Bleu Electrique",dna:"Oriental / Amber",keyNotes:"cardamom, lavender, cedar, amber",priceRange:"$38 - $55",occasion:"evening",season:"fw",sprays:3,tip:"A darker spin on the La Nuit DNA you have in Midnight Rendezvous."},
  "poseidon's legend": {fullName:"Poseidon's Legend",inspiration:"Creed Aventus + Dior Homme Sport",dna:"Aquatic / Marine",keyNotes:"pineapple, grapefruit, musk, sea",priceRange:"$40 - $58",occasion:"casual",season:"ss",sprays:3,tip:"A sporty Aventus variant — check for redundancy with your existing Poseidon bottles."},
  "oud incense": {fullName:"Oud Incense",inspiration:"Maison Francis Kurkdjian Oud Satin Mood",dna:"Oud / Resinous",keyNotes:"oud, incense, violet, benzoin",priceRange:"$45 - $65",occasion:"special",season:"fw",sprays:2,tip:"A luxury incense oud — genuinely fills your Oud gap with class."},
  "summer love": {fullName:"Summer Love",inspiration:"Versace Eros Flame",dna:"Oriental / Amber",keyNotes:"tomato leaf, lemon, geranium, amber",priceRange:"$35 - $50",occasion:"date",season:"ss",sprays:3,tip:"A summer-friendly oriental — good for warm weather dates and evenings."},
  "chypre woods": {fullName:"Chypre Woods",inspiration:"Parfums de Marly Herod",dna:"Chypre",keyNotes:"pipe tobacco, woods, vanilla, amber",priceRange:"$40 - $58",occasion:"evening",season:"fw",sprays:3,tip:"Adds the Chypre DNA that is completely missing from your collection — high value add."},
  "green oud": {fullName:"Green Oud",inspiration:"Xerjoff Alexandria II",dna:"Oud / Resinous",keyNotes:"rose, oud, sandalwood, green notes",priceRange:"$45 - $65",occasion:"date",season:"ss",sprays:2,tip:"A rare green-inflected oud — very unique in the Dua lineup."},
  "leather noir": {fullName:"Leather Noir",inspiration:"Parfums de Marly Layton",dna:"Floral",keyNotes:"apple, lavender, vanilla, woods",priceRange:"$38 - $55",occasion:"date",season:"yr",sprays:3,tip:"Despite the name this follows the Layton profile — a warm versatile crowd-pleaser."},
  "his intensity": {fullName:"His Intensity",inspiration:"Dior Homme Intense",dna:"Floral",keyNotes:"iris, amber, cocoa, woods",priceRange:"$38 - $55",occasion:"date",season:"fw",sprays:3,tip:"A powdery iris oriental — one of the most unique DNA profiles Dua offers."},
  "white musk": {fullName:"White Musk",inspiration:"Narciso Rodriguez For Him",dna:"Musky / Skin",keyNotes:"white musk, amber, vetiver",priceRange:"$35 - $50",occasion:"casual",season:"yr",sprays:3,tip:"A clean minimalist skin musk — adds the Musky/Skin DNA you barely have."},
  "smoky oud": {fullName:"Smoky Oud",inspiration:"By Kilian Black Phantom + Oud",dna:"Tobacco / Smoky",keyNotes:"rum, coffee, oud, vanilla",priceRange:"$40 - $58",occasion:"evening",season:"fw",sprays:2,tip:"Builds on the Black Phantom DNA in your Black Widow — check for redundancy first."},
  "aqua verde": {fullName:"Aqua Verde",inspiration:"Hermès Eau de Citron Noir",dna:"Citrus / Fresh",keyNotes:"black lemon, bergamot, woods, musk",priceRange:"$35 - $50",occasion:"casual",season:"ss",sprays:3,tip:"A rare citrus in the Dua lineup — genuinely fills your Citrus/Fresh gap."},
  "cashmere oud": {fullName:"Cashmere Oud",inspiration:"Guerlain L'Instant Pour Homme",dna:"Oriental / Amber",keyNotes:"amber, cashmere, oud, sandalwood",priceRange:"$40 - $58",occasion:"date",season:"fw",sprays:3,tip:"A soft, warm oriental — approachable and crowd-pleasing."},
};

function analyzeDuaFragrance(query) {
  const q = query.toLowerCase().trim();
  
  // Try to find in catalog — fuzzy match
  let match = null;
  let matchKey = null;
  
  // Exact key match
  if (DUA_CATALOG[q]) { match = DUA_CATALOG[q]; matchKey = q; }
  
  // Partial match — find best
  if (!match) {
    let bestScore = 0;
    for (const key of Object.keys(DUA_CATALOG)) {
      const words = q.split(' ').filter(w => w.length > 2);
      const target = (key + ' ' + DUA_CATALOG[key].fullName.toLowerCase() + ' ' + DUA_CATALOG[key].inspiration.toLowerCase());
      // Score: word matches + substring bonus
      let score = words.filter(w => target.includes(w)).length;
      // Bonus if query is a substring of the key
      if (key.includes(q) || q.includes(key.slice(0,8))) score += 3;
      if (score > bestScore) { bestScore = score; match = DUA_CATALOG[key]; matchKey = key; }
    }
    // Require at least 1 word match to avoid false positives
    if (bestScore === 0) { match = null; matchKey = null; }
  }

  // If no match at all, generate a generic analysis
  if (!match || !matchKey) {
    return analyzeUnknownDua(query);
  }

  const info = match;
  const fullName = info.fullName;

  // Check if already owned
  const alreadyOwned = DB.col.find(f => f.name.toLowerCase() === fullName.toLowerCase());
  if (alreadyOwned) {
    return {
      fullName, inspiration: info.inspiration, dna: info.dna,
      keyNotes: info.keyNotes, priceRange: info.priceRange,
      verdict: 'SKIP', confidence: 10,
      reason: 'You already own ' + fullName + ' — it is in your vault! No need to repurchase unless you need a backup.',
      redundantWith: fullName + ' (already owned)',
      gapFilled: '', occasion: info.occasion, season: info.season,
      sprays: info.sprays, extraTip: info.tip
    };
  }

  // Check DNA redundancy against existing collection
  const sameDNA = DB.col.filter(f => {
    const fDNA = gst(f.name).dna || DEFAULT_DNA[f.name] || '';
    return fDNA === info.dna;
  });

  // Check inspiration redundancy — similar inspiration base
  const inspBase = info.inspiration.split('×')[0].split('+')[0].split('x ')[0].trim().toLowerCase();
  const sameInsp = DB.col.filter(f => f.inspiration.toLowerCase().includes(inspBase) && inspBase.length > 4);

  // DNA gap — if no bottles in this family
  const isDNAGap = sameDNA.length === 0;
  const isInspRedundant = sameInsp.length >= 2;

  let verdict, confidence, reason, redundantWith = '', gapFilled = '';

  if (isDNAGap) {
    verdict = 'BUY';
    confidence = 9;
    reason = 'Your collection has zero bottles in the ' + info.dna + ' family. ' + fullName + ' would fill a genuine DNA gap and add range to your rotation. A must-add.';
    gapFilled = info.dna + ' family — currently unrepresented in your vault';
  } else if (isInspRedundant) {
    verdict = 'SKIP';
    confidence = 8;
    reason = 'You already own ' + sameInsp.length + ' bottle(s) inspired by ' + sameInsp[0].inspiration.split('+')[0].trim() + ', including ' + sameInsp[0].name + '. Adding ' + fullName + ' risks significant redundancy without meaningful differentiation.';
    redundantWith = sameInsp.map(f => f.name).join(', ');
  } else if (sameDNA.length >= 8) {
    verdict = 'SKIP';
    confidence = 7;
    reason = 'You already have ' + sameDNA.length + ' bottles in the ' + info.dna + ' family — one of your largest clusters. Unless ' + fullName + ' offers something distinctly unique, it risks getting lost in the rotation.';
    redundantWith = sameDNA.slice(0,3).map(f => f.name).join(', ') + ' (and ' + (sameDNA.length-3) + ' more)';
  } else if (sameDNA.length <= 2) {
    verdict = 'BUY';
    confidence = 8;
    reason = 'The ' + info.dna + ' family is underrepresented in your collection with only ' + sameDNA.length + ' bottle(s). ' + fullName + ' would add meaningful variety and give you more options in this DNA space.';
    gapFilled = info.dna + ' family depth (currently ' + sameDNA.length + ' bottles)';
  } else {
    // Medium redundancy — season and occasion matter
    const sameOccDNA = sameDNA.filter(f => f.occ_key === info.occasion);
    if (sameOccDNA.length >= 3) {
      verdict = 'SKIP';
      confidence = 6;
      reason = 'You have ' + sameOccDNA.length + ' bottles with similar DNA and occasion profile. ' + fullName + ' would add to an already well-covered area. Consider only if the specific inspiration is not in your collection.';
      redundantWith = sameOccDNA.slice(0,2).map(f => f.name).join(', ');
    } else {
      verdict = 'BUY';
      confidence = 7;
      reason = 'While you have ' + sameDNA.length + ' bottles in the ' + info.dna + ' family, your ' + info.occasion + ' options in this DNA are limited. ' + fullName + ' would add useful variety without significant redundancy.';
      gapFilled = info.dna + ' for ' + info.occasion + ' occasions';
    }
  }

  return {
    fullName, inspiration: info.inspiration, dna: info.dna,
    keyNotes: info.keyNotes, priceRange: info.priceRange,
    verdict, confidence, reason, redundantWith, gapFilled,
    occasion: info.occasion, season: info.season,
    sprays: info.sprays, extraTip: info.tip
  };
}

function analyzeUnknownDua(query) {
  // For fragrances not in the catalog, do a best-guess analysis
  return {
    fullName: query + ' (Dua Brand)',
    inspiration: 'Unknown — fragrance not in database',
    dna: 'Woody / Aromatic',
    keyNotes: 'Not available',
    priceRange: '$35 - $65',
    verdict: 'BUY',
    confidence: 4,
    reason: 'This fragrance is not in the local database, so a full analysis is not available. Based on the name, it appears to be a Dua Brand fragrance — visit duabrand.com to check the notes and inspiration before purchasing. Low confidence rating reflects limited data.',
    redundantWith: '',
    gapFilled: 'Requires manual research',
    occasion: 'casual',
    season: 'yr',
    sprays: 3,
    extraTip: 'Visit duabrand.com to read reviews and check if the inspiration is already covered by your collection before buying.'
  };
}

function renderDuaResult(r, query) {
  window._duaResult = r;
  const isBuy = r.verdict === 'BUY';
  const verdictColor = isBuy ? 'var(--forest)' : 'var(--rose)';
  const verdictBg = isBuy ? 'rgba(45,80,40,.07)' : 'rgba(176,90,66,.07)';
  const verdictIcon = isBuy ? '✓' : '✕';
  const dnaCol = DNA_FAMILIES[r.dna]?.color || 'var(--gold)';
  const occMap = {date:'♥ Date',office:'◆ Office',evening:'✦ Evening',casual:'■ Casual',sport:'▲ Sport',special:'★ Special'};
  const seaMap = {ss:'Spring · Summer',fw:'Fall · Winter',yr:'Year-round'};

  // Confidence bar
  const conf = Math.min(10, Math.max(1, r.confidence || 5));
  const confBar = Array.from({length:10},(_,i) =>
    '<div style="flex:1;height:6px;background:' + (i < conf ? verdictColor : 'rgba(140,100,40,.15)') + ';"></div>'
  ).join('');

  const resultsEl = document.getElementById('dua-results');
  resultsEl.innerHTML = `
    <!-- VERDICT HEADER -->
    <div style="background:${verdictBg};border:1px solid ${verdictColor}44;border-left:5px solid ${verdictColor};padding:24px 26px;margin-bottom:1px;">
      <div style="display:flex;align-items:center;justify-content:space-between;flex-wrap:wrap;gap:12px;">
        <div>
          <div style="font-size:7.5px;letter-spacing:.22em;text-transform:uppercase;color:var(--dove);margin-bottom:4px;font-weight:700;">The Dua Brand</div>
          <div style="font-family:'Cormorant Garamond',serif;font-size:26px;font-weight:600;color:var(--cream);line-height:1.1;margin-bottom:3px;">${r.fullName}</div>
          <div style="font-family:'Cormorant Garamond',serif;font-style:italic;font-size:13px;color:var(--dove);">← ${r.inspiration}</div>
        </div>
        <div style="text-align:center;flex-shrink:0;">
          <div style="font-family:'Cormorant Garamond',serif;font-size:52px;font-weight:700;color:${verdictColor};line-height:1;">${verdictIcon}</div>
          <div style="font-size:11px;letter-spacing:.2em;text-transform:uppercase;color:${verdictColor};font-weight:700;">${r.verdict}</div>
        </div>
      </div>

      <!-- Confidence -->
      <div style="margin-top:16px;">
        <div style="font-size:7.5px;letter-spacing:.18em;text-transform:uppercase;color:var(--dove);margin-bottom:6px;font-weight:600;">Confidence ${conf}/10</div>
        <div style="display:flex;gap:2px;">${confBar}</div>
      </div>
    </div>

    <!-- REASON -->
    <div style="background:#ffffff;border:1px solid rgba(140,100,40,.12);padding:20px 26px;margin-bottom:1px;">
      <div style="font-size:8px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:8px;font-weight:700;">Analysis</div>
      <div style="font-size:11px;color:var(--cream);line-height:1.7;font-weight:500;">${r.reason}</div>
      ${r.redundantWith ? '<div style="margin-top:10px;padding:10px 14px;background:rgba(176,90,66,.07);border:1px solid rgba(176,90,66,.2);font-size:10px;color:var(--rose);font-weight:500;">⚠ Redundant with: <strong>' + r.redundantWith + '</strong></div>' : ''}
      ${r.gapFilled ? '<div style="margin-top:10px;padding:10px 14px;background:rgba(45,80,40,.07);border:1px solid rgba(45,80,40,.25);font-size:10px;color:var(--forest);font-weight:500;">✓ Fills gap: ' + r.gapFilled + '</div>' : ''}
    </div>

    <!-- DETAILS ROW -->
    <div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(140px,1fr));gap:1px;background:rgba(140,100,40,.12);margin-bottom:1px;">
      <div style="background:#ffffff;padding:16px 18px;">
        <div style="font-size:7px;letter-spacing:.18em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">DNA Family</div>
        <div style="font-size:11px;color:${dnaCol};font-weight:700;">${r.dna}</div>
      </div>
      <div style="background:#ffffff;padding:16px 18px;">
        <div style="font-size:7px;letter-spacing:.18em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Key Notes</div>
        <div style="font-size:10px;color:var(--cream);font-weight:500;">${r.keyNotes}</div>
      </div>
      <div style="background:#ffffff;padding:16px 18px;">
        <div style="font-size:7px;letter-spacing:.18em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Price Range</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:18px;color:var(--gold);font-weight:600;">${r.priceRange}</div>
      </div>
      <div style="background:#ffffff;padding:16px 18px;">
        <div style="font-size:7px;letter-spacing:.18em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Best For</div>
        <div style="font-size:10px;color:var(--cream);font-weight:500;">${occMap[r.occasion]||r.occasion}</div>
        <div style="font-size:9px;color:var(--dove);margin-top:2px;">${seaMap[r.season]||r.season}</div>
      </div>
      <div style="background:#ffffff;padding:16px 18px;">
        <div style="font-size:7px;letter-spacing:.18em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">Sprays</div>
        <div style="font-family:'Cormorant Garamond',serif;font-size:28px;color:var(--gold);font-weight:600;line-height:1;">${r.sprays}</div>
      </div>
    </div>

    <!-- TIP -->
    <div style="background:#ffffff;border:1px solid rgba(140,100,40,.12);padding:16px 26px;margin-bottom:1px;">
      <div style="font-size:8px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);margin-bottom:6px;font-weight:700;">💡 Pro Tip</div>
      <div style="font-size:10.5px;color:var(--cream);line-height:1.6;font-weight:400;">${r.extraTip}</div>
    </div>

    <!-- ADD TO VAULT BUTTON (only if BUY) -->
    ${isBuy ? `
    <div style="background:#ffffff;border:1px solid rgba(45,80,40,.25);padding:20px 26px;">
      <div style="font-size:8px;letter-spacing:.2em;text-transform:uppercase;color:var(--forest);margin-bottom:8px;font-weight:700;">Ready to Buy?</div>
      <div style="font-size:10px;color:var(--dove);margin-bottom:14px;">Add it to your vault now so it's ready when it arrives.</div>
      <button class="btn btn-gold" onclick="addDuaToVault()"/g,'&quot;')})" style="font-size:9px;padding:11px 20px;">
        + Add to My Vault
      </button>
    </div>` : `
    <div style="background:#ffffff;border:1px solid rgba(176,90,66,.15);padding:20px 26px;">
      <div style="font-size:10px;color:var(--dove);line-height:1.6;">Want to search a different Dua fragrance? Type another name above.</div>
    </div>`}

    <!-- SEARCH AGAIN -->
    <div style="padding:16px 0;text-align:center;">
      <button class="btn btn-muted" onclick="document.getElementById('dua-input').value='';document.getElementById('dua-results').style.display='none';document.getElementById('dua-input').focus();" style="font-size:8.5px;">
        ← Search Another Fragrance
      </button>
    </div>
  `;
}

function addDuaToVault() {
  const r = window._duaResult;
  if (!r) { alert('No result to add.'); return; }

  // Check if already exists
  if (DB.col.find(f => f.name.toLowerCase() === r.fullName.toLowerCase())) {
    alert(r.fullName + ' is already in your vault!');
    return;
  }

  // Add to collection
  const newBottle = {
    house: 'The Dua Brand',
    name: r.fullName,
    inspiration: r.inspiration || 'Original',
    occ_key: r.occasion || 'casual',
    occ_detail: r.occasion || 'Casual / everyday',
    s_key: r.season || 'yr',
  };
  DB.col.push(newBottle);

  // Set DNA and notes in state
  const st = gst(r.fullName);
  if (r.dna) st.dna = r.dna;
  if (r.extraTip) st.notes = 'Advisor tip: ' + r.extraTip;

  saveDB();
  populateHouses();
  populateSugSelect();
  updateStats();

  // Show confirmation
  const btn = event.target;
  btn.textContent = '✓ Added to Vault!';
  btn.style.color = 'var(--forest)';
  btn.style.borderColor = 'var(--forest)';
  btn.disabled = true;

  setTimeout(() => {
    if (confirm(r.fullName + ' added! Go to your collection to see it?')) {
      showPage('collection', document.querySelector('.nav-tab'));
    }
  }, 500);
}

// ============================================================
// IMPORT / EXPORT
// ============================================================
const CSV_COLUMNS = [
  {col:'house',       req:true,  example:'The Dua Brand',         note:'Brand or house name'},
  {col:'name',        req:true,  example:'Ottoman Breeze',         note:'Full fragrance name'},
  {col:'inspiration', req:false, example:'Nishane Hacivat',        note:'Inspired by / DNA reference'},
  {col:'occasion',    req:false, example:'casual',                 note:'date / office / evening / casual / sport / special'},
  {col:'season',      req:false, example:'ss',                     note:'ss = Spring/Summer  fw = Fall/Winter  yr = Year-round'},
  {col:'dna',         req:false, example:'Fougère',                note:'Aquatic / Marine, Fougère, Woody / Aromatic, Oriental / Amber, Oud / Resinous, Citrus / Fresh, Gourmand, Floral, Chypre, Tobacco / Smoky, Musky / Skin'},
  {col:'base',        req:false, example:'yes',                    note:'yes = layering base bottle'},
  {col:'notes',       req:false, example:'Great projection',       note:'Personal notes'},
  {col:'rating',      req:false, example:'4',                      note:'1-5 stars'},
];

let pendingImport = null;

function renderImportExport() {
  // Build CSV guide table
  const tbody = document.getElementById('csv-guide-body');
  if (tbody) {
    tbody.innerHTML = CSV_COLUMNS.map(c => `
      <tr style="border-bottom:1px solid rgba(140,100,40,.07);">
        <td style="padding:7px 12px;color:var(--cream);font-weight:600;font-family:'Cormorant Garamond',serif;font-size:13px;">${c.col}</td>
        <td style="padding:7px 12px;color:${c.req?'var(--rose)':'var(--dove)'};">${c.req?'Required':'Optional'}</td>
        <td style="padding:7px 12px;color:var(--dove);font-style:italic;">${c.example}</td>
        <td style="padding:7px 12px;color:var(--dove);font-size:9px;">${c.note}</td>
      </tr>`).join('');
  }
}

function exportCSV() {
  const headers = CSV_COLUMNS.map(c => c.col).join(',');
  const rows = DB.col.map(f => {
    const st = gst(f.name);
    const vals = [
      csvCell(f.house),
      csvCell(f.name),
      csvCell(f.inspiration || ''),
      csvCell(f.occ_key || 'casual'),
      csvCell(f.s_key || 'yr'),
      csvCell(st.dna || DEFAULT_DNA[f.name] || ''),
      csvCell(f.isBase ? 'yes' : ''),
      csvCell(st.notes || ''),
      csvCell(st.rating ? String(st.rating) : ''),
    ];
    return vals.join(',');
  });
  const csv = [headers, ...rows].join('\n');
  downloadFile(csv, 'my-fragrance-vault.csv', 'text/csv');
}

function downloadTemplate() {
  const headers = CSV_COLUMNS.map(c => c.col).join(',');
  const example = [
    csvCell('The Dua Brand'),
    csvCell('Ottoman Breeze'),
    csvCell('Nishane Hacivat'),
    csvCell('casual'),
    csvCell('ss'),
    csvCell('Fougère'),
    csvCell('yes'),
    csvCell('Amazing layering base'),
    csvCell('5'),
  ].join(',');
  const csv = [headers, example].join('\n');
  downloadFile(csv, 'fragrance-vault-template.csv', 'text/csv');
}

function csvCell(val) {
  const str = String(val || '');
  if (str.includes(',') || str.includes('"') || str.indexOf('\n') >= 0) {
    return '"' + str.replace(/"/g, '""') + '"';
  }
  return str;
}

function downloadFile(content, filename, type) {
  const blob = new Blob([content], {type});
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url; a.download = filename; a.click();
  setTimeout(() => URL.revokeObjectURL(url), 1000);
}

function importCSV(input) {
  const file = input.files[0];
  if (!file) return;
  const reader = new FileReader();
  reader.onload = function(e) {
    try {
      const text = e.target.result;
      const lines = text.trim().split('\n');
      const headers = parseCSVLine(lines[0]).map(h => h.trim().toLowerCase());
      
      const nameIdx = headers.indexOf('name');
      const houseIdx = headers.indexOf('house');
      if (nameIdx === -1 || houseIdx === -1) {
        setImportStatus('Error: CSV must have "name" and "house" columns.', true);
        return;
      }

      const parsed = [];
      for (let i = 1; i < lines.length; i++) {
        if (!lines[i].trim()) continue;
        const vals = parseCSVLine(lines[i]);
        const get = col => {
          const idx = headers.indexOf(col);
          return idx >= 0 ? (vals[idx] || '').trim() : '';
        };
        const name = get('name');
        const house = get('house');
        if (!name || !house) continue;
        parsed.push({
          house, name,
          inspiration: get('inspiration') || 'Original',
          occ_key: get('occasion') || 'casual',
          occ_detail: get('occasion') || 'Casual / everyday',
          s_key: get('season') || 'yr',
          isBase: get('base').toLowerCase() === 'yes',
          _dna: get('dna'),
          _notes: get('notes'),
          _rating: parseInt(get('rating')) || 0,
        });
      }

      if (!parsed.length) {
        setImportStatus('No valid bottles found in CSV.', true);
        return;
      }

      pendingImport = parsed;
      showImportPreview(parsed);
    } catch(err) {
      setImportStatus('Error reading file: ' + err.message, true);
    }
  };
  reader.readAsText(file);
  input.value = '';
}

function parseCSVLine(line) {
  const result = [];
  let cur = '', inQ = false;
  for (let i = 0; i < line.length; i++) {
    const c = line[i];
    if (c === '"') {
      if (inQ && line[i+1] === '"') { cur += '"'; i++; }
      else inQ = !inQ;
    } else if (c === ',' && !inQ) {
      result.push(cur); cur = '';
    } else {
      cur += c;
    }
  }
  result.push(cur);
  return result;
}

function showImportPreview(parsed) {
  const mode = document.querySelector('input[name="import-mode"]:checked')?.value || 'replace';
  const preview = document.getElementById('import-preview');
  const content2 = document.getElementById('import-preview-content');
  
  const existing = DB.col.map(f => f.name.toLowerCase());
  const newBottles = parsed.filter(f => !existing.includes(f.name.toLowerCase()));
  const dupes = parsed.filter(f => existing.includes(f.name.toLowerCase()));

  content2.innerHTML = `
    <div style="display:flex;gap:20px;flex-wrap:wrap;margin-bottom:16px;">
      <div><div style="font-family:'Cormorant Garamond',serif;font-size:32px;color:var(--gold);font-weight:600;">${parsed.length}</div><div style="font-size:8.5px;color:var(--dove);">Bottles in CSV</div></div>
      <div><div style="font-family:'Cormorant Garamond',serif;font-size:32px;color:var(--forest);font-weight:600;">${newBottles.length}</div><div style="font-size:8.5px;color:var(--dove);">New bottles</div></div>
      ${mode==='replace'?`<div><div style="font-family:'Cormorant Garamond',serif;font-size:32px;color:var(--rose);font-weight:600;">${DB.col.length}</div><div style="font-size:8.5px;color:var(--dove);">Will be removed</div></div>`:`<div><div style="font-family:'Cormorant Garamond',serif;font-size:32px;color:var(--dove);font-weight:600;">${dupes.length}</div><div style="font-size:8.5px;color:var(--dove);">Already exist (skipped)</div></div>`}
    </div>
    <div style="font-size:9.5px;color:var(--cream);font-weight:600;margin-bottom:8px;">First 5 bottles detected:</div>
    ${parsed.slice(0,5).map(f => '<div style="padding:5px 0;border-bottom:1px solid rgba(140,100,40,.08);font-size:10px;color:var(--cream);">' + f.name + ' <span style="color:var(--gold);font-size:8.5px;">' + f.house + '</span></div>').join('')}
    ${parsed.length > 5 ? '<div style="font-size:9px;color:var(--dove);margin-top:6px;">+' + (parsed.length-5) + ' more</div>' : ''}
    <div style="margin-top:14px;padding:10px 14px;background:rgba(176,90,66,.07);border:1px solid rgba(176,90,66,.2);font-size:9.5px;color:var(--rose);">
      ${mode==='replace'?'This will REPLACE your entire current collection. Your wear logs, ratings and notes will be cleared.':'This will ADD new bottles only. Your existing data is safe.'}
    </div>
  `;

  document.getElementById('import-confirm-btn').onclick = () => confirmImport(mode);
  preview.style.display = 'block';
  preview.scrollIntoView({behavior:'smooth'});
}

function confirmImport(mode) {
  if (!pendingImport) return;
  const parsed = pendingImport;

  if (mode === 'replace') {
    DB.col = parsed.map(f => ({house:f.house, name:f.name, inspiration:f.inspiration, occ_key:f.occ_key, occ_detail:f.occ_detail, s_key:f.s_key, isBase:f.isBase}));
    DB.st = {};
    parsed.forEach(f => {
      if (f._dna || f._notes || f._rating) {
        DB.st[f.name] = {};
        if (f._dna) DB.st[f.name].dna = f._dna;
        if (f._notes) DB.st[f.name].notes = f._notes;
        if (f._rating) DB.st[f.name].rating = f._rating;
      }
    });
  } else {
    const existing = new Set(DB.col.map(f => f.name.toLowerCase()));
    parsed.forEach(f => {
      if (!existing.has(f.name.toLowerCase())) {
        DB.col.push({house:f.house, name:f.name, inspiration:f.inspiration, occ_key:f.occ_key, occ_detail:f.occ_detail, s_key:f.s_key, isBase:f.isBase});
        if (f._dna || f._notes || f._rating) {
          DB.st[f.name] = {};
          if (f._dna) DB.st[f.name].dna = f._dna;
          if (f._notes) DB.st[f.name].notes = f._notes;
          if (f._rating) DB.st[f.name].rating = f._rating;
        }
      }
    });
  }

  saveDB();
  populateHouses();
  populateSugSelect();
  renderGrid();
  updateStats();
  pendingImport = null;
  document.getElementById('import-preview').style.display = 'none';
  setImportStatus('Import successful! ' + DB.col.length + ' bottles loaded.', false);
  setTimeout(() => showPage('collection', document.querySelector('.nav-tab')), 1500);
}

function cancelImport() {
  pendingImport = null;
  document.getElementById('import-preview').style.display = 'none';
}

function setImportStatus(msg, isError) {
  const el = document.getElementById('import-status');
  if (el) {
    el.textContent = msg;
    el.style.color = isError ? 'var(--rose)' : 'var(--forest)';
  }
}

function exportBackup() {
  const backup = {
    version: 1,
    exported: new Date().toISOString(),
    col: DB.col,
    layers: DB.layers,
    st: DB.st,
    wishlist: DB.wishlist || [],
  };
  downloadFile(JSON.stringify(backup, null, 2), 'fragrance-vault-backup.json', 'application/json');
}

function importBackup(input) {
  const file = input.files[0];
  if (!file) return;
  const reader = new FileReader();
  reader.onload = function(e) {
    try {
      const backup = JSON.parse(e.target.result);
      if (!backup.col || !Array.isArray(backup.col)) throw new Error('Invalid backup file');
      if (!confirm('This will replace ALL your data including wears, ratings and notes. Are you sure?')) return;
      DB.col = backup.col;
      DB.layers = backup.layers || [];
      DB.st = backup.st || {};
      DB.wishlist = backup.wishlist || [];
      saveDB();
      populateHouses();
      populateSugSelect();
      renderGrid();
      updateStats();
      setImportStatus('Backup restored! ' + DB.col.length + ' bottles loaded.', false);
      setTimeout(() => showPage('collection', document.querySelector('.nav-tab')), 1500);
    } catch(err) {
      setImportStatus('Error: ' + err.message, true);
    }
  };
  reader.readAsText(file);
  input.value = '';
}

// ============================================================
// ============================================================
// DARK MODE
// ============================================================
function toggleDarkMode() {
  const isDark = document.documentElement.getAttribute('data-theme') === 'dark';
  const newTheme = isDark ? 'light' : 'dark';
  document.documentElement.setAttribute('data-theme', newTheme);
  localStorage.setItem('vault_theme', newTheme);
  const btn = document.getElementById('dark-toggle');
  if (btn) btn.textContent = newTheme === 'dark' ? '☽' : '☀';
}

function initTheme() {
  const saved = localStorage.getItem('vault_theme') || 'light';
  document.documentElement.setAttribute('data-theme', saved);
  const btn = document.getElementById('dark-toggle');
  if (btn) btn.textContent = saved === 'dark' ? '☽' : '☀';
}

// ============================================================
// SERVICE WORKER — offline PWA support
// ============================================================
function registerServiceWorker() {
  // Service worker requires a separate sw.js file hosted on the same origin.
  // The app works fully offline via localStorage — all data persists between sessions.
  // To enable true offline caching, host a sw.js file alongside index.html on GitHub Pages.
}

// ============================================================
// PUSH NOTIFICATIONS / ROTATION REMINDERS
// ============================================================
async function requestNotificationPermission() {
  const statusBtn = document.getElementById('notif-status');
  if (!('Notification' in window)) {
    if (statusBtn) { statusBtn.textContent = 'Notifications not supported on this device'; }
    return;
  }
  const perm = await Notification.requestPermission();
  if (perm === 'granted') {
    if (statusBtn) { statusBtn.textContent = '✓ Notifications enabled'; statusBtn.style.color = 'var(--forest)'; }
    localStorage.setItem('vault_notif', '1');
    scheduleRotationCheck();
  } else {
    if (statusBtn) { statusBtn.textContent = 'Permission denied — enable in Safari Settings'; }
  }
}

function scheduleRotationCheck() {
  // Check every time the page loads — if a frag is very overdue, show a notification
  const now = new Date();
  const overdue = DB.col.filter(f => {
    const st = gst(f.name);
    const wears = st.wears || [];
    if (!wears.length) return false;
    const last = new Date(wears[wears.length - 1]);
    const days = Math.floor((now - last) / 86400000);
    return days > 30 && (f.s_key === 'yr' || (f.s_key === 'ss' && now.getMonth() >= 3 && now.getMonth() <= 8) || (f.s_key === 'fw' && (now.getMonth() < 3 || now.getMonth() > 8)));
  }).slice(0, 3);

  if (overdue.length && Notification.permission === 'granted') {
    const names = overdue.map(f => f.name).join(', ');
    setTimeout(() => {
      new Notification('The Vault — Rotation Reminder', {
        body: 'You have not worn ' + names + ' in over 30 days. Time to rotate!',
      });
    }, 3000);
  }
}

function buildReminderBanner() {
  const banner = document.getElementById('reminder-banner');
  const listEl = document.getElementById('reminder-list');
  if (!banner || !listEl) return;

  const now = new Date();
  const month = now.getMonth();
  const isSS = month >= 3 && month <= 8;
  const currentSeason = isSS ? 'ss' : 'fw';

  // Find bottles that are seasonally appropriate but haven't been worn in 14+ days
  const reminders = DB.col.map(f => {
    const st = gst(f.name);
    const wears = st.wears || [];
    const last = wears.length ? new Date(wears[wears.length - 1]) : null;
    const days = last ? Math.floor((now - last) / 86400000) : 999;
    const relevant = f.s_key === currentSeason || f.s_key === 'yr';
    return {f, days, relevant};
  }).filter(x => x.relevant && x.days >= 14)
    .sort((a, b) => b.days - a.days)
    .slice(0, 5);

  if (!reminders.length) {
    banner.style.display = 'none';
    return;
  }

  banner.style.display = 'block';
  listEl.innerHTML = reminders.map(({f, days}) => {
    const label = days === 999 ? 'Never worn' : days + ' days ago';
    const color = days > 30 ? 'var(--rose)' : 'var(--gold-dim)';
    return '<div style="display:flex;align-items:center;justify-content:space-between;padding:6px 0;border-bottom:1px solid rgba(140,100,40,.07);">' +
      '<div><div style="font-size:10px;color:var(--cream);font-weight:600;">' + f.name + '</div>' +
      '<div style="font-size:8px;color:var(--dove);">' + f.house + '</div></div>' +
      '<div style="font-size:9px;font-weight:600;color:' + color + ';">' + label + '</div>' +
      '</div>';
  }).join('');

  // Update notification status button
  const statusBtn = document.getElementById('notif-status');
  if (statusBtn) {
    if (!('Notification' in window)) {
      statusBtn.textContent = 'Notifications unavailable';
    } else if (Notification.permission === 'granted') {
      statusBtn.textContent = '✓ Push reminders on';
      statusBtn.style.color = 'var(--forest)';
    } else if (Notification.permission === 'denied') {
      statusBtn.textContent = 'Notifications blocked — check Settings';
    } else {
      statusBtn.textContent = 'Push reminders off';
    }
  }
}

// ============================================================
// INIT
// ============================================================
initTheme();loadDB();populateHouses();populateSugSelect();populateTagFilter();renderSprayDots();renderGrid();updateStats();fetchWeather();filterQL('');setTimeout(buildMorningRec,1200);
document.addEventListener('keydown',e=>{if(e.key==='Escape'){closeDetDirect();['add-overlay','conf-overlay'].forEach(id=>document.getElementById(id).classList.add('hidden'));}});
</script>

</body>
</html>
