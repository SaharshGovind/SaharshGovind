# Saharsh Govind

```aura width=860 height=200
<div style={{
 width:'100%',height:'100%',background:'#08080c',
 display:'flex',alignItems:'center',fontFamily:'Inter,sans-serif',
 position:'relative',overflow:'hidden',borderRadius:16,
 border:'1px solid rgba(110,80,220,0.25)'
}}>
 <style>{`
 @keyframes drift{0%,100%{transform:translateX(0);opacity:.6}50%{transform:translateX(150px);opacity:1}}
 @keyframes pulse{0%,100%{transform:scale(1);opacity:.5}50%{transform:scale(1.25);opacity:1}}
 #glow1{animation:drift 9s ease-in-out infinite}
 #glow2{animation:drift 12s ease-in-out infinite reverse}
 #glow3{animation:pulse 7s ease-in-out infinite}
 `}</style>
 <svg width="860" height="200" style={{position:'absolute',top:0,left:0}}>
  <defs>
   <radialGradient id="purple"><stop offset="0%" stopColor="rgba(120,40,255,.65)"/><stop offset="100%" stopColor="rgba(120,40,255,0)"/></radialGradient>
   <radialGradient id="blue"><stop offset="0%" stopColor="rgba(0,130,255,.55)"/><stop offset="100%" stopColor="rgba(0,130,255,0)"/></radialGradient>
  </defs>
  <ellipse id="glow1" cx="180" cy="190" rx="280" ry="180" fill="url(#purple)"/>
  <ellipse id="glow2" cx="650" cy="190" rx="300" ry="180" fill="url(#blue)"/>
  <ellipse id="glow3" cx="430" cy="180" rx="220" ry="140" fill="url(#purple)"/>
 </svg>
 <div style={{
  position:'absolute',left:38,top:52,width:96,height:96,
  borderRadius:50,background:'linear-gradient(135deg,#7928ca,#0088ff)',
  display:'flex',alignItems:'center',justifyContent:'center',padding:4
 }}>
  <img src={github.user.avatarUrl} width={88} height={88} style={{borderRadius:50}}/>
 </div>
 <div style={{display:'flex',flexDirection:'column',marginLeft:155,gap:10,zIndex:2}}>
  <div style={{display:'flex',fontSize:36,fontWeight:800,color:'#fff',letterSpacing:'-1px',lineHeight:1.1}}>
   {github.user.name || 'Saharsh Govind'}
  </div>
  <div style={{display:'flex',fontSize:14,color:'#b8a5ff',fontWeight:500}}>
   B.Tech CSE Student · Developer · Problem Solver
  </div>
  <div style={{display:'flex',gap:7,marginTop:5,flexWrap:'wrap'}}>
   {['C++','Java','Python','DSA','Backend Development','SQL'].map(function(tag){
    return <div key={tag} style={{
     display:'flex',padding:'5px 10px',borderRadius:20,
     background:'rgba(110,70,240,.15)',
     border:'1px solid rgba(140,100,255,.35)',
     color:'#ded3ff',fontSize:11,fontWeight:600
    }}>{tag}</div>;
   })}
  </div>
 </div>
</div>
```

## About Me

- 🎓 B.Tech Computer Science Engineering student.
- 💻 Interested in software development, problem-solving, and backend development.
- 🧠 Practicing Data Structures and Algorithms using C++.
- 🌱 Learning Java, Python, databases, and backend technologies.
- 🛠️ Building academic projects and improving my development skills.
- 🎯 Goal: Become a skilled software developer and build useful real-world applications.

## GitHub Statistics

```aura width=860 height=140
(function() {
 var stats = [
  {label:'Repositories',value:String(github.stats.totalRepos),color:'#a78bfa'},
  {label:'Stars',value:String(github.stats.totalStars),color:'#60a5fa'},
  {label:'Commits',value:String(github.stats.totalCommits),color:'#f59e0b'}
 ];
 return (
  <div style={{
   width:'100%',height:'100%',background:'#08080c',
   display:'flex',alignItems:'center',justifyContent:'center',
   fontFamily:'Inter,sans-serif',borderRadius:16,
   border:'1px solid rgba(110,80,220,.25)',
   position:'relative',overflow:'hidden'
  }}>
   <style>{`
    @keyframes glow{0%,100%{opacity:.35;transform:translateX(0)}50%{opacity:.9;transform:translateX(100px)}}
    #statGlow{animation:glow 9s ease-in-out infinite}
   `}</style>
   <svg width="860" height="140" style={{position:'absolute',top:0,left:0}}>
    <defs>
     <radialGradient id="statGradient">
      <stop offset="0%" stopColor="rgba(110,40,255,.55)"/>
      <stop offset="100%" stopColor="rgba(110,40,255,0)"/>
     </radialGradient>
    </defs>
    <ellipse id="statGlow" cx="400" cy="140" rx="350" ry="140" fill="url(#statGradient)"/>
   </svg>
   {stats.map(function(s,i){
    return <div key={s.label} style={{
     flex:1,display:'flex',flexDirection:'column',
     alignItems:'center',justifyContent:'center',
     padding:'16px 8px',
     borderRight:i<stats.length-1?'1px solid rgba(255,255,255,.08)':'none',
     gap:8,zIndex:1
    }}>
     <div style={{display:'flex',fontSize:30,fontWeight:800,color:s.color,lineHeight:1}}>{s.value}</div>
     <div style={{display:'flex',fontSize:11,color:'#b8b2ca',fontWeight:600,letterSpacing:'1.5px'}}>{s.label.toUpperCase()}</div>
    </div>;
   })}
  </div>
);
})()
```

