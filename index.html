import { useState, useEffect, useRef, useCallback } from "react";

// ── PALETTE LIGHT PRO ─────────────────────────────────────────────────────────
const C = {
  bg:       "#F4F6FA",
  surface:  "#FFFFFF",
  surfaceL: "#F8FAFE",
  border:   "#E2E8F2",
  borderM:  "#CBD5E8",
  text:     "#0F1A2E",
  textM:    "#4A5568",
  textL:    "#8A96A8",
  blue:     "#1A6BF0",
  blueL:    "#EBF2FF",
  blueD:    "#0F4AC4",
  accent:   "#F97316",
  accentL:  "#FFF3E8",
  green:    "#10B981",
  greenL:   "#ECFDF5",
  red:      "#EF4444",
  redL:     "#FEF2F2",
  amber:    "#F59E0B",
  amberL:   "#FFFBEB",
};

const SHOE_SIZES   = [35,35.5,36,36.5,37,37.5,38,38.5,39,39.5,40,40.5,41,41.5,42,42.5,43,43.5,44,44.5,45,45.5,46,47];
const CLOTH_SIZES  = ["XS","S","M","L","XL","XXL"];
// Tailles rapides affichées dans la barre selon catégorie
const QUICK_SHOES  = [39,39.5,40,40.5,41,41.5,42,42.5,43,44,45];
const QUICK_CLOTH  = ["XS","S","M","L","XL"];
const COLORS_PAL   = [
  {name:"Noir",   hex:"#1a1a1a"},{name:"Blanc",  hex:"#f0f0f0"},
  {name:"Rouge",  hex:"#e63946"},{name:"Bleu",   hex:"#2196f3"},
  {name:"Vert",   hex:"#10b981"},{name:"Orange", hex:"#f97316"},
  {name:"Gris",   hex:"#8a96a8"},{name:"Jaune",  hex:"#f59e0b"},
  {name:"Rose",   hex:"#f72585"},
];

const PRODUCTS = [
  { id:1, name:"Air Zoom Pegasus 41", brand:"NIKE", sport:"running", category:"Chaussures",
    price:127.50, oldPrice:149.99, rating:4.7, reviews:2341,
    isLatest:true, monthsOld:2, stockLevel:"normal", stockCount:42,
    sizes:[38,39,40,40.5,41,42,42.5,43,44,45],
    colors:["Noir","Blanc","Orange","Bleu"],
    colorHex:{"Noir":"#1a1a1a","Blanc":"#f0f0f0","Orange":"#f97316","Bleu":"#2196f3"},
    tags:["Drop 10mm","ZoomX","Mesh respirant"],
    accent:"#1A6BF0",
    img:"https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=800&q=90",
    imgAlt:"https://images.unsplash.com/photo-1595950653106-6c9ebd614d3a?w=800&q=90",
    stores:[{name:"Nike.com",price:129.99,badge:"Officiel"},{name:"Amazon",price:127.50,badge:"Meilleur prix"},{name:"Decathlon",price:134.00}],
    competitorIds:[4,5],
    pitch:"La référence du running quotidien. Amorti réactif, respirabilité maximale.",
    quote:"\"Mes pieds n'ont jamais été aussi heureux sur 42km\" — Thomas K.",
  },
  { id:2, name:"Speedcross 6 GTX", brand:"SALOMON", sport:"trail", category:"Chaussures",
    price:135.00, oldPrice:160.00, rating:4.9, reviews:1876,
    isLatest:true, monthsOld:4, stockLevel:"low", stockCount:7,
    sizes:[39,40,40.5,41,42,43,44,45],
    colors:["Noir","Bleu","Gris"],
    colorHex:{"Noir":"#1a1a1a","Bleu":"#2196f3","Gris":"#8a96a8"},
    tags:["Gore-Tex","Contagrip","Imperméable"],
    accent:"#10B981",
    img:"https://images.unsplash.com/photo-1606107557195-0e29a4b5b4aa?w=800&q=90",
    imgAlt:"https://images.unsplash.com/photo-1539185441755-769473a23570?w=800&q=90",
    stores:[{name:"Salomon",price:139.00,badge:"Officiel"},{name:"Amazon",price:135.00,badge:"Meilleur prix"},{name:"RunDiscount",price:142.00}],
    competitorIds:[],
    pitch:"Le roi des sentiers boueux. Gore-Tex intégral, grip bestial, confort trail.",
    quote:"\"Rien ne l'arrête, ni la boue ni les pierres\" — Marine L.",
  },
  { id:3, name:"Forerunner 965", brand:"GARMIN", sport:"tech", category:"Montres",
    price:344.00, oldPrice:499.00, rating:4.8, reviews:987,
    isLatest:false, monthsOld:15, stockLevel:"normal", stockCount:28,
    sizes:["S","M","L"],
    colors:["Noir","Gris","Blanc"],
    colorHex:{"Noir":"#1a1a1a","Gris":"#8a96a8","Blanc":"#f0f0f0"},
    tags:["AMOLED","GPS multi-bande","Cardio"],
    accent:"#7C3AED",
    img:"https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=800&q=90",
    imgAlt:"https://images.unsplash.com/photo-1508685096489-7aacd43bd3b1?w=800&q=90",
    stores:[{name:"Garmin",price:349.00,badge:"Officiel"},{name:"Amazon",price:344.00,badge:"Meilleur prix"},{name:"Fnac",price:359.00}],
    competitorIds:[],
    pitch:"L'outil ultime du coureur sérieux. AMOLED, maps, récupération IA.",
    quote:"\"Ma montre me connaît mieux que mon coach\" — Julien M.",
  },
  { id:4, name:"Clifton 9", brand:"HOKA", sport:"running", category:"Chaussures",
    price:155.00, oldPrice:null, rating:4.6, reviews:1203,
    isLatest:true, monthsOld:1, stockLevel:"normal", stockCount:63,
    sizes:[38,39,40,41,42,43,44,45,46],
    colors:["Blanc","Orange","Bleu","Noir"],
    colorHex:{"Blanc":"#f0f0f0","Orange":"#f97316","Bleu":"#2196f3","Noir":"#1a1a1a"},
    tags:["Maximaliste","Récupération","Drop 5mm"],
    accent:"#F97316",
    img:"https://images.unsplash.com/photo-1600185365483-26d7a4cc7519?w=800&q=90",
    imgAlt:"https://images.unsplash.com/photo-1556048219-bb6978360b84?w=800&q=90",
    stores:[{name:"Hoka",price:159.95,badge:"Officiel"},{name:"Amazon",price:155.00,badge:"Meilleur prix"},{name:"Running Expert",price:162.00}],
    competitorIds:[1,5],
    pitch:"Le nuage sous les pieds. Amorti maximaliste pour longues sorties.",
    quote:"\"Mes douleurs aux genoux ont disparu\" — Claire D.",
  },
  { id:5, name:"Gel-Nimbus 26", brand:"ASICS", sport:"running", category:"Chaussures",
    price:175.00, oldPrice:200.00, rating:4.5, reviews:654,
    isLatest:true, monthsOld:2, stockLevel:"normal", stockCount:31,
    sizes:[39,40,40.5,41,42,42.5,43,44,45],
    colors:["Bleu","Noir","Vert","Gris"],
    colorHex:{"Bleu":"#2196f3","Noir":"#1a1a1a","Vert":"#10b981","Gris":"#8a96a8"},
    tags:["PureGEL","Drop 10mm","Longues distances"],
    accent:"#10B981",
    img:"https://images.unsplash.com/photo-1491553895911-0055eca6402d?w=800&q=90",
    imgAlt:"https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=800&q=90",
    stores:[{name:"Asics",price:179.95,badge:"Officiel"},{name:"Amazon",price:175.00,badge:"Meilleur prix"},{name:"Intersport",price:185.00}],
    competitorIds:[1,4],
    pitch:"La technologie GEL à son summum. Confort légendaire, ultra-distances.",
    quote:"\"Le seul modèle sur lequel je coure mes 100km\" — Antoine R.",
  },
  { id:6, name:"Vest Hydratation 8L", brand:"NATHAN", sport:"trail", category:"Accessoires",
    price:87.00, oldPrice:null, rating:4.4, reviews:432,
    isLatest:false, monthsOld:11, stockLevel:"normal", stockCount:19,
    sizes:["S","M","L","XL"],
    colors:["Noir","Vert","Orange","Bleu"],
    colorHex:{"Noir":"#1a1a1a","Vert":"#10b981","Orange":"#f97316","Bleu":"#2196f3"},
    tags:["8 litres","Flasks 500ml","Unisexe"],
    accent:"#1A6BF0",
    img:"https://images.unsplash.com/photo-1551698618-1dfe5d97d256?w=800&q=90",
    imgAlt:"https://images.unsplash.com/photo-1527719327859-c6ce80353573?w=800&q=90",
    stores:[{name:"Nathan",price:89.99,badge:"Officiel"},{name:"Amazon",price:87.00,badge:"Meilleur prix"},{name:"Decathlon",price:94.00}],
    competitorIds:[],
    pitch:"Légèreté et praticité pour trails de longue haleine. Flasks inclus.",
    quote:"\"Elle ne bouge pas d'un millimètre sur terrain technique\" — Sara P.",
  },
];

