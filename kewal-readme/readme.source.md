```aura width=860 height=200
 <div style={{
 width: '100%', height: '100%', background: '#08080c',
 display: 'flex', alignItems: 'center', fontFamily: 'Inter',
 position: 'relative', overflow: 'hidden', borderRadius: 16,
 border: '1px solid rgba(110,80,220,0.18)'
}}>

 <style>
   {`
     @keyframes float-slow {
       0%, 100% { transform: translateX(0px); opacity: 0.8; }
       50% { transform: translateX(350px); opacity: 1.2; }
     }
     @keyframes float-medium {
       0%, 100% { transform: translateX(0px); opacity: 0.7; }
       50% { transform: translateX(-250px); opacity: 1.1; }
     }
     @keyframes float-fast {
       0%, 100% { transform: translateX(0px); opacity: 0.9; }
       50% { transform: translateX(200px); opacity: 0.6; }
     }
     @keyframes float-diagonal {
       0%, 100% { transform: translateX(0px); opacity: 0.75; }
       50% { transform: translateX(300px); opacity: 1.0; }
     }
     @keyframes float-wave {
       0%, 100% { transform: translateX(0px); opacity: 0.65; }
       33% { transform: translateX(-160px); opacity: 0.9; }
       66% { transform: translateX(80px); opacity: 1.0; }
     }
     @keyframes float-pulse {
       0%, 100% { transform: scale(1); opacity: 0.8; }
       50% { transform: scale(1.3); opacity: 0.4; }
     }
     #glow-1 { animation: float-slow 8s ease-in-out infinite; }
     #glow-2 { animation: float-medium 12s ease-in-out infinite; }
     #glow-3 { animation: float-fast 9s ease-in-out infinite; }
     #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
     #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
     #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
     #glow-7 { animation: float-wave 13s ease-in-out infinite; }
     #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
   `}
 </style>

 <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
   <defs>
     <radialGradient id="g1" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(110,20,210,0.72)" />
       <stop offset="40%" stopColor="rgba(90,15,180,0.35)" />
       <stop offset="70%" stopColor="rgba(90,15,180,0)" />
     </radialGradient>
     <radialGradient id="g2" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(40,60,255,0.6)" />
       <stop offset="45%" stopColor="rgba(30,50,200,0.25)" />
       <stop offset="70%" stopColor="rgba(30,50,200,0)" />
     </radialGradient>
     <radialGradient id="g3" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,130,255,0.45)" />
       <stop offset="50%" stopColor="rgba(0,100,220,0.18)" />
       <stop offset="70%" stopColor="rgba(0,100,220,0)" />
     </radialGradient>
     <radialGradient id="g4" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,190,230,0.32)" />
       <stop offset="70%" stopColor="rgba(0,190,230,0)" />
     </radialGradient>
     <radialGradient id="g5" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(90,30,200,0.38)" />
       <stop offset="70%" stopColor="rgba(90,30,200,0)" />
     </radialGradient>
     <radialGradient id="g6" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(160,30,255,0.55)" />
       <stop offset="45%" stopColor="rgba(130,20,220,0.22)" />
       <stop offset="70%" stopColor="rgba(130,20,220,0)" />
     </radialGradient>
     <radialGradient id="g7" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(20,60,255,0.42)" />
       <stop offset="50%" stopColor="rgba(10,40,200,0.16)" />
       <stop offset="70%" stopColor="rgba(10,40,200,0)" />
     </radialGradient>
     <radialGradient id="g8" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,170,255,0.40)" />
       <stop offset="50%" stopColor="rgba(0,130,220,0.15)" />
       <stop offset="70%" stopColor="rgba(0,130,220,0)" />
     </radialGradient>
   </defs>

   <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
   <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
   <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
   <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
   <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
   <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />
   <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />
   <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g8)" />
 </svg>

 <div style={{
   position: 'absolute', left: 48, top: 52, width: 96, height: 96,
   borderRadius: 48, background: 'linear-gradient(135deg, #6622ee, #0088ff)',
   display: 'flex', alignItems: 'center', justifyContent: 'center',
 }}>
   <img src={'data:image/jpeg;base64,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'} width={88} height={88} style={{ borderRadius: 44 }} />
 </div>

 <div style={{ display:'flex', flexDirection:'column', marginLeft:168, gap:8, zIndex: 10 }}>
   <div style={{ display:'flex', fontSize:38, fontWeight:800, color:'#ffffff', letterSpacing:'-1px', lineHeight:1 }}>
     {'Kewal'}
   </div>
   <div style={{ display:'flex', fontSize:15, color:'rgba(180,165,255,0.8)', fontWeight:400, letterSpacing:'0.3px' }}>
     {'Bioinformatics Student'}
   </div>
   <div style={{ display:'flex', gap:8, marginTop:6 }}>
     {['Python', 'SQL', 'Linux', 'Git'].map(function(tag) {
       return (
         <div key={tag} style={{
           display:'flex', padding:'4px 12px', borderRadius:20,
           background:'rgba(80,40,220,0.18)', border:'1px solid rgba(100,70,240,0.32)',
           color:'rgba(205,195,255,0.85)', fontSize:12, fontWeight:600,
         }}>{tag}</div>
       );
     })}
   </div>
 </div>
</div>
```