## Tech Stack

```aura width=860 height=230
(function() {
 var categories = [
  {title:'LANGUAGES',color:'#a78bfa',items:['C++','Java','Python','C','SQL']},
  {title:'CORE CS',color:'#60a5fa',items:['Data Structures','OOP','DBMS','Linux']},
  {title:'BACKEND',color:'#34d399',items:['Flask','FastAPI','SQLAlchemy','REST APIs']},
  {title:'DATA & TOOLS',color:'#f59e0b',items:['NumPy','Pandas','Scikit-learn','Streamlit','Git','GitHub','VS Code','MySQL','SQLite']}
 ];
 return (
  <div style={{
   width:'100%',height:'100%',background:'#08080c',
   display:'flex',flexDirection:'column',fontFamily:'Inter,sans-serif',
   padding:'18px 24px',gap:15,borderRadius:16,
   border:'1px solid rgba(110,80,220,.25)',
   position:'relative',overflow:'hidden'
  }}>
   <style>{`
    @keyframes techGlow{0%,100%{opacity:.3}50%{opacity:.8}}
    #techGlow{animation:techGlow 8s ease-in-out infinite}
   `}</style>
   <svg width="860" height="230" style={{position:'absolute',top:0,left:0}}>
    <defs>
     <radialGradient id="techGradient">
      <stop offset="0%" stopColor="rgba(90,45,230,.4)"/>
      <stop offset="100%" stopColor="rgba(90,45,230,0)"/>
     </radialGradient>
    </defs>
    <ellipse id="techGlow" cx="600" cy="200" rx="350" ry="180" fill="url(#techGradient)"/>
   </svg>
   <div style={{display:'flex',fontSize:10,fontWeight:700,color:'#a99ad5',letterSpacing:'3px',zIndex:1}}>TECHNOLOGIES & TOOLS</div>
   <div style={{display:'flex',flexDirection:'column',gap:14,zIndex:1}}>
    {categories.map(function(cat){
     return <div key={cat.title} style={{display:'flex',alignItems:'flex-start',gap:12}}>
      <div style={{display:'flex',fontSize:10,fontWeight:700,color:cat.color,letterSpacing:'.5px',width:105,flexShrink:0,paddingTop:6}}>{cat.title}</div>
      <div style={{display:'flex',flexWrap:'wrap',gap:7}}>
       {cat.items.map(function(item){
        return <div key={item} style={{
         display:'flex',padding:'5px 10px',borderRadius:6,
         background:cat.color+'15',
         border:'1px solid '+cat.color+'40',
         color:'#e1dcff',fontSize:11,fontWeight:600
        }}>{item}</div>;
       })}
      </div>
     </div>;
    })}
   </div>
  </div>
);
})()
```

## Connect With Me

```aura width=170 height=44 link="https://github.com/SaharshGovind" inline align=center
<SocialMediaButton
 icon="https://raw.githubusercontent.com/collectioneur/collectioneur/main/icons/github-icon.svg"
 text="GitHub"
 backgroundColor="#000000"
 width={170}
 height={44}
 gradientStops={[
  {offset:'0%',color:'#b57af9'},
  {offset:'30%',color:'#000000'},
  {offset:'60%',color:'#9d6bf0'},
  {offset:'80%',color:'#000000'},
  {offset:'100%',color:'#c89dfb'}
 ]}
/>
```

<p align="center">
  <a href="https://github.com/SaharshGovind">GitHub Profile</a>
  &nbsp;•&nbsp;
  <a href="https://github.com/SaharshGovind?tab=repositories">My Projects</a>
</p>

<p align="center">
  <sub>Learning, building, and improving one commit at a time.</sub>
</p>

<p align="center">
  <sub>Powered by <a href="https://github.com/collectioneur/readme-aura">readme-aura</a></sub>
</p>