const INTENT_KW = {
  race_prep:["marathon","semi","10km","5km","préparer","compétition","chrono","objectif","course"],
  running:["running","run","jogging","courir","chaussure","pegasus","clifton","nimbus"],
  trail:["trail","montagne","sentier","speedcross","salomon"],
  tech:["montre","gps","garmin","cardio","forerunner"],
};

function computeScore(p, intents=[]) {
  let fresh = p.monthsOld<=3?25:p.monthsOld<=8?18:p.monthsOld<=14?10:4;
  const drop = p.oldPrice?(p.oldPrice-p.price)/p.oldPrice:0;
  let price = drop>=0.15?25:drop>=0.08?19:drop>0?13:8;
  if(p.stockLevel==="low") price=Math.min(25,price+4);
  const quality = Math.round(Math.min(25,((p.rating-3.5)/1.5)*15+Math.min(10,Math.log10(p.reviews+1)*3.3)));
  let rel=10;
  if(intents.includes("running")&&p.sport==="running") rel+=10;
  if(intents.includes("trail")&&p.sport==="trail") rel+=10;
  if(intents.includes("tech")&&p.category==="Montres") rel+=10;
  if(intents.includes("race_prep")&&["running","trail"].includes(p.sport)) rel+=5;
  return {total:fresh+price+quality+Math.min(25,rel),fresh,price,quality,relevance:Math.min(25,rel)};
}

function sColor(s){return s>=80?C.green:s>=65?C.blue:s>=50?C.amber:C.red;}
function sBg(s){return s>=80?C.greenL:s>=65?C.blueL:s>=50?C.amberL:C.redL;}
function sLabel(s){return s>=80?"Excellent":s>=65?"Bon achat":s>=50?"Passable":"À éviter";}
function sEmoji(s){return s>=80?"🔥":s>=65?"✅":s>=50?"⚠️":"❌";}

// ── Anneau SVG ─────────────────────────────────────────────────────────────────
function Ring({score,size=60,sw=5}){
  const [v,setV]=useState(0);
  const r=(size-sw*2)/2, circ=2*Math.PI*r, col=sColor(v);
  useEffect(()=>{
    let s=null;
    const go=ts=>{if(!s)s=ts;const p=Math.min((ts-s)/850,1),e=1-Math.pow(1-p,3);setV(Math.round(e*score));if(p<1)requestAnimationFrame(go);};
    requestAnimationFrame(go);
  },[score]);
  return(
    <div style={{position:"relative",width:size,height:size,flexShrink:0}}>
      <svg width={size} height={size} style={{transform:"rotate(-90deg)"}}>
        <circle cx={size/2} cy={size/2} r={r} fill="none" stroke={C.border} strokeWidth={sw}/>
        <circle cx={size/2} cy={size/2} r={r} fill="none" stroke={col} strokeWidth={sw}
          strokeLinecap="round" strokeDasharray={`${(v/100)*circ} ${circ}`} style={{transition:"stroke 0.3s"}}/>
      </svg>
      <div style={{position:"absolute",inset:0,display:"flex",flexDirection:"column",alignItems:"center",justifyContent:"center"}}>
        <span style={{color:col,fontFamily:"'DM Mono',monospace",fontWeight:700,fontSize:size>55?15:11,lineHeight:1}}>{v}</span>
        <span style={{color:C.textL,fontSize:7,lineHeight:1,marginTop:1}}>/100</span>
      </div>
    </div>
  );
}

// ── Barre sous-score ──────────────────────────────────────────────────────────
function Bar({label,icon,value,max=25,color}){
  const [w,setW]=useState(0);
  useEffect(()=>{setTimeout(()=>setW((value/max)*100),100);},[value,max]);
  return(
    <div style={{marginBottom:8}}>
      <div style={{display:"flex",justifyContent:"space-between",marginBottom:3}}>
        <span style={{color:C.textL,fontSize:10}}>{icon} {label}</span>
        <span style={{color,fontSize:10,fontWeight:700}}>{value}/{max}</span>
      </div>
      <div style={{height:4,background:C.border,borderRadius:4,overflow:"hidden"}}>
        <div style={{height:"100%",width:`${w}%`,background:color,borderRadius:4,transition:"width 0.85s cubic-bezier(.22,1,.36,1)"}}/>
      </div>
    </div>
  );
}

// ── Filtre taille étendu ──────────────────────────────────────────────────────
function SizeDrawer({selectedSizes,onToggle,category}){
  // Affiche uniquement les tailles pertinentes selon la catégorie sélectionnée
  const showShoes  = category === "Chaussures" || category === "Tous";
  const showCloth  = category === "Accessoires" || category === "Montres" || category === "Tous";

  return(
    <div style={{display:"flex",flexDirection:"column",gap:16,padding:4}}>
      {showShoes && (
        <div>
          <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:10}}>
            Pointure — toutes les tailles
          </div>
          {/* Grouper par entier pour la lisibilité */}
          {[35,36,37,38,39,40,41,42,43,44,45,46,47].map(base => {
            const half = base + 0.5;
            const hasHalf = SHOE_SIZES.includes(half) && half < 47;
            return (
              <div key={base} style={{display:"flex",gap:5,marginBottom:6}}>
                {/* Entier */}
                {SHOE_SIZES.includes(base) && (()=>{const a=selectedSizes.includes(base);return(
                  <button onClick={()=>onToggle(base)} style={{width:52,height:34,borderRadius:8,border:`1.5px solid ${a?C.blue:C.border}`,background:a?C.blue:"#fff",color:a?"#fff":C.textM,fontFamily:"'DM Mono',monospace",fontWeight:600,fontSize:12,cursor:"pointer",transition:"all 0.13s"}}>{base}</button>
                );})()}
                {/* Demi-pointure */}
                {hasHalf && (()=>{const a=selectedSizes.includes(half);return(
                  <button onClick={()=>onToggle(half)} style={{width:52,height:34,borderRadius:8,border:`1.5px solid ${a?C.blue:C.border}`,background:a?C.blue:C.surfaceL,color:a?"#fff":C.textL,fontFamily:"'DM Mono',monospace",fontWeight:600,fontSize:11,cursor:"pointer",transition:"all 0.13s",borderStyle:"dashed"}}>{half}</button>
                );})()}
              </div>
            );
          })}
        </div>
      )}
      {showCloth && (
        <div>
          <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:10}}>
            Taille vêtement / accessoire
          </div>
          <div style={{display:"flex",gap:6,flexWrap:"wrap"}}>
            {CLOTH_SIZES.map(sz=>{const a=selectedSizes.includes(sz);return(
              <button key={sz} onClick={()=>onToggle(sz)} style={{padding:"0 18px",height:36,borderRadius:8,border:`1.5px solid ${a?C.blue:C.border}`,background:a?C.blue:"#fff",color:a?"#fff":C.textM,fontWeight:700,fontSize:13,cursor:"pointer",transition:"all 0.14s"}}>{sz}</button>
            );})}
          </div>
        </div>
      )}
      {!showShoes && !showCloth && (
        <div style={{color:C.textL,fontSize:13,padding:"8px 0"}}>Sélectionnez une catégorie pour voir les tailles disponibles.</div>
      )}
    </div>
  );
}

