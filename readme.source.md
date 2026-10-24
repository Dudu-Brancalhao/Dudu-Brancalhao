```aura width=800 height=340
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#070a12', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.6; } 50% { transform: translate(28px, -22px); opacity: 0.9; } }
    @keyframes orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(-22px, 18px); opacity: 0.75; } }
    @keyframes ring-blink { 0%, 100% { opacity: 0.05; } 50% { opacity: 0.16; } }
    @keyframes dot-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    #h-o1 { animation: orb-a 9s ease-in-out infinite; }
    #h-o2 { animation: orb-b 11s ease-in-out infinite 0.8s; }
    #h-o3 { animation: orb-a 8s ease-in-out infinite 2s; }
    #h-o4 { animation: orb-b 13s ease-in-out infinite 0.4s; }
    #h-r1 { animation: ring-blink 8s ease-in-out infinite; }
    #h-r2 { animation: ring-blink 8s ease-in-out infinite 1.6s; }
    #h-r3 { animation: ring-blink 8s ease-in-out infinite 3.2s; }
    #h-dot { animation: dot-spin 18s linear infinite; transform-origin: 400px 170px; }
  `}</style>
  <svg width="800" height="340" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(56,132,255,0.55)" /><stop offset="100%" stopColor="rgba(56,132,255,0)" /></radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(45,212,191,0.45)" /><stop offset="100%" stopColor="rgba(45,212,191,0)" /></radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,120,255,0.38)" /><stop offset="100%" stopColor="rgba(139,120,255,0)" /></radialGradient>
      <radialGradient id="hg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(80,170,255,0.3)" /><stop offset="100%" stopColor="rgba(80,170,255,0)" /></radialGradient>
    </defs>
    <ellipse id="h-o1" cx="110" cy="290" rx="260" ry="200" fill="url(#hg1)" />
    <ellipse id="h-o2" cx="710" cy="70" rx="230" ry="190" fill="url(#hg2)" />
    <ellipse id="h-o3" cx="630" cy="320" rx="200" ry="160" fill="url(#hg3)" />
    <ellipse id="h-o4" cx="210" cy="50" rx="190" ry="150" fill="url(#hg4)" />
    <circle id="h-r1" cx="400" cy="170" r="70" fill="none" stroke="rgba(255,255,255,0.14)" strokeWidth="0.7" />
    <circle id="h-r2" cx="400" cy="170" r="125" fill="none" stroke="rgba(255,255,255,0.14)" strokeWidth="0.7" />
    <circle id="h-r3" cx="400" cy="170" r="190" fill="none" stroke="rgba(255,255,255,0.14)" strokeWidth="0.7" />
    <g id="h-dot"><circle cx="400" cy="45" r="2.5" fill="rgba(255,255,255,0.6)" /></g>
  </svg>
  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center' }}>
    <span style={{ fontSize: 54, fontWeight: 700, color: '#ffffff', letterSpacing: -2, lineHeight: 1 }}>Eduardo Brancalhão</span>
    <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.5)', marginTop: 16, letterSpacing: 5, textTransform: 'uppercase' }}>software engineer · backend · ai-native</span>
    <div style={{ display: 'flex', gap: 8, marginTop: 28 }}>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.65)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>crypto wallets</span>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.65)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>prediction markets</span>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.65)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>real-time video</span>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.65)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)', letterSpacing: 1 }}>spec-driven</span>
    </div>
  </div>