```aura width=860 height=224
(function() {
 var categories = [
   { title: 'Languages', color: '#a78bfa', items: ['Python', 'SQL', 'Bash'] },
   { title: 'Libraries', color: '#60a5fa', items: ['NumPy', 'Pandas', 'Matplotlib'] },
   { title: 'Tools', color: '#c084fc', items: ['Jupyter', 'Linux', 'Git', 'GitHub'] },
   { title: 'Speaks', color: '#8e8aa8', dim: true, items: ['Hindi · Native', 'English · Advanced', 'German · Beginner'] },
 ];

 return (
   <div style={{
     width: '100%', height: '100%',
     background: '#08080c',
     display: 'flex', flexDirection: 'column',
     fontFamily: 'Inter', padding: '18px 32px', gap: 14,
     borderRadius: 16, border: '1px solid rgba(110,80,220,0.18)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>
       {`
         @keyframes float-slow {
           0%, 100% { transform: translateX(0px); opacity: 0.8; }
           50% { transform: translateX(350px); opacity: 1.2; }
         }
         @keyframes float-medium {
           0%, 100% { transform: translateX(0px); opacity: 0.7; }
           50% { transform: translateX(-250px); opacity: 1.1; }
         }
         @keyframes float-fast {
           0%, 100% { transform: translateX(0px); opacity: 0.9; }
           50% { transform: translateX(200px); opacity: 0.6; }
         }
         @keyframes float-diagonal {
           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }
           50% { transform: translate(120px, 30px); opacity: 1.0; }
         }
         @keyframes float-wave {
           0%, 100% { transform: translateX(0px); opacity: 0.65; }
           33% { transform: translateX(-160px); opacity: 0.9; }
           66% { transform: translateX(80px); opacity: 1.0; }
         }
         @keyframes float-pulse {
           0%, 100% { transform: scale(1); opacity: 0.8; }
           50% { transform: scale(1.3); opacity: 0.4; }
         }
         #glow-1 { animation: float-slow 9s ease-in-out infinite; }
         #glow-2 { animation: float-medium 12s ease-in-out infinite; }
         #glow-3 { animation: float-fast 8s ease-in-out infinite; }
         #glow-4 { animation: float-diagonal 11s ease-in-out infinite reverse; }
         #glow-5 { animation: float-wave 14s ease-in-out infinite reverse; }
         #glow-6 { animation: float-pulse 6s ease-in-out infinite; }
       `}
     </style>

     <svg width="860" height="224" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="g1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(115,20,215,0.68)" />
           <stop offset="42%" stopColor="rgba(85,15,175,0.30)" />
           <stop offset="70%" stopColor="rgba(85,15,175,0)" />
         </radialGradient>
         <radialGradient id="g2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(55,55,255,0.55)" />
           <stop offset="45%" stopColor="rgba(35,45,210,0.22)" />
           <stop offset="70%" stopColor="rgba(35,45,210,0)" />
         </radialGradient>
         <radialGradient id="g3" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,130,255,0.42)" />
           <stop offset="50%" stopColor="rgba(0,100,220,0.16)" />
           <stop offset="70%" stopColor="rgba(0,100,220,0)" />
         </radialGradient>
         <radialGradient id="g4" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,185,240,0.32)" />
           <stop offset="70%" stopColor="rgba(0,185,240,0)" />
         </radialGradient>
         <radialGradient id="g5" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(100,25,205,0.42)" />
           <stop offset="70%" stopColor="rgba(100,25,205,0)" />
         </radialGradient>
         <radialGradient id="g6" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(60,80,255,0.35)" />
           <stop offset="70%" stopColor="rgba(60,80,255,0)" />
         </radialGradient>
       </defs>
       <ellipse id="glow-1" cx="170" cy="224" rx="260" ry="170" fill="url(#g1)" />
       <ellipse id="glow-2" cx="320" cy="234" rx="220" ry="140" fill="url(#g2)" />
       <ellipse id="glow-3" cx="460" cy="234" rx="190" ry="130" fill="url(#g3)" />
       <ellipse id="glow-4" cx="590" cy="244" rx="160" ry="110" fill="url(#g4)" />
       <ellipse id="glow-5" cx="750" cy="244" rx="140" ry="100" fill="url(#g5)" />
       <ellipse id="glow-6" cx="420" cy="194" rx="100" ry="80" fill="url(#g6)" />
     </svg>

     <div style={{ display:'flex', fontSize:10, fontWeight:700, color:'rgba(155,140,210,0.5)', letterSpacing:'3px' }}>
       TECH STACK
     </div>
     <div style={{ display:'flex', flexDirection:'column', gap:14 }}>
       {categories.map(function(cat) {
         return (
           <div key={cat.title} style={{ display:'flex', alignItems:'center', gap:16, marginTop: cat.dim ? 4 : 0, opacity: cat.dim ? 0.8 : 1 }}>
             <div style={{ display:'flex', fontSize:10, fontWeight:700, color:cat.color, letterSpacing:'1px', width:80 }}>
               {cat.title.toUpperCase()}
             </div>
             <div style={{ display:'flex', flexWrap:'wrap', gap:7 }}>
               {cat.items.map(function(item) {
                 return (
                   <div key={item} style={{
                     display:'flex', padding:'4px 13px', borderRadius:6,
                     background:cat.color + '15', border:'1px solid ' + cat.color + '35',
                     color:'rgba(225,220,255,0.85)', fontSize:12, fontWeight:600,
                   }}>{item}</div>
                 );
               })}
             </div>
           </div>
         );
       })}
     </div>
   </div>
 );
})()
```