// ── Panneau filtres avancés ───────────────────────────────────────────────────
function AdvPanel({filters,onChange,onReset,count}){
  const [open,setOpen]=useState(false);
  const ref=useRef(null);
  useEffect(()=>{
    const h=e=>{if(ref.current&&!ref.current.contains(e.target))setOpen(false);};
    if(open)document.addEventListener("mousedown",h);
    return()=>document.removeEventListener("mousedown",h);
  },[open]);

  return(
    <div ref={ref} style={{position:"relative"}}>
      <button onClick={()=>setOpen(v=>!v)} style={{
        display:"flex",alignItems:"center",gap:8,
        background:count>0?C.blueL:"#fff",
        border:`1.5px solid ${count>0?C.blue:C.border}`,
        color:count>0?C.blue:C.textM,
        fontWeight:700,fontSize:13,padding:"8px 16px",borderRadius:10,cursor:"pointer",transition:"all 0.18s"
      }}>
        <span>⚙ Filtres</span>
        {count>0&&<span style={{background:C.blue,color:"#fff",borderRadius:"50%",width:18,height:18,fontSize:10,fontWeight:900,display:"flex",alignItems:"center",justifyContent:"center"}}>{count}</span>}
        <span style={{fontSize:9,opacity:.5}}>{open?"▲":"▼"}</span>
      </button>

      {open&&(
        <div style={{
          position:"absolute",top:"calc(100% + 8px)",right:0,zIndex:400,
          background:"#fff",border:`1px solid ${C.border}`,borderRadius:18,
          padding:24,width:400,
          boxShadow:"0 20px 60px rgba(15,26,46,0.12), 0 4px 16px rgba(15,26,46,0.06)",
          animation:"fadeDown .2s ease"
        }}>
          <div style={{display:"flex",justifyContent:"space-between",alignItems:"center",marginBottom:20}}>
            <span style={{fontWeight:800,fontSize:16,color:C.text}}>Filtres avancés</span>
            <button onClick={onReset} style={{background:"none",border:"none",color:C.textL,fontSize:12,cursor:"pointer",fontWeight:600}}>Réinitialiser</button>
          </div>

          {/* Couleurs */}
          <div style={{marginBottom:20}}>
            <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:12}}>Couleur</div>
            <div style={{display:"flex",flexWrap:"wrap",gap:8}}>
              {COLORS_PAL.map(c=>{const a=filters.colors.includes(c.name);return(
                <button key={c.name} onClick={()=>onChange("colors",c.name)} style={{
                  display:"flex",alignItems:"center",gap:7,
                  background:a?C.blueL:"#fff",border:`1.5px solid ${a?C.blue:C.border}`,
                  borderRadius:9,padding:"6px 11px",cursor:"pointer",transition:"all 0.14s"
                }}>
                  <div style={{width:14,height:14,borderRadius:"50%",background:c.hex,border:c.name==="Blanc"?"1px solid #ccc":"none",outline:a?`2px solid ${C.blue}`:"none",outlineOffset:1}}/>
                  <span style={{color:a?C.blue:C.textM,fontSize:12,fontWeight:600}}>{c.name}</span>
                </button>
              );})}
            </div>
          </div>

          {/* Prix */}
          <div style={{marginBottom:20}}>
            <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:12}}>Budget</div>
            <div style={{display:"flex",alignItems:"center",gap:10,marginBottom:10}}>
              {["priceMin","priceMax"].map((key,i)=>(
                <div key={key} style={{flex:1,position:"relative"}}>
                  <span style={{position:"absolute",left:10,top:"50%",transform:"translateY(-50%)",color:C.textL,fontSize:13}}>€</span>
                  <input type="number" placeholder={i===0?"Min":"Max"} value={filters[key]}
                    onChange={e=>onChange(key,e.target.value)}
                    style={{width:"100%",border:`1.5px solid ${C.border}`,borderRadius:9,padding:"9px 9px 9px 26px",fontSize:14,fontWeight:600,color:C.text,outline:"none",background:"#fff",fontFamily:"'DM Mono',monospace"}}
                    onFocus={e=>e.target.style.borderColor=C.blue} onBlur={e=>e.target.style.borderColor=C.border}/>
                </div>
              ))}
            </div>
            <div style={{display:"flex",gap:6,flexWrap:"wrap"}}>
              {[{l:"< 100€",mn:"",mx:"100"},{l:"100–200€",mn:"100",mx:"200"},{l:"200–400€",mn:"200",mx:"400"},{l:"400€+",mn:"400",mx:""}].map(r=>{
                const a=filters.priceMin===r.mn&&filters.priceMax===r.mx;
                return <button key={r.l} onClick={()=>{onChange("priceMin",r.mn);onChange("priceMax",r.mx);}} style={{background:a?C.blueL:"#fff",border:`1.5px solid ${a?C.blue:C.border}`,color:a?C.blue:C.textM,fontSize:11,fontWeight:700,padding:"5px 12px",borderRadius:20,cursor:"pointer"}}>{r.l}</button>;
              })}
            </div>
          </div>

          {/* Toggles */}
          <div style={{marginBottom:20}}>
            <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:12}}>Options</div>
            {[{k:"promoOnly",l:"En promotion uniquement",i:"🏷️"},{k:"inStockOnly",l:"En stock uniquement",i:"📦"},{k:"newOnly",l:"Nouvelles sorties uniquement",i:"✦"}].map(opt=>(
              <label key={opt.k} style={{display:"flex",alignItems:"center",gap:12,cursor:"pointer",marginBottom:12}}>
                <div onClick={()=>onChange(opt.k,!filters[opt.k])} style={{width:42,height:22,borderRadius:11,background:filters[opt.k]?C.blue:C.border,position:"relative",transition:"background .2s",flexShrink:0}}>
                  <div style={{position:"absolute",top:2,left:filters[opt.k]?20:2,width:18,height:18,borderRadius:"50%",background:"#fff",transition:"left .2s",boxShadow:"0 1px 4px rgba(0,0,0,0.2)"}}/>
                </div>
                <span style={{color:C.textM,fontSize:13}}>{opt.i} {opt.l}</span>
              </label>
            ))}
          </div>

          {/* Score min */}
          <div>
            <div style={{display:"flex",justifyContent:"space-between",alignItems:"center",marginBottom:10}}>
              <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase"}}>Score IA minimum</div>
              <span style={{color:sColor(filters.minScore),fontWeight:800,fontSize:15,fontFamily:"'DM Mono',monospace"}}>{filters.minScore}/100</span>
            </div>
            <input type="range" min="0" max="90" step="5" value={filters.minScore}
              onChange={e=>onChange("minScore",parseInt(e.target.value))}
              style={{width:"100%",cursor:"pointer"}}/>
            <div style={{display:"flex",justifyContent:"space-between",marginTop:6}}>
              {["Tous","Passable","Bon","Excellent"].map((l,i)=>(
                <span key={l} style={{color:C.textL,fontSize:9}}>{l}</span>
              ))}
            </div>
          </div>
        </div>
      )}
    </div>
  );
}