</div>
```

```aura width=800 height=230
<div style={{ display: 'flex', flexDirection: 'row', gap: 16, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes ab-orb { 0%, 100% { transform: translate(0,0); opacity: 0.6; } 50% { transform: translate(18px,-12px); opacity: 0.9; } }
    @keyframes cursor-blink { 0%, 49% { opacity: 1; } 50%, 100% { opacity: 0; } }
    #ab-o1 { animation: ab-orb 8s ease-in-out infinite; }
    #ab-o2 { animation: ab-orb 10s ease-in-out infinite 1.5s; }
    #ab-cursor { animation: cursor-blink 1.1s step-end infinite; }
  `}</style>
  <div style={{ position: 'relative', display: 'flex', flex: 1, height: '100%', background: '#070a12', borderRadius: 16, overflow: 'hidden', border: '1px solid rgba(255,255,255,0.06)' }}>
    <svg width="560" height="230" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="ag1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(56,132,255,0.45)" /><stop offset="100%" stopColor="rgba(56,132,255,0)" /></radialGradient>
        <radialGradient id="ag2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(45,212,191,0.35)" /><stop offset="100%" stopColor="rgba(45,212,191,0)" /></radialGradient>
      </defs>
      <ellipse id="ab-o1" cx="40" cy="200" rx="160" ry="120" fill="url(#ag1)" />
      <ellipse id="ab-o2" cx="520" cy="20" rx="160" ry="120" fill="url(#ag2)" />
    </svg>
    <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 30px' }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 3, textTransform: 'uppercase', marginBottom: 12 }}>about</span>
      <span style={{ fontSize: 24, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>Building backend systems</span>
      <span style={{ fontSize: 24, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>that move real money.</span>
      <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.55)', marginTop: 12, lineHeight: 1.5 }}>Node.js · NestJS · TypeScript · PostgreSQL. Frontend roots in React.</span>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 14 }}>
        <span style={{ fontSize: 13, color: 'rgba(125,211,252,0.85)', fontFamily: 'monospace' }}>{'> spec first, then agents'}</span>
        <span id="ab-cursor" style={{ fontSize: 13, color: 'rgba(125,211,252,0.85)', fontFamily: 'monospace', marginLeft: 2 }}>_</span>
      </div>
    </div>
  </div>
  <div style={{ display: 'flex', flexDirection: 'column', gap: 16, width: 224, flexShrink: 0 }}>
    <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: '#070a12', borderRadius: 16, border: '1px solid rgba(255,255,255,0.06)', justifyContent: 'center', padding: '0 20px' }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 2, textTransform: 'uppercase' }}>now</span>
      <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff', marginTop: 6 }}>Software Engineer</span>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 2 }}>@ Hubib · crypto & markets</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', flex: 1, background: '#070a12', borderRadius: 16, border: '1px solid rgba(255,255,255,0.06)', justifyContent: 'center', padding: '0 20px' }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 2, textTransform: 'uppercase' }}>principle</span>
      <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff', marginTop: 6 }}>Security and data</span>
      <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>integrity first.</span>
    </div>
  </div>
</div>
```

```aura width=800 height=210 link="https://github.com/Dudu-Brancalhao/AgroHub"
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', width: '100%', height: '100%', background: '#070a12', borderRadius: 20, overflow: 'hidden', border: '1px solid rgba(255,255,255,0.06)', fontFamily: 'Inter, sans-serif', padding: '0 34px' }}>
  <style>{`
    @keyframes fp-orb { 0%, 100% { transform: translate(0,0); opacity: 0.5; } 50% { transform: translate(-20px,14px); opacity: 0.8; } }
    #fp-o1 { animation: fp-orb 10s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="210" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="fg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(139,120,255,0.4)" /><stop offset="100%" stopColor="rgba(139,120,255,0)" /></radialGradient>
    </defs>
    <ellipse id="fp-o1" cx="700" cy="170" rx="220" ry="150" fill="url(#fg1)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 3, textTransform: 'uppercase' }}>featured project</span>
  <div style={{ display: 'flex', alignItems: 'baseline', marginTop: 8 }}>
    <span style={{ fontSize: 28, fontWeight: 700, color: '#ffffff' }}>AgroHub</span>
    <span style={{ fontSize: 13, color: 'rgba(125,211,252,0.85)', marginLeft: 12 }}>view repo</span>
  </div>
  <span style={{ fontSize: 14, color: 'rgba(255,255,255,0.6)', marginTop: 6 }}>Take-home project: rural producer registry with API, React frontend and dashboard. Deployed, spec-driven, built with Claude Code.</span>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 8, marginTop: 16 }}>
    {['NestJS', 'Prisma', 'PostgreSQL', 'Docker', 'OpenAPI', 'JWT', '45 test files', 'React'].map((t, i) => (
      <span key={i} style={{ padding: '5px 14px', background: 'rgba(255,255,255,0.05)', color: 'rgba(255,255,255,0.7)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.1)' }}>{t}</span>
    ))}
  </div>