```aura width=132 height=44 link="mailto:kewalxraaj@gmail.com" inline align=center
<SocialMediaButton
  icon="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iI0VBNDMzNSIgZD0iTTI0IDUuNDU3djEzLjkwOWMwIC45MDQtLjczMiAxLjYzNi0xLjYzNiAxLjYzNmgtMy44MTlWMTEuNzNMMTIgMTYuNjRsLTYuNTQ1LTQuOTF2OS4yNzNIMS42MzZBMS42MzYgMS42MzYgMCAwIDEgMCAxOS4zNjZWNS40NTdjMC0yLjAyMyAyLjMwOS0zLjE3OCAzLjkyNy0xLjk2NEw1LjQ1NSA0LjY0IDEyIDkuNTQ4bDYuNTQ1LTQuOTEgMS41MjgtMS4xNDVDMjEuNjkgMi4yOCAyNCAzLjQzNCAyNCA1LjQ1N3oiLz48L3N2Zz4="
  text="Email"
  backgroundColor="#0d0b16"
  width={132}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#a78bfa' },
    { offset: '15%', color: '#0d0b16' },
    { offset: '45%', color: '#7c3aed' },
    { offset: '60%', color: '#60a5fa' },
    { offset: '80%', color: '#0d0b16' },
    { offset: '100%', color: '#6e50dc' },
  ]}
  iconSize={22}
/>
```

<br>
<p align="center"><sub>𝗉𝗈𝗐𝖾𝗋𝖾𝖽 𝖻𝗒 <a href="https://github.com/collectioneur/readme-aura">𝗋𝖾𝖺𝖽𝗆𝖾-𝖺𝗎𝗋𝖺</a></sub></p>