// ── Carte produit ─────────────────────────────────────────────────────────────
function ProductCard({p,intents,all,onOpen,selectedSizes}){
  const [sc,setSc]=useState(null);
  const [hov,setHov]=useState(false);
  const [loaded,setLoaded]=useState(false);
  const saving=p.oldPrice?Math.round((1-p.price/p.oldPrice)*100):null;
  const best=Math.min(...p.stores.map(s=>s.price));
  const bestStore=p.stores.find(s=>s.price===best);
  const sizeOk=selectedSizes.length===0||selectedSizes.some(sz=>p.sizes.includes(sz));
  const lowSc=sc&&sc.total<55;

  useEffect(()=>{const t=setTimeout(()=>setSc(computeScore(p,intents)),300+p.id*90);return()=>clearTimeout(t);},[p,intents]);

  return(
    <div onClick={()=>sc&&onOpen(p,sc)} style={{
      background:C.surface,borderRadius:20,overflow:"hidden",cursor:"pointer",
      border:`1.5px solid ${sc?sColor(sc.total)+"28":C.border}`,
      transition:"all 0.28s cubic-bezier(.22,1,.36,1)",
      opacity:sizeOk?1:0.45,
      boxShadow:"0 1px 4px rgba(15,26,46,0.06)"
    }}
      onMouseEnter={e=>{if(sizeOk){e.currentTarget.style.transform="translateY(-4px)";e.currentTarget.style.boxShadow=`0 12px 36px rgba(15,26,46,0.12), 0 0 0 2px ${sc?sColor(sc.total)+"30":C.blue+"20"}`;setHov(true);}}}
      onMouseLeave={e=>{e.currentTarget.style.transform="none";e.currentTarget.style.boxShadow="0 1px 4px rgba(15,26,46,0.06)";setHov(false);}}>

      {/* IMAGE */}
      <div style={{position:"relative",height:240,overflow:"hidden",background:C.surfaceL}}>
        <img src={hov?p.imgAlt:p.img} alt={p.name} onLoad={()=>setLoaded(true)} style={{
          width:"100%",height:"100%",objectFit:"cover",
          transition:"transform 0.55s cubic-bezier(.22,1,.36,1), opacity 0.35s",
          transform:hov?"scale(1.06)":"scale(1)", opacity:loaded?1:0
        }}/>

        {/* Overlay léger bas */}
        <div style={{position:"absolute",inset:0,background:"linear-gradient(to top,rgba(244,246,250,0.9) 0%,transparent 45%)"}}/>

        {/* Badges haut-gauche */}
        <div style={{position:"absolute",top:12,left:12,display:"flex",flexDirection:"column",gap:5}}>
          {p.isLatest&&<span style={{background:C.blue,color:"#fff",fontSize:10,fontWeight:700,padding:"3px 10px",borderRadius:20,letterSpacing:.5}}>Nouveau</span>}
          {saving&&<span style={{background:C.accent,color:"#fff",fontSize:10,fontWeight:700,padding:"3px 10px",borderRadius:20}}>-{saving}%</span>}
          {p.stockLevel==="low"&&<span style={{background:C.red,color:"#fff",fontSize:10,fontWeight:700,padding:"3px 10px",borderRadius:20}}>⚡ {p.stockCount} restants</span>}
        </div>

        {/* Score haut-droite */}
        <div style={{position:"absolute",top:12,right:12}}>
          {sc?(
            <div style={{background:"rgba(255,255,255,0.96)",backdropFilter:"blur(8px)",borderRadius:14,padding:"9px 11px",border:`1.5px solid ${sColor(sc.total)}28`,boxShadow:"0 2px 12px rgba(15,26,46,0.1)",display:"flex",flexDirection:"column",alignItems:"center",gap:3}}>
              <Ring score={sc.total} size={50} sw={4}/>
              <span style={{color:sColor(sc.total),fontSize:8,fontWeight:800,letterSpacing:.8}}>{sLabel(sc.total).toUpperCase()}</span>
            </div>
          ):(
            <div style={{background:"rgba(255,255,255,0.9)",borderRadius:12,padding:12,border:`1px solid ${C.border}`,display:"flex",gap:3}}>
              {[0,1,2].map(i=><div key={i} style={{width:5,height:5,borderRadius:"50%",background:C.border,animation:"pulse 1s infinite",animationDelay:`${i*.2}s`}}/>)}
            </div>
          )}
        </div>

        {/* Indicateurs taille sur image */}
        {selectedSizes.length>0&&(
          <div style={{position:"absolute",bottom:10,left:10,display:"flex",gap:5}}>
            {selectedSizes.filter(sz=>p.sizes.includes(sz)).slice(0,3).map(sz=>(
              <span key={sz} style={{background:C.green,color:"#fff",fontSize:10,fontWeight:800,padding:"2px 8px",borderRadius:8}}>{sz} ✓</span>
            ))}
            {selectedSizes.filter(sz=>!p.sizes.includes(sz)).slice(0,1).map(sz=>(
              <span key={sz} style={{background:C.red,color:"#fff",fontSize:10,fontWeight:800,padding:"2px 8px",borderRadius:8}}>{sz} ✗</span>
            ))}
          </div>
        )}
      </div>

      {/* CORPS */}
      <div style={{padding:"16px 18px 18px"}}>
        {/* Marque + nom */}
        <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.5,textTransform:"uppercase",marginBottom:3}}>{p.brand}</div>
        <h3 style={{fontWeight:800,fontSize:17,color:C.text,margin:"0 0 6px",lineHeight:1.2}}>{p.name}</h3>
        <p style={{color:C.textL,fontSize:12,margin:"0 0 12px",lineHeight:1.55}}>{p.pitch}</p>

        {/* Couleurs */}
        <div style={{display:"flex",gap:6,alignItems:"center",marginBottom:12}}>
          {p.colors.map(c=>(
            <div key={c} title={c} style={{width:15,height:15,borderRadius:"50%",background:p.colorHex[c],border:`1.5px solid ${C.border}`,boxShadow:"0 1px 3px rgba(15,26,46,0.1)"}}/>
          ))}
          <span style={{color:C.textL,fontSize:10,marginLeft:2}}>{p.colors.length} coloris</span>
        </div>

        {/* Tags */}
        <div style={{display:"flex",gap:5,flexWrap:"wrap",marginBottom:12}}>
          {p.tags.map(t=><span key={t} style={{background:C.surfaceL,border:`1px solid ${C.border}`,color:C.textM,fontSize:10,padding:"2px 9px",borderRadius:20}}>{t}</span>)}
        </div>

        {/* Étoiles */}
        <div style={{display:"flex",alignItems:"center",gap:6,marginBottom:8}}>
          <div style={{display:"flex",gap:2}}>
            {[1,2,3,4,5].map(i=>(
              <svg key={i} width="12" height="12" viewBox="0 0 24 24" fill={i<=Math.round(p.rating)?C.amber:C.border}>
                <polygon points="12,2 15.09,8.26 22,9.27 17,14.14 18.18,21.02 12,17.77 5.82,21.02 7,14.14 2,9.27 8.91,8.26"/>
              </svg>
            ))}
          </div>
          <span style={{color:C.textM,fontSize:11,fontWeight:600}}>{p.rating}</span>
          <span style={{color:C.textL,fontSize:11}}>({p.reviews.toLocaleString()} avis)</span>
        </div>

        {/* Citation */}
        <div style={{background:C.surfaceL,border:`1px solid ${C.border}`,borderLeft:`3px solid ${p.accent}`,borderRadius:"0 8px 8px 0",padding:"8px 12px",marginBottom:14}}>
          <p style={{color:C.textM,fontSize:11,margin:0,fontStyle:"italic",lineHeight:1.5}}>{p.quote}</p>
        </div>

        <div style={{height:1,background:C.border,marginBottom:14}}/>

        {/* Prix + CTA */}
        <div style={{display:"flex",justifyContent:"space-between",alignItems:"flex-end"}}>
          <div>
            <div style={{display:"flex",alignItems:"baseline",gap:8}}>
              <span style={{fontFamily:"'DM Mono',monospace",fontWeight:700,fontSize:26,color:C.text,lineHeight:1}}>{best.toFixed(2)}€</span>
              {p.oldPrice&&<span style={{color:C.textL,fontSize:13,textDecoration:"line-through"}}>{p.oldPrice}€</span>}
            </div>
            <div style={{color:C.textL,fontSize:10,marginTop:2}}>
              {bestStore?.badge&&<span style={{background:C.greenL,color:C.green,fontWeight:700,padding:"1px 6px",borderRadius:10,marginRight:4,fontSize:9}}>{bestStore.badge}</span>}
              {bestStore?.name}
            </div>
          </div>
          <button onClick={e=>{e.stopPropagation();sc&&onOpen(p,sc);}} style={{
            background:C.blue,border:"none",color:"#fff",
            fontWeight:700,fontSize:13,padding:"10px 18px",borderRadius:11,
            cursor:"pointer",transition:"all 0.18s",whiteSpace:"nowrap",
            boxShadow:`0 4px 14px ${C.blue}40`
          }}
            onMouseEnter={e=>{e.currentTarget.style.background=C.blueD;e.currentTarget.style.transform="scale(1.04)";}}
            onMouseLeave={e=>{e.currentTarget.style.background=C.blue;e.currentTarget.style.transform="scale(1)";}}>
            Analyser →
          </button>
        </div>

        {/* Alerte alternative */}
        {lowSc&&(()=>{
          const alt=all.filter(x=>x.id!==p.id&&x.category===p.category)
            .map(x=>({...x,sc:computeScore(x,intents).total}))
            .filter(x=>x.sc>sc.total+10).sort((a,b)=>b.sc-a.sc)[0];
          return alt?(
            <div style={{marginTop:12,background:C.amberL,border:`1px solid ${C.amber}40`,borderRadius:10,padding:"10px 12px",display:"flex",gap:10,alignItems:"center"}}>
              <span style={{fontSize:18,flexShrink:0}}>💡</span>
              <div>
                <div style={{color:C.amber,fontSize:10,fontWeight:700,marginBottom:1}}>Meilleure option disponible</div>
                <div style={{color:C.textM,fontSize:11}}>{alt.name} · Score {alt.sc}/100 · {alt.price}€</div>
              </div>
            </div>
          ):null;
        })()}
      </div>
    </div>
  );
}

