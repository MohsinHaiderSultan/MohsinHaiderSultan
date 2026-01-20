<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mohsin Haider Sultan | AI & Cybersecurity Engineer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/lucide@latest"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;900&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; }
        .glass { background: rgba(15, 23, 42, 0.6); backdrop-filter: blur(12px); border: 1px solid rgba(255, 255, 255, 0.05); }
        .cyber-grid {
            background-image: linear-gradient(to right, #1e293b 1px, transparent 1px), 
                              linear-gradient(to bottom, #1e293b 1px, transparent 1px);
            background-size: 40px 40px;
            mask-image: radial-gradient(ellipse 60% 50% at 50% 0%, #000 70%, transparent 100%);
        }
        @keyframes pulse-slow {
            0%, 100% { opacity: 0.4; }
            50% { opacity: 0.8; }
        }
        .animate-pulse-slow { animation: pulse-slow 3s infinite; }
    </style>
</head>
<body class="bg-[#020617] text-slate-300 overflow-x-hidden selection:bg-cyan-500/30">

    <!-- Background Decoration -->
    <div class="fixed inset-0 pointer-events-none z-0">
        <div class="absolute inset-0 cyber-grid opacity-20"></div>
        <div class="absolute top-0 left-1/4 w-96 h-96 bg-cyan-500/10 blur-[120px] rounded-full"></div>
        <div class="absolute bottom-0 right-1/4 w-96 h-96 bg-blue-600/10 blur-[120px] rounded-full"></div>
    </div>

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 glass px-6 py-4">
        <div class="max-w-6xl mx-auto flex justify-between items-center">
            <div class="flex items-center gap-3">
                <div class="p-2 bg-cyan-500/10 rounded-lg border border-cyan-500/20">
                    <i data-lucide="fingerprint" class="text-cyan-400"></i>
                </div>
                <span class="font-bold text-xl tracking-tight text-white hidden sm:block">
                    MOHSIN<span class="text-cyan-400">.AI</span>
                </span>
            </div>
            
            <div class="flex items-center gap-8 text-xs font-bold uppercase tracking-widest">
                <a href="#projects" class="hover:text-cyan-400 transition-colors">Projects</a>
                <a href="#radar" class="hover:text-cyan-400 transition-colors">Tech Radar</a>
                <div class="h-4 w-px bg-white/10 hidden sm:block"></div>
                <div class="hidden sm:flex items-center gap-2 text-emerald-400">
                    <span class="relative flex h-2 w-2">
                        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
                        <span class="relative inline-flex rounded-full h-2 w-2 bg-emerald-500"></span>
                    </span>
                    SYSTEM: OPERATIONAL
                </div>
            </div>
        </div>
    </nav>

    <!-- Hero Header -->
    <header class="relative z-10 pt-24 pb-16 px-6">
        <div class="max-w-6xl mx-auto text-center space-y-8">
            <div class="inline-block w-full max-w-4xl mx-auto rounded-2xl overflow-hidden shadow-2xl shadow-cyan-500/10">
                <img src="https://capsule-render.vercel.app/api?type=waving&color=00D4FF&height=180&section=header&text=Mohsin%20Haider&fontSize=70" alt="Mohsin Haider" class="w-full">
            </div>
            
            <div class="space-y-4">
                <h1 class="text-4xl md:text-6xl font-black text-white tracking-tight">
                    AI & CYBERSECURITY <span class="text-transparent bg-clip-text bg-gradient-to-r from-cyan-400 to-blue-500">ENGINEER</span>
                </h1>
                <div class="flex justify-center">
                    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=36BCF7&center=true&vCenter=true&width=435&lines=Building+AI+LogGuard;Developing+PhishGuard+AI;Securing+the+Future+with+ML;Cyber+Threat+Intelligence" alt="Typing SVG" />
                </div>
            </div>

            <div class="flex justify-center gap-4 pt-4">
                <a href="https://linkedin.com/in/MohsinHaiderSultan" target="_blank" class="p-3 bg-white/5 border border-white/10 rounded-full hover:bg-cyan-500/10 hover:border-cyan-500/50 transition-all text-white">
                    <i data-lucide="linkedin" size="20"></i>
                </a>
                <a href="mailto:mohsinhaidersultan001@gmail.com" class="p-3 bg-white/5 border border-white/10 rounded-full hover:bg-cyan-500/10 hover:border-cyan-500/50 transition-all text-white">
                    <i data-lucide="mail" size="20"></i>
                </a>
                <a href="https://github.com/MohsinHaiderSultan" target="_blank" class="p-3 bg-white/5 border border-white/10 rounded-full hover:bg-cyan-500/10 hover:border-cyan-500/50 transition-all text-white">
                    <i data-lucide="github" size="20"></i>
                </a>
            </div>
        </div>
    </header>

    <!-- Flagship Projects -->
    <section id="projects" class="py-20 px-6 relative z-10">
        <div class="max-w-6xl mx-auto">
            <div class="flex items-center gap-4 mb-12">
                <i data-lucide="terminal" class="text-cyan-500" size="32"></i>
                <h2 class="text-3xl font-bold text-white tracking-tighter uppercase">Project Terminal</h2>
                <div class="h-px flex-1 bg-gradient-to-r from-white/10 to-transparent"></div>
            </div>

            <div class="grid md:grid-cols-2 gap-8">
                <!-- AI LogGuard -->
                <div class="group relative glass p-8 rounded-2xl overflow-hidden hover:border-cyan-500/50 transition-all duration-500">
                    <div class="absolute top-0 right-0 p-4 opacity-5 group-hover:opacity-20 transition-opacity">
                        <i data-lucide="activity" size="64"></i>
                    </div>
                    <div class="relative z-10 space-y-4">
                        <div class="flex items-center gap-3">
                            <div class="p-2 bg-white/5 rounded-lg text-emerald-400">
                                <i data-lucide="activity"></i>
                            </div>
                            <div>
                                <h3 class="text-xl font-bold text-white tracking-wide">AI LOGGUARD</h3>
                                <p class="text-cyan-500/80 text-xs font-bold uppercase tracking-widest">Anomaly Detection</p>
                            </div>
                        </div>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            Automated threat hunting in system telemetry with 95%+ accuracy. Designed to identify sophisticated zero-day anomalies using ML.
                        </p>
                        <div class="flex flex-wrap gap-2 pt-2">
                            <code class="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">Python</code>
                            <code class="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">XGBoost</code>
                            <code class="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">ELK Stack</code>
                        </div>
                    </div>
                </div>

                <!-- PhishGuard -->
                <div class="group relative glass p-8 rounded-2xl overflow-hidden hover:border-cyan-500/50 transition-all duration-500">
                    <div class="absolute top-0 right-0 p-4 opacity-5 group-hover:opacity-20 transition-opacity">
                        <i data-lucide="shield-alert" size="64"></i>
                    </div>
                    <div class="relative z-10 space-y-4">
                        <div class="flex items-center gap-3">
                            <div class="p-2 bg-white/5 rounded-lg text-amber-400">
                                <i data-lucide="shield-alert"></i>
                            </div>
                            <div>
                                <h3 class="text-xl font-bold text-white tracking-wide">PHISHGUARD AI</h3>
                                <p class="text-cyan-500/80 text-xs font-bold uppercase tracking-widest">Threat Intelligence</p>
                            </div>
                        </div>
                        <p class="text-slate-400 text-sm leading-relaxed">
                            High-speed classification of malicious URLs using linguistic analysis and transformer models. Real-time protection API.
                        </p>
                        <div class="flex flex-wrap gap-2 pt-2">
                            <code class="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">Streamlit</code>
                            <code class="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">NLP</code>
                            <code class="px-2 py-1 bg-cyan-500/10 text-cyan-400 text-[10px] font-bold rounded border border-cyan-500/20 uppercase">FastAPI</code>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Tech Radar -->
    <section id="radar" class="py-20 px-6 bg-slate-950/50 relative z-10">
        <div class="max-w-6xl mx-auto">
            <div class="text-center mb-16 space-y-2">
                <h2 class="text-3xl font-bold text-white tracking-tight flex items-center justify-center gap-3">
                    <i data-lucide="zap" class="text-cyan-400"></i> TECH RADAR
                </h2>
                <p class="text-slate-500 uppercase text-xs font-bold tracking-[0.2em]">Deployment-Ready Stack</p>
            </div>

            <div class="grid md:grid-cols-3 gap-6">
                <div class="glass p-8 rounded-3xl group">
                    <div class="flex items-center gap-4 mb-6">
                        <div class="p-3 bg-white/5 rounded-2xl group-hover:scale-110 transition-transform text-cyan-400">
                            <i data-lucide="brain"></i>
                        </div>
                        <h3 class="font-black text-white tracking-widest text-sm uppercase">AI & Intelligence</h3>
                    </div>
                    <ul class="space-y-4 text-sm text-slate-400">
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> LLMs & RAG</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Predictive ML</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Agentic AI</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Data Science</li>
                    </ul>
                </div>
                <div class="glass p-8 rounded-3xl group">
                    <div class="flex items-center gap-4 mb-6">
                        <div class="p-3 bg-white/5 rounded-2xl group-hover:scale-110 transition-transform text-blue-500">
                            <i data-lucide="shield-check"></i>
                        </div>
                        <h3 class="font-black text-white tracking-widest text-sm uppercase">Cyber Defense</h3>
                    </div>
                    <ul class="space-y-4 text-sm text-slate-400">
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Threat Hunting</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Cryptography</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Zero Trust</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> SIEM / Splunk</li>
                    </ul>
                </div>
                <div class="glass p-8 rounded-3xl group">
                    <div class="flex items-center gap-4 mb-6">
                        <div class="p-3 bg-white/5 rounded-2xl group-hover:scale-110 transition-transform text-indigo-500">
                            <i data-lucide="cpu"></i>
                        </div>
                        <h3 class="font-black text-white tracking-widest text-sm uppercase">Engineering</h3>
                    </div>
                    <ul class="space-y-4 text-sm text-slate-400">
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Python (Advanced)</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Docker & K8s</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> AWS Security</li>
                        <li class="flex items-center gap-3"><div class="w-1.5 h-1.5 rounded-full bg-cyan-500"></div> Linux Kernel</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Analytics -->
    <section class="py-20 px-6 relative z-10">
        <div class="max-w-6xl mx-auto">
            <div class="flex items-center gap-4 mb-12">
                <i data-lucide="database" class="text-cyan-500" size="32"></i>
                <h2 class="text-3xl font-bold text-white tracking-tighter uppercase">Analytics Hub</h2>
                <div class="h-px flex-1 bg-gradient-to-r from-white/10 to-transparent"></div>
            </div>
            
            <div class="grid lg:grid-cols-2 gap-8 items-start">
                <div class="space-y-8">
                    <img src="https://github-readme-stats.vercel.app/api?username=MohsinHaiderSultan&show_icons=true&theme=transparent&title_color=00D4FF&text_color=ffffff&icon_color=00D4FF&border_radius=10&hide_border=true" class="w-full glass rounded-2xl p-4" alt="Stats" />
                    <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=MohsinHaiderSultan&layout=compact&theme=transparent&title_color=00D4FF&text_color=ffffff&border_radius=10&hide_border=true" class="w-full glass rounded-2xl p-4" alt="Langs" />
                </div>
                <div class="space-y-8">
                    <img src="https://github-readme-activity-graph.vercel.app/graph?username=MohsinHaiderSultan&theme=react-dark&hide_border=true&area=true&color=00D4FF" class="w-full glass rounded-2xl p-4" alt="Activity" />
                    <img src="https://github-profile-trophy.vercel.app/?username=MohsinHaiderSultan&theme=dracula&no-frame=true&column=7" class="w-full opacity-80" alt="Trophies" />
                </div>
            </div>
        </div>
    </section>

    <!-- Recent Commits -->
    <section class="py-20 px-6 bg-slate-950/50">
        <div class="max-w-6xl mx-auto">
            <div class="flex justify-between items-end mb-12">
                <div class="space-y-2">
                    <h2 class="text-3xl font-bold text-white tracking-tight uppercase">Recent Commits</h2>
                    <p class="text-slate-500 text-xs font-bold tracking-widest uppercase">Live GitHub Feed</p>
                </div>
                <a href="https://github.com/MohsinHaiderSultan" class="text-cyan-400 font-bold text-xs uppercase hover:underline flex items-center gap-1">
                    View All <i data-lucide="chevron-right" size="14"></i>
                </a>
            </div>
            <div id="repo-grid" class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Repos will be injected here -->
                <div class="h-48 glass rounded-2xl animate-pulse"></div>
                <div class="h-48 glass rounded-2xl animate-pulse"></div>
                <div class="h-48 glass rounded-2xl animate-pulse"></div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-24 px-6 border-t border-white/5">
        <div class="max-w-4xl mx-auto text-center space-y-12">
            <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight" class="mx-auto w-full max-w-2xl opacity-80" alt="Quote" />
            <div class="flex flex-col items-center gap-6">
                <div class="flex gap-8 text-xs font-black tracking-[0.3em] text-slate-500 uppercase">
                    <span class="flex items-center gap-2">
                        <div class="w-2 h-2 rounded-full bg-emerald-500"></div>
                        System: Operational
                    </span>
                    <span class="flex items-center gap-2">
                        <i data-lucide="lock" size="12"></i>
                        Security: Maximum
                    </span>
                </div>
                <p class="text-slate-600 text-[10px] font-bold tracking-widest uppercase">
                    Mohsin Haider Sultan &copy; <span id="year"></span> // Built with Intelligence
                </p>
            </div>
        </div>
    </footer>

    <script>
        // Initialize Lucide Icons
        lucide.createIcons();
        document.getElementById('year').textContent = new Date().getFullYear();

        // Fetch Repos
        async function fetchRepos() {
            const username = 'MohsinHaiderSultan';
            const grid = document.getElementById('repo-grid');
            
            try {
                const response = await fetch(`https://api.github.com/users/${username}/repos?sort=updated&per_page=6`);
                const repos = await response.json();
                
                grid.innerHTML = repos.map(repo => `
                    <a href="${repo.html_url}" target="_blank" class="block p-6 glass rounded-2xl hover:border-cyan-500/50 hover:-translate-y-1 transition-all group">
                        <div class="flex justify-between mb-4">
                            <i data-lucide="github" class="text-white/20 group-hover:text-cyan-400 transition-colors"></i>
                            <i data-lucide="external-link" class="text-white/20 group-hover:text-white transition-colors" size="16"></i>
                        </div>
                        <h3 class="font-bold text-white mb-2 truncate group-hover:text-cyan-400 transition-colors uppercase tracking-wide">
                            ${repo.name.replace(/-/g, ' ')}
                        </h3>
                        <p class="text-slate-500 text-xs line-clamp-2 mb-4 leading-relaxed">
                            ${repo.description || "Experimental engineering project hosted on GitHub."}
                        </p>
                        <div class="flex items-center justify-between text-[10px] font-black text-slate-400 uppercase">
                            <span class="flex items-center gap-1">
                                <div class="w-2 h-2 rounded-full bg-cyan-500"></div>
                                ${repo.language || 'Code'}
                            </span>
                            <span class="flex items-center gap-1">
                                <i data-lucide="star" class="text-amber-500" size="12"></i>
                                ${repo.stargazers_count}
                            </span>
                        </div>
                    </a>
                `).join('');
                
                // Re-init icons for dynamic content
                lucide.createIcons();
                
            } catch (error) {
                grid.innerHTML = '<p class="text-center col-span-full py-10 text-slate-500">Failed to load system telemetry.</p>';
            }
        }

        fetchRepos();
    </script>
</body>
</html>
