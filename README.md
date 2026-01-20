import React, { useState, useEffect } from 'react';
import { 
  Github, 
  ExternalLink, 
  Mail, 
  Linkedin,
  ShieldCheck, 
  Brain, 
  Terminal, 
  Lock, 
  Cpu, 
  Activity, 
  Database, 
  Search,
  ChevronRight,
  ShieldAlert,
  Fingerprint,
  Zap,
  Globe,
  Star // Added missing Star import
} from 'lucide-react';

const App = () => {
  const GITHUB_USERNAME = 'MohsinHaiderSultan';
  const [userData, setUserData] = useState(null);
  const [repos, setRepos] = useState([]);
  const [loading, setLoading] = useState(true);

  useEffect(() => {
    const fetchData = async () => {
      try {
        const [userRes, repoRes] = await Promise.all([
          fetch(`https://api.github.com/users/${GITHUB_USERNAME}`),
          fetch(`https://api.github.com/users/${GITHUB_USERNAME}/repos?sort=updated&per_page=6`)
        ]);
        const userJson = await userRes.json();
        const repoJson = await repoRes.json();
        setUserData(userJson);
        setRepos(repoJson);
      } catch (err) {
        console.error("Error fetching GitHub data:", err);
      } finally {
        setLoading(false);
      }
    };
    fetchData();
  }, []);

  const skillGroups = [
    {
      title: "AI & INTELLIGENCE",
      icon: <Brain className="text-cyan-400" />,
      skills: ["LLMs & RAG", "Predictive ML", "Agentic AI", "Data Science"]
    },
    {
      title: "CYBER DEFENSE",
      icon: <ShieldCheck className="text-blue-500" />,
      skills: ["Threat Hunting", "Cryptography", "Zero Trust", "SIEM / Splunk"]
    },
    {
      title: "ENGINEERING",
      icon: <Cpu className="text-indigo-500" />,
      skills: ["Python (Advanced)", "Docker & K8s", "AWS Security", "Linux Kernel"]
    }
  ];

  const flagshipProjects = [
    {
      title: "AI LOGGUARD",
      subtitle: "Advanced Anomaly Detection System",
      tech: ["Python", "XGBoost", "ELK Stack"],
      desc: "Automated threat hunting in system telemetry with 95%+ accuracy. Designed to identify sophisticated zero-day anomalies.",
      icon: <Activity className="text-emerald-400" />
    },
    {
      title: "PHISHGUARD AI",
      subtitle: "Real-time Threat Intelligence",
      tech: ["Streamlit", "NLP", "FastAPI"],
      desc: "High-speed classification of malicious URLs using linguistic analysis and transformer models.",
      icon: <ShieldAlert className="text-amber-400" />
    }
  ];

  return (
    <div className="min-h-screen bg-[#020617] text-slate-300 font-sans selection:bg-cyan-500/30">
      {/* Dynamic Grid Background */}
      <div className="fixed inset-0 pointer-events-none z-0">
        <div className="absolute inset-0 bg-[linear-gradient(to_right,#1e293b_1px,transparent_1px),linear-gradient(to_bottom,#1e293b_1px,transparent_1px)] bg-[size:40px_40px] [mask-image:radial-gradient(ellipse_60%_50%_at_50%_0%,#000_70%,transparent_100%)] opacity-20" />
        <div className="absolute top-0 left-1/4 w-96 h-96 bg-cyan-500/10 blur-[120px] rounded-full" />
        <div className="absolute bottom-0 right-1/4 w-96 h-96 bg-blue-600/10 blur-[120px] rounded-full" />
      </div>

      {/* Navigation */}
      <nav className="sticky top-0 z-50 backdrop-blur-xl border-b border-white/5 bg-slate-950/80 px-6 py-4">
        <div className="max-w-6xl mx-auto flex justify-between items-center">
          <div className="flex items-center gap-3">
            <div className="p-2 bg-cyan-500/10 rounded-lg border border-cyan-500/20">
              <Fingerprint className="text-cyan-400" size={24} />
            </div>
            <span className="font-bold text-xl tracking-tight text-white hidden sm:block">
              MOHSIN<span className="text-cyan-400">.AI</span>
            </span>
          </div>
          
          <div className="flex items-center gap-8 text-xs font-bold uppercase tracking-widest">
            <a href="#projects" className="hover:text-cyan-400 transition-colors">Projects</a>
            <a href="#radar" className="hover:text-cyan-400 transition-colors">Tech Radar</a>
            <div className="h-4 w-px bg-white/10 hidden sm:block" />
            <div className="hidden sm:flex items-center gap-2 text-emerald-400">
              <span className="relative flex h-2 w-2">
                <span className="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
                <span className="relative inline-flex rounded-full h-2 w-2 bg-emerald-500"></span>
              </span>
              SYSTEM: OPERATIONAL
            </div>
          </div>
        </div>
      </nav>

      {/* Hero Header */}
      <header className="relative z-10 pt-24 pb-16 px-6">
        <div className="max-w-6xl mx-auto text-center space-y-8">
          <div className="inline-block">
             <img 
              src={`https://capsule-render.vercel.app/api?type=waving&color=00D4FF&height=180&section=header&text=Mohsin%20Haider&fontSize=70`} 
              alt="Mohsin Haider"
              className="w-full max-w-4xl mx-auto rounded-2xl shadow-2xl shadow-cyan-500/10"
            />
          </div>
          
          <div className="space-y-4">
            <h1 className="text-4xl md:text-6xl font-black text-white tracking-tight">
              AI & CYBERSECURITY <span className="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-500">ENGINEER</span>
            </h1>
            <div className="flex justify-center">
              <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=36BCF7&center=true&vCenter=true&width=435&lines=Building+AI+LogGuard;Developing+PhishGuard+AI;Securing+the+Future+with+ML;Cyber+Threat+Intelligence" alt="Typing SVG" />
            </div>
          </div>

          <div className="flex justify-center gap-4 pt-4">
            <a href={`https://linkedin.com/in/MohsinHaiderSultan`} target="_blank" className="p-3 bg-white/5 border border-white/10 rounded-full hover:bg-cyan-500/10 hover:border-cyan-500/50 transition-all text-white">
              <Linkedin size={20} />
            </a>
            <a href={`mailto:mohsinhaidersultan001@gmail.com`} className="p-3 bg-white/5 border border-white/10 rounded-full hover:bg-cyan-500/10 hover:border-cyan-500/50 transition-all text-white">
              <Mail size={20} />
            </a>
            <a href={`https://github.com/${GITHUB_USERNAME}`} target="_blank" className="p-3 bg-white/5 border border-white/10 rounded-full hover:bg-cyan-500/10 hover:border-cyan-500/50 transition-all text-white">
              <Github size={20} />
            </a>
          </div>
        </div>
      </header>

      {/* Flagship Projects Section */}
      <section id="projects" className="py-20 px-6 relative z-10">
        <div className="max-w-6xl mx-auto">
          <div className="flex items-center gap-4 mb-12">
            <Terminal className="text-cyan-500" size={32} />
            <h2 className="text-3xl font-bold text-white tracking-tighter">PROJECT TERMINAL</h2>
            <div className="h-px flex-1 bg-gradient-to-r from-white/10 to-transparent" />
          </div>

          <div className="grid md:grid-cols-2 gap-8">
            {flagshipProjects.map((p, i) => (
              <div key={i} className="group relative bg-slate-900/40 border border-white/5 p-8 rounded-2xl overflow-hidden hover:border-cyan-500/50 transition-all duration-500">
                <div className="absolute top-0 right-0 p-4 opacity-5 group-hover:opacity-20 transition-opacity">
                  {p.icon}
                </div>
                <div className="relative z-10 space-y-4">
                  <div className="flex items-center gap-3">
                    <div className="p-2 bg-white/5 rounded-lg">
                      {p.icon}
                    </div>
                    <div>
                      <h3 className="text-xl font-bold text-white tracking-wide">{p.title}</h3>
                      <p className="text-cyan-500/80 text-xs font-bold uppercase tracking-widest">{p.subtitle}</p>
                    </div>
                  </div>
                  <p className="text-slate-400 leading-relaxed">
                    {p.desc}
                  </p>
                  <div className="flex flex-wrap gap-2 pt-2">
                    {p.tech.map((t, idx) => (
                      <code key={idx} className="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">
                        {t}
                      </code>
                    ))}
                  </div>
                </div>
                <div className="absolute bottom-0 left-0 h-1 w-0 bg-cyan-500 group-hover:w-full transition-all duration-700" />
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Tech Radar Section */}
      <section id="radar" className="py-20 px-6 bg-slate-950/50 relative z-10">
        <div className="max-w-6xl mx-auto">
          <div className="text-center mb-16 space-y-2">
            <h2 className="text-3xl font-bold text-white tracking-tight flex items-center justify-center gap-3">
              <Zap className="text-cyan-400" /> TECH RADAR
            </h2>
            <p className="text-slate-500 uppercase text-xs font-bold tracking-[0.2em]">Deployment-Ready Stack</p>
          </div>

          <div className="grid md:grid-cols-3 gap-6">
            {skillGroups.map((group, idx) => (
              <div key={idx} className="bg-slate-900/60 border border-white/5 p-8 rounded-3xl hover:bg-slate-900/80 transition-colors group">
                <div className="flex items-center gap-4 mb-6">
                  <div className="p-3 bg-white/5 rounded-2xl group-hover:scale-110 transition-transform">
                    {group.icon}
                  </div>
                  <h3 className="font-black text-white tracking-widest text-sm uppercase">{group.title}</h3>
                </div>
                <ul className="space-y-4">
                  {group.skills.map((skill, sIdx) => (
                    <li key={sIdx} className="flex items-center gap-3 text-slate-400 text-sm">
                      <div className="w-1.5 h-1.5 rounded-full bg-cyan-500/40" />
                      {skill}
                    </li>
                  ))}
                </ul>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Analytics Hub */}
      <section className="py-20 px-6 relative z-10">
        <div className="max-w-6xl mx-auto">
          <div className="flex items-center gap-4 mb-12">
            <Database className="text-cyan-500" size={32} />
            <h2 className="text-3xl font-bold text-white tracking-tighter">ANALYTICS HUB</h2>
            <div className="h-px flex-1 bg-gradient-to-r from-white/10 to-transparent" />
          </div>

          <div className="grid lg:grid-cols-2 gap-8 items-start">
            <div className="space-y-8">
              <div className="p-6 bg-slate-900/40 border border-white/5 rounded-2xl flex justify-center">
                 <img src={`https://github-readme-stats.vercel.app/api?username=${GITHUB_USERNAME}&show_icons=true&theme=transparent&title_color=00D4FF&text_color=ffffff&icon_color=00D4FF&border_radius=10&hide_border=true`} className="w-full" alt="GitHub Stats" />
              </div>
              <div className="p-6 bg-slate-900/40 border border-white/5 rounded-2xl flex justify-center">
                 <img src={`https://github-readme-stats.vercel.app/api/top-langs/?username=${GITHUB_USERNAME}&layout=compact&theme=transparent&title_color=00D4FF&text_color=ffffff&border_radius=10&hide_border=true`} className="w-full" alt="Top Languages" />
              </div>
            </div>
            
            <div className="space-y-8">
               <div className="p-6 bg-slate-900/40 border border-white/5 rounded-2xl flex justify-center overflow-hidden">
                 <img src={`https://github-readme-activity-graph.vercel.app/graph?username=${GITHUB_USERNAME}&theme=react-dark&hide_border=true&area=true&color=00D4FF`} className="w-full scale-110" alt="Activity Graph" />
               </div>
               <div className="p-6 bg-slate-900/40 border border-white/5 rounded-2xl flex justify-center">
                 <img src={`https://github-profile-trophy.vercel.app/?username=${GITHUB_USERNAME}&theme=dracula&no-frame=true&column=7`} className="w-full opacity-80 hover:opacity-100 transition-opacity" alt="Trophies" />
               </div>
            </div>
          </div>
        </div>
      </section>

      {/* Recent Repos */}
      <section className="py-20 px-6 bg-slate-950/50">
        <div className="max-w-6xl mx-auto">
          <div className="flex justify-between items-end mb-12">
            <div className="space-y-2">
              <h2 className="text-3xl font-bold text-white tracking-tight">RECENT COMMITS</h2>
              <p className="text-slate-500 text-xs font-bold tracking-widest uppercase">Live GitHub Feed</p>
            </div>
            <a href={`https://github.com/${GITHUB_USERNAME}`} className="text-cyan-400 font-bold text-xs uppercase hover:underline flex items-center gap-1">
              View All <ChevronRight size={14} />
            </a>
          </div>

          <div className="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
            {loading ? Array(6).fill(0).map((_, i) => (
              <div key={i} className="h-48 bg-white/5 rounded-2xl animate-pulse" />
            )) : repos.map((repo) => (
              <a 
                key={repo.id} 
                href={repo.html_url}
                target="_blank"
                className="block p-6 bg-slate-900/60 border border-white/5 rounded-2xl hover:border-cyan-500/50 hover:-translate-y-1 transition-all group"
              >
                <div className="flex justify-between mb-4">
                  <Github className="text-white/20 group-hover:text-cyan-400 transition-colors" size={20} />
                  <ExternalLink className="text-white/20 group-hover:text-white transition-colors" size={16} />
                </div>
                <h3 className="font-bold text-white mb-2 truncate group-hover:text-cyan-400 transition-colors uppercase tracking-wide">
                  {repo.name.replace(/-/g, ' ')}
                </h3>
                <p className="text-slate-500 text-xs line-clamp-2 mb-4 leading-relaxed">
                  {repo.description || "Experimental engineering project hosted on GitHub."}
                </p>
                <div className="flex items-center gap-3 text-[10px] font-black text-slate-400 uppercase">
                  <span className="flex items-center gap-1">
                    <div className="w-2 h-2 rounded-full bg-cyan-500" />
                    {repo.language || 'Code'}
                  </span>
                  <span className="flex items-center gap-1">
                    <Star size={12} className="text-amber-500" />
                    {repo.stargazers_count}
                  </span>
                </div>
              </a>
            ))}
          </div>
        </div>
      </section>

      {/* Footer / Quote */}
      <footer className="py-24 px-6 border-t border-white/5">
        <div className="max-w-4xl mx-auto text-center space-y-12">
          <img src={`https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight`} className="mx-auto w-full max-w-2xl opacity-80" alt="Quote" />
          
          <div className="flex flex-col items-center gap-6">
            <div className="flex gap-8 text-xs font-black tracking-[0.3em] text-slate-500 uppercase">
              <span className="flex items-center gap-2">
                <div className="w-2 h-2 rounded-full bg-emerald-500" />
                System: Operational
              </span>
              <span className="flex items-center gap-2">
                <Lock size={12} />
                Security: Maximum
              </span>
            </div>
            
            <p className="text-slate-600 text-[10px] font-bold tracking-widest uppercase">
              Mohsin Haider Sultan &copy; {new Date().getFullYear()} // Built with Intelligence
            </p>
          </div>
        </div>
      </footer>
    </div>
  );
};

export default App;