// ── Modale analyse ────────────────────────────────────────────────────────────
function Modal({p,sc,intents,all,onClose}){
  const [ai,setAi]=useState(null);
  const [loading,setLoading]=useState(true);
  const col=sColor(sc.total);
  const bg=sBg(sc.total);

  useEffect(()=>{
    (async()=>{
      try{
        const comps=all.filter(x=>p.competitorIds.includes(x.id));
        const res=await fetch("/api/chat",{method:"POST",headers:{"Content-Type":"application/json"},body:JSON.stringify({model:"claude-sonnet-4-20250514",max_tokens:900,
          system:`Expert équipement sportif. Réponds UNIQUEMENT en JSON valide sans markdown.
{"verdict":"string","buySignal":"ACHETER MAINTENANT"|"ATTENDRE"|"CHERCHER MIEUX","buyReason":"string max 15 mots","priceNote":"string","freshnessNote":"string","bestStore":"string","bestPrice":number,"alternatives":[{"name":"string","price":number,"advantage":"string"}],"addons":[{"name":"string","why":"string"}],"tip":"string max 20 mots"}`,
          messages:[{role:"user",content:`Produit: ${p.name} (${p.brand}), ${p.price}€${p.oldPrice?` (était ${p.oldPrice}€)`:""}. Sorti il y a ${p.monthsOld} mois. Note: ${p.rating}/5 (${p.reviews} avis). Stock: ${p.stockLevel} (${p.stockCount} unités). Tailles: ${p.sizes.join(", ")}. Couleurs: ${p.colors.join(", ")}. Offres: ${p.stores.map(s=>`${s.name} ${s.price}€`).join(", ")}. Concurrents: ${comps.map(x=>`${x.name} ${x.price}€ note${x.rating}`).join(", ")||"aucun"}. Profil: ${intents.join(", ")||"généraliste"}. Score: ${sc.total}/100.`}]})});
        const d=await res.json();
        setAi(JSON.parse((d.content?.find(b=>b.type==="text")?.text||"{}").replace(/```json|```/g,"").trim()));
      }catch{
        const bp=p.stores.sort((a,b)=>a.price-b.price)[0];
        setAi({verdict:"Très bon produit avec excellent rapport qualité-prix.",buySignal:sc.total>=65?"ACHETER MAINTENANT":sc.total>=50?"ATTENDRE":"CHERCHER MIEUX",buyReason:"Score IA favorable",priceNote:p.oldPrice?`-${Math.round((1-p.price/p.oldPrice)*100)}% vs prix conseillé`:"Prix stable",freshnessNote:p.monthsOld<=4?"Modèle très récent":`${p.monthsOld} mois sur le marché`,bestStore:bp.name,bestPrice:bp.price,alternatives:[],addons:[],tip:"Vérifiez les tailles disponibles avant l'achat."});
      }
      setLoading(false);
    })();
  },[]);

  const sigBg=ai?.buySignal==="ACHETER MAINTENANT"?C.greenL:ai?.buySignal==="ATTENDRE"?C.amberL:C.redL;
  const sigCol=ai?.buySignal==="ACHETER MAINTENANT"?C.green:ai?.buySignal==="ATTENDRE"?C.amber:C.red;

  return(
    <div onClick={onClose} style={{position:"fixed",inset:0,background:"rgba(15,26,46,0.55)",zIndex:700,display:"flex",alignItems:"center",justifyContent:"center",padding:20,backdropFilter:"blur(6px)"}}>
      <div onClick={e=>e.stopPropagation()} style={{
        background:"#fff",borderRadius:24,maxWidth:540,width:"100%",maxHeight:"90vh",
        overflowY:"auto",boxShadow:"0 32px 80px rgba(15,26,46,0.2), 0 0 0 1px rgba(15,26,46,0.08)"
      }}>
        {/* Image hero */}
        <div style={{position:"relative",height:200,overflow:"hidden",borderRadius:"24px 24px 0 0",background:C.surfaceL}}>
          <img src={p.img} alt={p.name} style={{width:"100%",height:"100%",objectFit:"cover"}}/>
          <div style={{position:"absolute",inset:0,background:"linear-gradient(to top,#fff,transparent 50%)"}}/>
          <button onClick={onClose} style={{position:"absolute",top:14,right:14,width:34,height:34,borderRadius:"50%",background:"rgba(255,255,255,0.92)",border:`1px solid ${C.border}`,color:C.textM,fontSize:18,cursor:"pointer",display:"flex",alignItems:"center",justifyContent:"center",boxShadow:"0 2px 8px rgba(15,26,46,0.1)"}}>×</button>
          <div style={{position:"absolute",bottom:14,left:18}}>
            <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.5,textTransform:"uppercase"}}>{p.brand}</div>
            <div style={{fontWeight:800,fontSize:20,color:C.text,lineHeight:1.1}}>{p.name}</div>
          </div>
        </div>

        <div style={{padding:"22px 24px 28px"}}>
          {/* Score bloc */}
          <div style={{display:"flex",gap:16,alignItems:"center",background:bg,border:`1.5px solid ${col}28`,borderRadius:16,padding:"15px 18px",marginBottom:18}}>
            <Ring score={sc.total} size={80} sw={6}/>
            <div style={{flex:1}}>
              <div style={{fontWeight:800,fontSize:18,color:col,marginBottom:10}}>{sEmoji(sc.total)} {sLabel(sc.total)}</div>
              <Bar label="Fraîcheur" icon="🗓️" value={sc.fresh} color="#7C3AED"/>
              <Bar label="Signal prix" icon="💰" value={sc.price} color={C.blue}/>
              <Bar label="Qualité & avis" icon="⭐" value={sc.quality} color={C.amber}/>
              <Bar label="Pertinence" icon="🎯" value={sc.relevance} color={C.green}/>
            </div>
          </div>

          {/* Tailles + coloris */}
          <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:10,marginBottom:18}}>
            <div style={{background:C.surfaceL,border:`1px solid ${C.border}`,borderRadius:12,padding:"12px 14px"}}>
              <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:8}}>Tailles disponibles</div>
              <div style={{display:"flex",flexWrap:"wrap",gap:4}}>
                {p.sizes.slice(0,8).map(sz=><span key={sz} style={{background:"#fff",border:`1px solid ${C.border}`,color:C.textM,fontSize:10,padding:"2px 7px",borderRadius:6,fontFamily:"'DM Mono',monospace",fontWeight:600}}>{sz}</span>)}
                {p.sizes.length>8&&<span style={{color:C.textL,fontSize:10}}>+{p.sizes.length-8}</span>}
              </div>
            </div>
            <div style={{background:C.surfaceL,border:`1px solid ${C.border}`,borderRadius:12,padding:"12px 14px"}}>
              <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:8}}>Coloris</div>
              <div style={{display:"flex",gap:7,flexWrap:"wrap",alignItems:"center"}}>
                {p.colors.map(c=><div key={c} title={c} style={{width:20,height:20,borderRadius:"50%",background:p.colorHex[c],border:`1.5px solid ${C.border}`,boxShadow:"0 1px 4px rgba(15,26,46,0.1)"}}/>)}
              </div>
            </div>
          </div>

          {loading?(
            <div style={{textAlign:"center",padding:32}}>
              <div style={{display:"inline-flex",gap:6,marginBottom:10}}>{[0,1,2].map(i=><div key={i} style={{width:8,height:8,borderRadius:"50%",background:C.blue,animation:"bounce 1s infinite",animationDelay:`${i*.2}s`}}/>)}</div>
              <div style={{color:C.textL,fontSize:13}}>Analyse IA en cours...</div>
            </div>
          ):ai&&(<>
            {/* Signal achat */}
            <div style={{background:sigBg,border:`1.5px solid ${sigCol}30`,borderRadius:14,padding:"14px 18px",marginBottom:14,display:"flex",justifyContent:"space-between",alignItems:"center"}}>
              <div>
                <div style={{color:sigCol,fontWeight:800,fontSize:18}}>{ai.buySignal}</div>
                <div style={{color:C.textM,fontSize:12,marginTop:2}}>{ai.buyReason}</div>
              </div>
              <span style={{fontSize:28}}>{ai.buySignal==="ACHETER MAINTENANT"?"🛒":ai.buySignal==="ATTENDRE"?"⏳":"🔄"}</span>
            </div>

            {/* Verdict */}
            <div style={{background:C.surfaceL,border:`1px solid ${C.border}`,borderLeft:`3px solid ${C.blue}`,borderRadius:"0 12px 12px 0",padding:"12px 16px",marginBottom:14}}>
              <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:5}}>Verdict</div>
              <p style={{color:C.textM,fontSize:13,margin:0,fontStyle:"italic",lineHeight:1.65}}>"{ai.verdict}"</p>
            </div>

            {/* Comparatif prix */}
            <div style={{marginBottom:14}}>
              <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:10}}>Comparer les prix</div>
              {p.stores.map(s=>{
                const isBest=s.price===Math.min(...p.stores.map(x=>x.price));
                return(
                  <div key={s.name} style={{display:"flex",justifyContent:"space-between",alignItems:"center",padding:"11px 14px",marginBottom:8,borderRadius:12,background:isBest?C.blueL:"#fff",border:`1.5px solid ${isBest?C.blue+"40":C.border}`}}>
                    <div style={{display:"flex",alignItems:"center",gap:8}}>
                      {isBest&&<span style={{background:C.green,color:"#fff",fontSize:9,fontWeight:800,padding:"2px 8px",borderRadius:10}}>MEILLEUR PRIX</span>}
                      <span style={{color:C.textM,fontSize:13,fontWeight:isBest?700:400}}>{s.name}</span>
                    </div>
                    <div style={{display:"flex",alignItems:"center",gap:10}}>
                      <span style={{color:isBest?C.blue:C.text,fontFamily:"'DM Mono',monospace",fontWeight:700,fontSize:17}}>{s.price}€</span>
                      <button style={{background:isBest?C.blue:"#fff",border:`1px solid ${C.border}`,color:isBest?"#fff":C.textM,fontSize:11,fontWeight:700,padding:"6px 13px",borderRadius:8,cursor:"pointer"}}>Acheter →</button>
                    </div>
                  </div>
                );
              })}
            </div>

            {/* Grille infos */}
            <div style={{display:"grid",gridTemplateColumns:"1fr 1fr",gap:8,marginBottom:14}}>
              {[{l:"Prix",v:ai.priceNote,i:"📉",c:C.blue},{l:"Fraîcheur",v:ai.freshnessNote,i:"🗓️",c:"#7C3AED"},{l:"Astuce",v:ai.tip,i:"💡",c:C.amber},{l:"Stock",v:`${p.stockCount} unités · ${p.stockLevel==="low"?"⚡ Critique":"Disponible"}`,i:"📦",c:p.stockLevel==="low"?C.red:C.green}].map((x,i)=>(
                <div key={i} style={{background:C.surfaceL,border:`1px solid ${C.border}`,borderRadius:10,padding:"11px 13px"}}>
                  <div style={{color:C.textL,fontSize:10,marginBottom:4}}>{x.i} {x.l}</div>
                  <div style={{color:C.textM,fontSize:11,lineHeight:1.5}}>{x.v}</div>
                </div>
              ))}
            </div>

            {ai.alternatives?.length>0&&(
              <div style={{marginBottom:14}}>
                <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:10}}>Alternatives</div>
                {ai.alternatives.map((a,i)=>(
                  <div key={i} style={{background:"#F5F3FF",border:"1px solid #7C3AED28",borderRadius:10,padding:"10px 14px",marginBottom:8,display:"flex",justifyContent:"space-between",alignItems:"center"}}>
                    <div><div style={{color:C.text,fontSize:13,fontWeight:600,marginBottom:2}}>{a.name}</div><div style={{color:C.textM,fontSize:11}}>{a.advantage}</div></div>
                    <span style={{color:C.blue,fontFamily:"'DM Mono',monospace",fontWeight:700,fontSize:16}}>{a.price}€</span>
                  </div>
                ))}
              </div>
            )}

            {ai.addons?.length>0&&(
              <div>
                <div style={{color:C.textL,fontSize:10,fontWeight:700,letterSpacing:1.2,textTransform:"uppercase",marginBottom:10}}>À associer</div>
                {ai.addons.map((a,i)=>(
                  <div key={i} style={{background:C.amberL,border:`1px solid ${C.amber}30`,borderRadius:10,padding:"10px 14px",marginBottom:8,display:"flex",gap:10,alignItems:"center"}}>
                    <span style={{fontSize:18}}>🛍️</span>
                    <div><div style={{color:C.text,fontSize:13,fontWeight:600}}>{a.name}</div><div style={{color:C.textM,fontSize:11}}>{a.why}</div></div>
                  </div>
                ))}
              </div>
            )}
          </>)}
        </div>
      </div>
    </div>
  );
}