</div>
```

```aura width=800 height=190
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#070a12', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes st-orb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(18px,-14px); opacity: 0.7; } }
    #st-o1 { animation: st-orb 10s ease-in-out infinite; }
    #st-o2 { animation: st-orb 12s ease-in-out infinite 1s; }
  `}</style>
  <svg width="800" height="190" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="sg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(56,132,255,0.38)" /><stop offset="100%" stopColor="rgba(56,132,255,0)" /></radialGradient>
      <radialGradient id="sg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(45,212,191,0.32)" /><stop offset="100%" stopColor="rgba(45,212,191,0)" /></radialGradient>
    </defs>
    <ellipse id="st-o1" cx="80" cy="150" rx="170" ry="120" fill="url(#sg1)" />
    <ellipse id="st-o2" cx="720" cy="40" rx="160" ry="120" fill="url(#sg2)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 18 }}>stack</span>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 10, justifyContent: 'center', maxWidth: 700 }}>
    {['Node.js', 'NestJS', 'TypeScript', 'PostgreSQL', 'Prisma', 'Docker', 'WebSockets', 'WebRTC', 'Python', 'React', 'Next.js', 'Claude Code'].map((t, i) => (
      <span key={i} style={{ padding: '7px 18px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.7)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(255,255,255,0.09)' }}>{t}</span>
    ))}
  </div>
</div>
```

```aura width=140 height=44 link="https://www.linkedin.com/in/eduardo-brancalhao/" inline align=center
<SocialMediaButton
  icon="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iIzBBNjZDMiIgZD0iTTIwLjQ0NyAyMC40NTJoLTMuNTU0di01LjU2OWMwLTEuMzI4LS4wMjctMy4wMzctMS44NTItMy4wMzctMS44NTMgMC0yLjEzNiAxLjQ0NS0yLjEzNiAyLjkzOXY1LjY2N0g5LjM1MVY5aDMuNDE0djEuNTYxaC4wNDZjLjQ3Ny0uOSAxLjYzNy0xLjg1IDMuMzctMS44NSAzLjYwMSAwIDQuMjY3IDIuMzcgNC4yNjcgNC45ODF2Ni4yNzZ6TTUuMzM3IDcuNDMzYy0xLjE0NCAwLTIuMDYzLS45MjYtMi4wNjMtMi4wNjUgMC0xLjEzOC45Mi0yLjA2MyAyLjA2My0yLjA2MyAxLjE0IDAgMi4wNjQuOTI1IDIuMDY0IDIuMDYzIDAgMS4xMzktLjkyNSAyLjA2NS0yLjA2NCAyLjA2NXptMS43ODIgMTMuMDE5SDMuNTU1VjloMy41NjR2MTEuNDUyek0yMi4yMjUgMEgxLjc3MUMuNzkyIDAgMCAuNzc0IDAgMS43Mjl2MjAuNTQyQzAgMjMuMjI3Ljc5MiAyNCAxLjc3MSAyNGgyMC40NTFDMjMuMiAyNCAyNCAyMy4yMjcgMjQgMjIuMjcxVjEuNzI5QzI0IC43NzQgMjMuMiAwIDIyLjIyMiAwaC4wMDN6Ii8+PC9zdmc+"
  text="LinkedIn"
  backgroundColor="#0a1a2b"
  width={140}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#0A66C2' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=140 height=44 link="https://dudu-portfolio.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/googlechrome/ffffff"
  text="Portfolio"
  backgroundColor="#141414"
  width={140}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=120 height=44 link="mailto:duduscala@gmail.com" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/gmail/EA4335"
  text="Email"
  backgroundColor="#2b0a0a"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#EA4335' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```