// ── Chat ──────────────────────────────────────────────────────────────────────
function Chat({onIntent,onClose}){
  const [msgs,setMsgs]=useState([{role:"assistant",text:"Bonjour ! 👋 Dites-moi votre sport, objectif ou pointure — j'adapte les scores en temps réel !"}]);
  const [input,setInput]=useState(""); const [loading,setLoading]=useState(false);
  const endRef=useRef(null);
  useEffect(()=>{endRef.current?.scrollIntoView({behavior:"smooth"});},[msgs]);
  async function send(){
    if(!input.trim()||loading)return;
    const msg=input.trim();setInput("");
    const nm=[...msgs,{role:"user",text:msg}];setMsgs(nm);setLoading(true);
    const lower=msg.toLowerCase();const found=[];
    Object.entries(INTENT_KW).forEach(([k,ws])=>{if(ws.some(w=>lower.includes(w)))found.push(k);});
    if(found.length)onIntent(found);
    try{
      const res=await fetch("/api/chat",{method:"POST",headers:{"Content-Type":"application/json"},body:JSON.stringify({model:"claude-sonnet-4-20250514",max_tokens:700,system:"Conseiller sport expert. Concis (3 phrases max), bienveillant, précis, français.",messages:nm.map(m=>({role:m.role==="assistant"?"assistant":"user",content:m.text}))})});
      const d=await res.json();
      const text=d.content?.find(b=>b.type==="text")?.text||"Réessayez !";
      setMsgs(p=>[...p,{role:"assistant",text}]);
      const al=[];Object.entries(INTENT_KW).forEach(([k,ws])=>{if(ws.some(w=>text.toLowerCase().includes(w)))al.push(k);});
      if(al.length)onIntent(al);
    }catch{setMsgs(p=>[...p,{role:"assistant",text:"Erreur réseau. Réessayez !"}]);}
    setLoading(false);
  }
  return(
    <div style={{position:"fixed",right:24,bottom:88,width:350,height:460,zIndex:500,background:"#fff",border:`1px solid ${C.border}`,borderRadius:20,display:"flex",flexDirection:"column",boxShadow:"0 20px 60px rgba(15,26,46,0.15)"}}>
      <div style={{padding:"14px 18px",borderBottom:`1px solid ${C.border}`,display:"flex",justifyContent:"space-between",alignItems:"center",background:C.blueL,borderRadius:"20px 20px 0 0"}}>
        <div style={{display:"flex",gap:10,alignItems:"center"}}>
          <div style={{width:32,height:32,borderRadius:9,background:C.blue,display:"flex",alignItems:"center",justifyContent:"center",fontSize:15}}>🤖</div>
          <div>
            <div style={{fontWeight:800,fontSize:14,color:C.text}}>Conseiller IA Sport</div>
            <div style={{color:C.textL,fontSize:10}}>Scores adaptés à votre profil</div>
          </div>
        </div>
        <button onClick={onClose} style={{background:"none",border:"none",color:C.textL,cursor:"pointer",fontSize:20}}>×</button>
      </div>
      <div style={{flex:1,overflowY:"auto",padding:14,display:"flex",flexDirection:"column",gap:10,background:C.surfaceL}}>
        {msgs.map((m,i)=>(
          <div key={i} style={{display:"flex",justifyContent:m.role==="user"?"flex-end":"flex-start"}}>
            <div style={{maxWidth:"82%",padding:"10px 14px",fontSize:13,lineHeight:1.6,borderRadius:m.role==="user"?"18px 18px 4px 18px":"18px 18px 18px 4px",background:m.role==="user"?C.blue:C.surface,color:m.role==="user"?"#fff":C.text,border:m.role==="assistant"?`1px solid ${C.border}`:"none",boxShadow:m.role==="assistant"?"0 1px 4px rgba(15,26,46,0.06)":"none"}}>{m.text}</div>
          </div>
        ))}
        {loading&&<div style={{display:"flex",gap:5,padding:"10px 14px",background:C.surface,borderRadius:"18px 18px 18px 4px",width:"fit-content",border:`1px solid ${C.border}`}}>{[0,1,2].map(i=><div key={i} style={{width:6,height:6,borderRadius:"50%",background:C.blue,animation:"bounce 1s infinite",animationDelay:`${i*.2}s`}}/>)}</div>}
        <div ref={endRef}/>
      </div>
      <div style={{padding:"10px 14px",borderTop:`1px solid ${C.border}`,display:"flex",gap:8,background:"#fff",borderRadius:"0 0 20px 20px"}}>
        <input value={input} onChange={e=>setInput(e.target.value)} onKeyDown={e=>e.key==="Enter"&&send()} placeholder="Pointure, couleur, sport..." style={{flex:1,background:C.surfaceL,border:`1.5px solid ${C.border}`,borderRadius:12,padding:"10px 14px",color:C.text,fontSize:13,outline:"none",fontFamily:"inherit"}} onFocus={e=>e.target.style.borderColor=C.blue} onBlur={e=>e.target.style.borderColor=C.border}/>
        <button onClick={send} disabled={loading} style={{background:loading?C.border:C.blue,border:"none",color:"#fff",fontWeight:700,fontSize:16,width:42,height:42,borderRadius:12,cursor:loading?"not-allowed":"pointer"}}>→</button>
      </div>
    </div>
  );
}

// ── APP ───────────────────────────────────────────────────────────────────────
export default function App(){
  const [search,setSearch]=useState("");
  const [intents,setIntents]=useState([]);
  const [chatOpen,setChatOpen]=useState(false);
  const [modal,setModal]=useState(null);
  const [category,setCategory]=useState("Tous");
  const [sort,setSort]=useState("score");
  const [selectedSizes,setSelectedSizes]=useState([]);
  const [showAllSizes,setShowAllSizes]=useState(false);
  const [advFilters,setAdvFilters]=useState({colors:[],priceMin:"",priceMax:"",promoOnly:false,inStockOnly:false,newOnly:false,minScore:0});
  const sizeRef=useRef(null);

  const addIntents=useCallback(arr=>setIntents(p=>[...new Set([...p,...arr])]),[]);
  const toggleSize=useCallback(sz=>setSelectedSizes(p=>p.includes(sz)?p.filter(x=>x!==sz):[...p,sz]),[]);
  // Vider les tailles sélectionnées quand on change de catégorie
  const handleCategory = useCallback((cat) => {
    setCategory(cat);
    setSelectedSizes([]);
  }, []);
  const changeAdv=useCallback((key,val)=>setAdvFilters(p=>{
    if(key==="colors"){const c=p.colors;return{...p,colors:c.includes(val)?c.filter(x=>x!==val):[...c,val]};}
    return{...p,[key]:val};
  }),[]);
  const resetAdv=useCallback(()=>setAdvFilters({colors:[],priceMin:"",priceMax:"",promoOnly:false,inStockOnly:false,newOnly:false,minScore:0}),[]);

  useEffect(()=>{
    const h=e=>{if(sizeRef.current&&!sizeRef.current.contains(e.target))setShowAllSizes(false);};
    if(showAllSizes)document.addEventListener("mousedown",h);
    return()=>document.removeEventListener("mousedown",h);
  },[showAllSizes]);

  const advCount=[advFilters.colors.length>0,advFilters.priceMin||advFilters.priceMax,advFilters.promoOnly,advFilters.inStockOnly,advFilters.newOnly,advFilters.minScore>0].filter(Boolean).length;
  const onSearch=v=>{setSearch(v);const lower=v.toLowerCase();const found=[];Object.entries(INTENT_KW).forEach(([k,ws])=>{if(ws.some(w=>lower.includes(w)))found.push(k);});if(found.length)addIntents(found);};
  const CATS=["Tous","Chaussures","Montres","Accessoires"];
  // Tailles rapides affichées selon catégorie active
  const showQuickShoes = category === "Chaussures" || category === "Tous";
  const showQuickCloth = category === "Montres" || category === "Accessoires" || category === "Tous";

  const filtered=[...PRODUCTS].filter(p=>{
    const s=search.toLowerCase();
    if(category!=="Tous"&&p.category!==category)return false;
    if(s&&!p.name.toLowerCase().includes(s)&&!p.brand.toLowerCase().includes(s)&&!p.sport.includes(s))return false;
    if(selectedSizes.length>0&&!selectedSizes.some(sz=>p.sizes.includes(sz)))return false;
    if(advFilters.colors.length>0&&!advFilters.colors.some(c=>p.colors.includes(c)))return false;
    if(advFilters.priceMin&&p.price<parseFloat(advFilters.priceMin))return false;
    if(advFilters.priceMax&&p.price>parseFloat(advFilters.priceMax))return false;
    if(advFilters.promoOnly&&!p.oldPrice)return false;
    if(advFilters.inStockOnly&&p.stockLevel==="out")return false;
    if(advFilters.newOnly&&!p.isLatest)return false;
    if(advFilters.minScore>0&&computeScore(p,intents).total<advFilters.minScore)return false;
    return true;
  }).sort((a,b)=>sort==="score"?computeScore(b,intents).total-computeScore(a,intents).total:sort==="price"?a.price-b.price:b.rating-a.rating);

  return(
    <div style={{minHeight:"100vh",background:C.bg,fontFamily:"'DM Sans',sans-serif",color:C.text}}>
      <style>{`
        @import url('https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700;800&family=DM+Mono:wght@500;600;700&display=swap');
        *{box-sizing:border-box;margin:0;padding:0;}
        ::-webkit-scrollbar{width:5px;}::-webkit-scrollbar-thumb{background:${C.borderM};border-radius:5px;}
        @keyframes bounce{0%,80%,100%{transform:translateY(0)}40%{transform:translateY(-5px)}}
        @keyframes pulse{0%,100%{opacity:1}50%{opacity:0.3}}
        @keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:none}}
        @keyframes fadeDown{from{opacity:0;transform:translateY(-10px)}to{opacity:1;transform:none}}
        input[type=range]{-webkit-appearance:none;background:${C.border};height:4px;border-radius:4px;outline:none;width:100%;}
        input[type=range]::-webkit-slider-thumb{-webkit-appearance:none;width:18px;height:18px;border-radius:50%;background:${C.blue};cursor:pointer;box-shadow:0 2px 8px ${C.blue}50;}
        input[type=number]::-webkit-inner-spin-button{display:none;}
        input[type=number]{-moz-appearance:textfield;}
      `}</style>

      {/* ── HEADER ── */}
      <header style={{position:"sticky",top:0,zIndex:200,background:"rgba(255,255,255,0.95)",backdropFilter:"blur(16px)",borderBottom:`1px solid ${C.border}`,boxShadow:"0 1px 8px rgba(15,26,46,0.06)"}}>
        <div style={{maxWidth:1400,margin:"0 auto",padding:"0 28px",height:60,display:"flex",alignItems:"center",gap:20}}>
          <div style={{display:"flex",alignItems:"center",gap:9,flexShrink:0}}>
            <div style={{width:34,height:34,borderRadius:9,background:C.blue,display:"flex",alignItems:"center",justifyContent:"center",fontSize:18,fontWeight:900}}>⚡</div>
            <span style={{fontWeight:800,fontSize:20,color:C.text}}>Sport<span style={{color:C.blue}}>Compare</span></span>
          </div>
          <div style={{flex:1,maxWidth:420,position:"relative"}}>
            <input value={search} onChange={e=>onSearch(e.target.value)} placeholder="Nike, trail, marathon, pointure 42..."
              style={{width:"100%",background:C.surfaceL,border:`1.5px solid ${C.border}`,borderRadius:12,padding:"9px 38px 9px 14px",color:C.text,fontSize:14,outline:"none",fontFamily:"inherit"}}
              onFocus={e=>e.target.style.borderColor=C.blue} onBlur={e=>e.target.style.borderColor=C.border}/>
            <span style={{position:"absolute",right:12,top:"50%",transform:"translateY(-50%)",color:C.textL,fontSize:15}}>🔍</span>
          </div>
          <div style={{display:"flex",gap:14,alignItems:"center",marginLeft:"auto"}}>
            {[{c:C.green,l:"Excellent"},{c:C.blue,l:"Bon achat"},{c:C.amber,l:"Passable"},{c:C.red,l:"À éviter"}].map(x=>(
              <div key={x.l} style={{display:"flex",alignItems:"center",gap:5}}>
                <div style={{width:7,height:7,borderRadius:"50%",background:x.c}}/>
                <span style={{color:C.textL,fontSize:11,fontWeight:500}}>{x.l}</span>
              </div>
            ))}
          </div>
        </div>
      </header>

      {/* ── HERO ── */}
      <div style={{background:`linear-gradient(135deg,${C.blueL} 0%,#fff 60%,${C.surfaceL} 100%)`,borderBottom:`1px solid ${C.border}`,padding:"44px 28px 36px"}}>
        <div style={{maxWidth:1400,margin:"0 auto",display:"flex",justifyContent:"space-between",alignItems:"center",gap:32,flexWrap:"wrap"}}>
          <div>
            <div style={{display:"inline-flex",alignItems:"center",gap:6,background:C.blueL,border:`1px solid ${C.blue}28`,color:C.blue,fontSize:11,fontWeight:700,letterSpacing:1.5,padding:"5px 14px",borderRadius:20,marginBottom:14}}>⚡ SCORE IA SUR CHAQUE PRODUIT</div>
            <h1 style={{fontWeight:900,fontSize:"clamp(28px,4vw,52px)",color:C.text,lineHeight:1.1,letterSpacing:-1.5,marginBottom:10}}>
              Trouvez votre taille.<br/><span style={{color:C.blue}}>Au meilleur prix.</span>
            </h1>
            <p style={{color:C.textM,fontSize:15,maxWidth:440,lineHeight:1.65}}>Filtrez par pointure ou taille, comparez les prix sur tous les sites, et laissez l'IA noter chaque produit pour décider au bon moment.</p>
          </div>
          <div style={{display:"flex",gap:20,flexWrap:"wrap"}}>
            {[{v:"6",l:"produits analysés",c:C.blueL,bc:C.blue},{v:"3",l:"marchands comparés",c:C.greenL,bc:C.green},{v:"4",l:"critères IA",c:C.amberL,bc:C.amber},{v:"0€",l:"coût pour vous",c:C.blueL,bc:C.blue}].map((s,i)=>(
              <div key={i} style={{background:s.c,border:`1.5px solid ${s.bc}28`,borderRadius:16,padding:"16px 20px",textAlign:"center",minWidth:100}}>
                <div style={{fontFamily:"'DM Mono',monospace",fontWeight:700,fontSize:28,color:s.bc,lineHeight:1}}>{s.v}</div>
                <div style={{color:C.textM,fontSize:10,fontWeight:600,marginTop:4,letterSpacing:.5}}>{s.l}</div>
              </div>
            ))}
          </div>
        </div>
      </div>

      {/* ── BARRE FILTRES STICKY ── */}
      <div style={{position:"sticky",top:60,zIndex:150,background:"rgba(255,255,255,0.97)",backdropFilter:"blur(12px)",borderBottom:`1px solid ${C.border}`,boxShadow:"0 2px 8px rgba(15,26,46,0.05)"}}>
        <div style={{maxWidth:1400,margin:"0 auto",padding:"12px 28px",display:"flex",flexDirection:"column",gap:10}}>

          {/* Ligne principale */}
          <div style={{display:"flex",alignItems:"center",gap:8,flexWrap:"wrap"}}>
            {/* Catégories */}
            <div style={{display:"flex",gap:5}}>
              {CATS.map(c=>(
                <button key={c} onClick={()=>handleCategory(c)} style={{background:category===c?C.blue:C.surface,border:`1.5px solid ${category===c?C.blue:C.border}`,color:category===c?"#fff":C.textM,fontWeight:700,fontSize:12,padding:"6px 14px",borderRadius:9,cursor:"pointer",transition:"all 0.15s"}}>{c}</button>
              ))}
            </div>

            <div style={{width:1,height:22,background:C.border,margin:"0 4px"}}/>

            {/* === FILTRE RAPIDE TAILLE === */}
            <div style={{display:"flex",alignItems:"center",gap:5,flex:1,flexWrap:"wrap"}}>
              <span style={{color:C.textL,fontSize:11,fontWeight:700,letterSpacing:1,whiteSpace:"nowrap"}}>
                {category === "Chaussures" ? "POINTURE :" : category === "Tous" ? "TAILLE / POINTURE :" : "TAILLE :"}
              </span>

              {/* Pointures rapides — seulement si catégorie chaussures ou tous */}
              {showQuickShoes && QUICK_SHOES.map(sz=>{const a=selectedSizes.includes(sz);return(
                <button key={sz} onClick={()=>toggleSize(sz)} style={{
                  minWidth: sz % 1 !== 0 ? 46 : 40, height:32, borderRadius:8,
                  background:a?C.blue:C.surface, border:`1.5px solid ${a?C.blue:C.border}`,
                  color:a?"#fff":sz % 1 !== 0 ? C.textL : C.textM,
                  fontFamily:"'DM Mono',monospace", fontWeight:600,
                  fontSize: sz % 1 !== 0 ? 11 : 12,
                  cursor:"pointer", transition:"all 0.13s", transform:a?"scale(1.07)":"scale(1)",
                  boxShadow:a?`0 2px 10px ${C.blue}40`:"none",
                  borderStyle: sz % 1 !== 0 ? "dashed" : "solid",
                }}>{sz}</button>
              );})}

              {/* Tailles textile — seulement si catégorie vêtement/accessoire ou tous */}
              {showQuickCloth && QUICK_CLOTH.map(sz=>{const a=selectedSizes.includes(sz);return(
                <button key={sz} onClick={()=>toggleSize(sz)} style={{
                  padding:"0 12px", height:32, borderRadius:8,
                  background:a?C.blue:C.surface, border:`1.5px solid ${a?C.blue:C.border}`,
                  color:a?"#fff":C.textM, fontWeight:700, fontSize:12,
                  cursor:"pointer", transition:"all 0.13s", transform:a?"scale(1.07)":"scale(1)",
                  boxShadow:a?`0 2px 10px ${C.blue}40`:"none",
                }}>{sz}</button>
              );})}

              {/* Bouton "Toutes les tailles" */}
              <div ref={sizeRef} style={{position:"relative"}}>
                <button onClick={()=>setShowAllSizes(v=>!v)} style={{
                  display:"flex",alignItems:"center",gap:5,
                  background:showAllSizes?C.blueL:C.surface,border:`1.5px solid ${showAllSizes?C.blue:C.border}`,
                  color:showAllSizes?C.blue:C.textM,fontWeight:700,fontSize:12,
                  padding:"0 12px",height:32,borderRadius:8,cursor:"pointer",whiteSpace:"nowrap"
                }}>+ Toutes <span style={{fontSize:9,opacity:.6}}>{showAllSizes?"▲":"▼"}</span></button>

                {showAllSizes&&(
                  <div style={{position:"absolute",top:"calc(100% + 6px)",left:0,zIndex:300,background:"#fff",border:`1px solid ${C.border}`,borderRadius:16,padding:18,width:340,boxShadow:"0 16px 48px rgba(15,26,46,0.14)",animation:"fadeDown .18s ease"}}>
                    <SizeDrawer selectedSizes={selectedSizes} onToggle={toggleSize} category={category}/>
                  </div>
                )}
              </div>

              {/* Effacer tailles */}
              {selectedSizes.length>0&&(
                <button onClick={()=>setSelectedSizes([])} style={{display:"flex",alignItems:"center",gap:4,background:C.blueL,border:`1px solid ${C.blue}30`,color:C.blue,fontWeight:700,fontSize:11,padding:"0 10px",height:30,borderRadius:8,cursor:"pointer"}}>
                  ✕ {selectedSizes.slice(0,3).join(", ")}{selectedSizes.length>3?` +${selectedSizes.length-3}`:""}
                </button>
              )}
            </div>

            {/* Tri + Filtres avancés */}
            <div style={{marginLeft:"auto",display:"flex",gap:8,alignItems:"center",flexShrink:0}}>
              <select value={sort} onChange={e=>setSort(e.target.value)} style={{background:C.surface,border:`1.5px solid ${C.border}`,color:C.textM,padding:"7px 12px",borderRadius:9,fontSize:12,cursor:"pointer",fontFamily:"inherit",outline:"none",fontWeight:600}}>
                <option value="score">Score IA ↓</option>
                <option value="price">Prix ↑</option>
                <option value="rating">Avis ↓</option>
              </select>
              <AdvPanel filters={advFilters} onChange={changeAdv} onReset={resetAdv} count={advCount}/>
            </div>
          </div>

          {/* Résumé filtres actifs */}
          {(selectedSizes.length>0||advCount>0||intents.length>0)&&(
            <div style={{display:"flex",gap:6,alignItems:"center",flexWrap:"wrap",paddingTop:4}}>
              <span style={{color:C.textL,fontSize:11,fontWeight:600}}>Filtres actifs :</span>
              {selectedSizes.map(sz=><span key={sz} style={{background:C.blueL,border:`1px solid ${C.blue}28`,color:C.blue,fontSize:10,fontWeight:700,padding:"2px 9px",borderRadius:20,fontFamily:"'DM Mono',monospace"}}>{sz}</span>)}
              {advFilters.colors.map(c=>{const col=COLORS_PAL.find(x=>x.name===c);return(
                <span key={c} style={{display:"flex",alignItems:"center",gap:4,background:C.surfaceL,border:`1px solid ${C.border}`,color:C.textM,fontSize:10,fontWeight:600,padding:"2px 9px",borderRadius:20}}>
                  <div style={{width:8,height:8,borderRadius:"50%",background:col?.hex}}/>{c}
                </span>
              );})}
              {(advFilters.priceMin||advFilters.priceMax)&&<span style={{background:C.surfaceL,border:`1px solid ${C.border}`,color:C.textM,fontSize:10,fontWeight:600,padding:"2px 9px",borderRadius:20,fontFamily:"'DM Mono',monospace"}}>{advFilters.priceMin||"0"}€ – {advFilters.priceMax||"∞"}€</span>}
              {advFilters.promoOnly&&<span style={{background:C.accentL,border:`1px solid ${C.accent}28`,color:C.accent,fontSize:10,fontWeight:700,padding:"2px 9px",borderRadius:20}}>🏷️ Promos</span>}
              {advFilters.newOnly&&<span style={{background:C.blueL,border:`1px solid ${C.blue}28`,color:C.blue,fontSize:10,fontWeight:700,padding:"2px 9px",borderRadius:20}}>✦ Nouveautés</span>}
              {advFilters.minScore>0&&<span style={{background:sBg(advFilters.minScore),border:`1px solid ${sColor(advFilters.minScore)}28`,color:sColor(advFilters.minScore),fontSize:10,fontWeight:700,padding:"2px 9px",borderRadius:20}}>Score ≥ {advFilters.minScore}</span>}
              {intents.map(i=><span key={i} style={{background:C.blueL,border:`1px solid ${C.blue}28`,color:C.blue,fontSize:10,fontWeight:600,padding:"2px 9px",borderRadius:20}}>{i==="race_prep"?"🏁 Course":i==="trail"?"⛰️ Trail":i==="running"?"🏃 Running":"⌚ Tech"}</span>)}
              <span style={{color:C.textL,fontSize:11,marginLeft:4}}>{filtered.length} résultat{filtered.length>1?"s":""}</span>
              <button onClick={()=>{setSelectedSizes([]);resetAdv();setSearch("");setIntents([]);}} style={{background:"none",border:"none",color:C.textL,fontSize:11,cursor:"pointer",textDecoration:"underline",marginLeft:4}}>Tout effacer</button>
            </div>
          )}
        </div>
      </div>

      {/* ── GRILLE ── */}
      <main style={{maxWidth:1400,margin:"0 auto",padding:"32px 28px 100px"}}>
        {filtered.length===0?(
          <div style={{textAlign:"center",padding:"80px 0"}}>
            <div style={{fontSize:52,marginBottom:14}}>🔍</div>
            <div style={{fontWeight:800,fontSize:22,color:C.textM,marginBottom:8}}>Aucun résultat</div>
            <div style={{color:C.textL,fontSize:14,marginBottom:20}}>Essayez d'autres tailles ou ajustez vos filtres</div>
            <button onClick={()=>{setSelectedSizes([]);resetAdv();setSearch("");}} style={{background:C.blue,border:"none",color:"#fff",fontWeight:700,fontSize:14,padding:"11px 24px",borderRadius:12,cursor:"pointer"}}>Réinitialiser</button>
          </div>
        ):(
          <div style={{display:"grid",gridTemplateColumns:"repeat(auto-fill,minmax(300px,1fr))",gap:22}}>
            {filtered.map((p,i)=>(
              <div key={p.id} style={{animation:`fadeUp .45s ease ${i*.07}s both`}}>
                <ProductCard p={p} intents={intents} all={PRODUCTS} onOpen={(prod,sc)=>setModal({p:prod,sc})} selectedSizes={selectedSizes}/>
              </div>
            ))}
          </div>
        )}
      </main>

      {/* ── FAB ── */}
      <div style={{position:"fixed",right:24,bottom:24,zIndex:400}}>
        <button onClick={()=>setChatOpen(v=>!v)} style={{
          display:"flex",alignItems:"center",gap:10,background:C.blue,
          border:"none",borderRadius:18,padding:"13px 20px",cursor:"pointer",
          boxShadow:`0 8px 28px ${C.blue}50`,transition:"all 0.22s"
        }}
          onMouseEnter={e=>{e.currentTarget.style.background=C.blueD;e.currentTarget.style.transform="translateY(-2px)";}}
          onMouseLeave={e=>{e.currentTarget.style.background=C.blue;e.currentTarget.style.transform="none";}}>
          <span style={{fontSize:18}}>{chatOpen?"✕":"🤖"}</span>
          {!chatOpen&&<div>
            <div style={{color:"#fff",fontWeight:800,fontSize:13,lineHeight:1}}>Conseiller IA</div>
            <div style={{color:"rgba(255,255,255,0.6)",fontSize:10,marginTop:1}}>Scores personnalisés</div>
          </div>}
        </button>
      </div>

      {chatOpen&&<Chat onIntent={addIntents} onClose={()=>setChatOpen(false)}/>}
      {modal&&<Modal p={modal.p} sc={modal.sc} intents={intents} all={PRODUCTS} onClose={()=>setModal(null)}/>}
    </div>
  );
}
