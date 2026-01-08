<html lang="en"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Subhajit Nandi | GitHub Profile</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://code.iconify.design/3/3.1.0/iconify.min.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet">
    <style>
        * { font-family: 'Inter', sans-serif; }
        
        .gradient-bg {
            background: linear-gradient(135deg, #0d1117 0%, #161b22 50%, #0d1117 100%);
        }
        
        .card-3d {
            transform-style: preserve-3d;
            transition: transform 0.6s ease;
        }
        
        .card-3d:hover {
            transform: rotateY(5deg) rotateX(5deg) translateZ(20px);
        }
        
        .floating {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px) rotateX(0deg); }
            50% { transform: translateY(-20px) rotateX(5deg); }
        }
        
        .glow {
            box-shadow: 0 0 60px rgba(88, 166, 255, 0.3), 0 0 100px rgba(136, 46, 224, 0.2);
        }
        
        .text-glow {
            text-shadow: 0 0 30px rgba(88, 166, 255, 0.5);
        }
        
        .pulse-ring {
            animation: pulse-ring 2s cubic-bezier(0.455, 0.03, 0.515, 0.955) infinite;
        }
        
        @keyframes pulse-ring {
            0% { transform: scale(0.8); opacity: 1; }
            100% { transform: scale(2); opacity: 0; }
        }
        
        .typing {
            overflow: hidden;
            border-right: 2px solid #58a6ff;
            white-space: nowrap;
            animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #58a6ff }
        }
        
        .skill-bar {
            background: linear-gradient(90deg, #58a6ff, #882ee0);
            animation: skill-fill 2s ease-out forwards;
        }
        
        @keyframes skill-fill {
            from { width: 0; }
        }
        
        .rotate-slow {
            animation: rotate 20s linear infinite;
        }
        
        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }
        
        .gradient-text {
            background: linear-gradient(135deg, #58a6ff, #882ee0, #f78166);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .stat-card {
            backdrop-filter: blur(10px);
            background: rgba(22, 27, 34, 0.8);
            border: 1px solid rgba(88, 166, 255, 0.2);
        }
        
        .hover-lift {
            transition: all 0.3s ease;
        }
        
        .hover-lift:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }
        
        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: #58a6ff;
            border-radius: 50%;
            animation: particle-float 10s infinite;
        }
        
        @keyframes particle-float {
            0%, 100% { transform: translateY(0) translateX(0); opacity: 0; }
            10% { opacity: 1; }
            90% { opacity: 1; }
            100% { transform: translateY(-100vh) translateX(100px); opacity: 0; }
        }
    </style>
</head>
<body class="gradient-bg min-h-screen text-white overflow-x-hidden">
    <!-- Particles Background -->
    <div id="particles" class="fixed inset-0 pointer-events-none overflow-hidden"></div>
    
    <!-- Animated Background Orbs -->
    <div class="fixed inset-0 pointer-events-none overflow-hidden">
        <div class="absolute top-1/4 left-1/4 w-96 h-96 bg-blue-500/10 rounded-full blur-3xl rotate-slow"></div>
        <div class="absolute bottom-1/4 right-1/4 w-80 h-80 bg-purple-500/10 rounded-full blur-3xl rotate-slow" style="animation-direction: reverse;"></div>
    </div>

    <div class="relative z-10 max-w-5xl mx-auto px-4 py-12">
        <!-- Header Section -->
        <header class="text-center mb-16">
            <div class="relative inline-block mb-8">
                <!-- Pulse Ring -->
                <div class="absolute inset-0 rounded-full bg-blue-500/30 pulse-ring"></div>
                <!-- Avatar -->
                <div class="floating">
                    <div class="w-32 h-32 md:w-40 md:h-40 rounded-full glow overflow-hidden border-4 border-gray-700 relative">
                        <img src="https://avatars.githubusercontent.com/subhajit-sudo" alt="Subhajit Nandi" class="w-full h-full object-cover" onerror="this.src='https://ui-avatars.com/api/?name=Subhajit+Nandi&amp;background=161b22&amp;color=58a6ff&amp;size=200'">
                    </div>
                </div>
            </div>
            
            <h1 class="text-4xl md:text-5xl font-semibold tracking-tight mb-4 gradient-text">Subhajit Nandi</h1>
            
            <div class="inline-block">
                <p class="text-lg md:text-xl text-gray-400 typing">@subhajit-sudo • Cybersecurity Enthusiast</p>
            </div>
            
            <div class="flex justify-center gap-4 mt-6">
                <span class="px-3 py-1 rounded-full text-xs font-medium bg-green-500/20 text-green-400 border border-green-500/30">🟢 Available for collaboration</span>
            </div>
        </header>

        <!-- About Section -->
        <section class="card-3d stat-card rounded-2xl p-6 md:p-8 mb-8 glow">
            <div class="flex items-center gap-3 mb-4">
                <span class="iconify text-blue-400" data-icon="lucide:user" data-width="24" style="stroke-width: 1.5;"></span>
                <h2 class="text-xl font-semibold tracking-tight">About Me</h2>
            </div>
            <p class="text-gray-300 leading-relaxed">
                👋 Hi there! I'm <span class="text-blue-400 font-medium">Subhajit Nandi</span>, a passionate developer and cybersecurity enthusiast from India. 
                I love exploring the depths of technology, from building applications to hunting bugs and solving CTF challenges.
                Currently focused on expanding my skills in penetration testing and ethical hacking.
            </p>
            <div class="flex flex-wrap gap-2 mt-4">
                <span class="px-3 py-1 rounded-full text-xs bg-gray-800 text-gray-300 border border-gray-700">🔐 Cybersecurity</span>
                <span class="px-3 py-1 rounded-full text-xs bg-gray-800 text-gray-300 border border-gray-700">💻 Developer</span>
                <span class="px-3 py-1 rounded-full text-xs bg-gray-800 text-gray-300 border border-gray-700">🎯 CTF Player</span>
                <span class="px-3 py-1 rounded-full text-xs bg-gray-800 text-gray-300 border border-gray-700">🐧 Linux Enthusiast</span>
            </div>
        </section>

        <!-- Stats Grid -->
        <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-8">
            <div class="stat-card rounded-xl p-4 text-center hover-lift">
                <div class="text-2xl md:text-3xl font-semibold gradient-text" id="repos">--</div>
                <div class="text-xs text-gray-400 mt-1">Repositories</div>
            </div>
            <div class="stat-card rounded-xl p-4 text-center hover-lift">
                <div class="text-2xl md:text-3xl font-semibold gradient-text" id="followers">--</div>
                <div class="text-xs text-gray-400 mt-1">Followers</div>
            </div>
            <div class="stat-card rounded-xl p-4 text-center hover-lift">
                <div class="text-2xl md:text-3xl font-semibold gradient-text" id="following">--</div>
                <div class="text-xs text-gray-400 mt-1">Following</div>
            </div>
            <div class="stat-card rounded-xl p-4 text-center hover-lift">
                <div class="text-2xl md:text-3xl font-semibold text-orange-400" id="thm-rank">Top 10%</div>
                <div class="text-xs text-gray-400 mt-1">TryHackMe</div>
            </div>
        </div>

        <!-- Skills Section -->
        <section class="card-3d stat-card rounded-2xl p-6 md:p-8 mb-8">
            <div class="flex items-center gap-3 mb-6">
                <span class="iconify text-purple-400" data-icon="lucide:code-2" data-width="24" style="stroke-width: 1.5;"></span>
                <h2 class="text-xl font-semibold tracking-tight">Skills &amp; Technologies</h2>
            </div>
            <div class="space-y-4">
                <div>
                    <div class="flex justify-between text-sm mb-1">
                        <span class="text-gray-300">Python</span>
                        <span class="text-gray-500">85%</span>
                    </div>
                    <div class="h-2 bg-gray-800 rounded-full overflow-hidden">
                        <div class="skill-bar h-full rounded-full" style="width: 85%;"></div>
                    </div>
                </div>
                <div>
                    <div class="flex justify-between text-sm mb-1">
                        <span class="text-gray-300">Linux &amp; Bash</span>
                        <span class="text-gray-500">90%</span>
                    </div>
                    <div class="h-2 bg-gray-800 rounded-full overflow-hidden">
                        <div class="skill-bar h-full rounded-full" style="width: 90%; animation-delay: 0.2s;"></div>
                    </div>
                </div>
                <div>
                    <div class="flex justify-between text-sm mb-1">
                        <span class="text-gray-300">Penetration Testing</span>
                        <span class="text-gray-500">75%</span>
                    </div>
                    <div class="h-2 bg-gray-800 rounded-full overflow-hidden">
                        <div class="skill-bar h-full rounded-full" style="width: 75%; animation-delay: 0.4s;"></div>
                    </div>
                </div>
                <div>
                    <div class="flex justify-between text-sm mb-1">
                        <span class="text-gray-300">Web Development</span>
                        <span class="text-gray-500">70%</span>
                    </div>
                    <div class="h-2 bg-gray-800 rounded-full overflow-hidden">
                        <div class="skill-bar h-full rounded-full" style="width: 70%; animation-delay: 0.6s;"></div>
                    </div>
                </div>
            </div>
            
            <!-- Tech Icons -->
            <div class="flex flex-wrap gap-3 mt-6 pt-6 border-t border-gray-800">
                <div class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover-lift" title="Python">
                    <span class="iconify text-yellow-400" data-icon="logos:python" data-width="24"></span>
                </div>
                <div class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover-lift" title="Linux">
                    <span class="iconify text-white" data-icon="logos:linux-tux" data-width="24"></span>
                </div>
                <div class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover-lift" title="Bash">
                    <span class="iconify text-green-400" data-icon="logos:bash-icon" data-width="24"></span>
                </div>
                <div class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover-lift" title="Git">
                    <span class="iconify" data-icon="logos:git-icon" data-width="24"></span>
                </div>
                <div class="w-10 h-10 rounded-lg bg-gray-800 flex items-center justify-center hover-lift" title="Docker">
                    <span class="iconify" data-icon="logos:docker-icon" data-width="24"></span>
                </div>
            </div>
        </section>

        <!-- TryHackMe Badge -->
        <section class="card-3d stat-card rounded-2xl p-6 md:p-8 mb-8 border-l-4 border-orange-500">
            <div class="flex items-center gap-3 mb-4">
                <div class="w-10 h-10 rounded-lg bg-orange-500/20 flex items-center justify-center">
                    <span class="iconify text-orange-400" data-icon="lucide:shield-check" data-width="24" style="stroke-width: 1.5;"></span>
                </div>
                <div>
                    <h2 class="text-xl font-semibold tracking-tight">TryHackMe</h2>
                    <p class="text-sm text-gray-400">@Subhajit1</p>
                </div>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mt-4">
                <div class="text-center p-3 bg-gray-800/50 rounded-lg">
                    <div class="text-lg font-semibold text-orange-400">50+</div>
                    <div class="text-xs text-gray-500">Rooms Completed</div>
                </div>
                <div class="text-center p-3 bg-gray-800/50 rounded-lg">
                    <div class="text-lg font-semibold text-orange-400">Active</div>
                    <div class="text-xs text-gray-500">Status</div>
                </div>
                <div class="text-center p-3 bg-gray-800/50 rounded-lg">
                    <div class="text-lg font-semibold text-orange-400">CTF</div>
                    <div class="text-xs text-gray-500">Focus</div>
                </div>
                <div class="text-center p-3 bg-gray-800/50 rounded-lg">
                    <div class="text-lg font-semibold text-orange-400">🏆</div>
                    <div class="text-xs text-gray-500">Achievements</div>
                </div>
            </div>
        </section>

        <!-- Connect Section -->
        <section class="stat-card rounded-2xl p-6 md:p-8 mb-8">
            <div class="flex items-center gap-3 mb-6">
                <span class="iconify text-green-400" data-icon="lucide:link" data-width="24" style="stroke-width: 1.5;"></span>
                <h2 class="text-xl font-semibold tracking-tight">Connect With Me</h2>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                <a href="https://github.com/subhajit-sudo" target="_blank" class="flex items-center gap-3 p-4 bg-gray-800/50 rounded-xl hover-lift border border-gray-700 hover:border-gray-600 transition-all">
                    <span class="iconify text-white" data-icon="lucide:github" data-width="24" style="stroke-width: 1.5;"></span>
                    <div>
                        <div class="text-sm font-medium">GitHub</div>
                        <div class="text-xs text-gray-500">@subhajit-sudo</div>
                    </div>
                </a>
                <a href="https://www.facebook.com/subhajitnandi64" target="_blank" class="flex items-center gap-3 p-4 bg-gray-800/50 rounded-xl hover-lift border border-gray-700 hover:border-blue-600 transition-all">
                    <span class="iconify text-blue-500" data-icon="lucide:facebook" data-width="24" style="stroke-width: 1.5;"></span>
                    <div>
                        <div class="text-sm font-medium">Facebook</div>
                        <div class="text-xs text-gray-500">Subhajit Nandi</div>
                    </div>
                </a>
                <a href="https://tryhackme.com/p/Subhajit1" target="_blank" class="flex items-center gap-3 p-4 bg-gray-800/50 rounded-xl hover-lift border border-gray-700 hover:border-orange-600 transition-all">
                    <span class="iconify text-orange-500" data-icon="lucide:shield" data-width="24" style="stroke-width: 1.5;"></span>
                    <div>
                        <div class="text-sm font-medium">TryHackMe</div>
                        <div class="text-xs text-gray-500">@Subhajit1</div>
                    </div>
                </a>
            </div>
        </section>

        <!-- GitHub Activity Graph Placeholder -->
        <section class="stat-card rounded-2xl p-6 md:p-8 mb-8">
            <div class="flex items-center gap-3 mb-6">
                <span class="iconify text-blue-400" data-icon="lucide:activity" data-width="24" style="stroke-width: 1.5;"></span>
                <h2 class="text-xl font-semibold tracking-tight">Contribution Graph</h2>
            </div>
            <div class="overflow-x-auto">
                <div id="contribution-graph" class="flex gap-1 min-w-max py-2">
                    <!-- Generated by JS -->
                </div>
            </div>
            <div class="flex justify-end items-center gap-2 mt-4 text-xs text-gray-500">
                <span>Less</span>
                <div class="flex gap-1">
                    <div class="w-3 h-3 rounded-sm bg-gray-800"></div>
                    <div class="w-3 h-3 rounded-sm bg-green-900"></div>
                    <div class="w-3 h-3 rounded-sm bg-green-700"></div>
                    <div class="w-3 h-3 rounded-sm bg-green-500"></div>
                    <div class="w-3 h-3 rounded-sm bg-green-400"></div>
                </div>
                <span>More</span>
            </div>
        </section>

        <!-- Footer -->
        <footer class="text-center py-8">
            <p class="text-sm text-gray-500">
                ⚡ Made with passion by <span class="text-blue-400">Subhajit Nandi</span>
            </p>
            <p class="text-xs text-gray-600 mt-2">Last updated: 2025</p>
        </footer>
    </div>

    <script>
        // Fetch GitHub Data
        async function fetchGitHubData() {
            try {
                const response = await fetch('https://api.github.com/users/subhajit-sudo');
                const data = await response.json();
                
                document.getElementById('repos').textContent = data.public_repos || '0';
                document.getElementById('followers').textContent = data.followers || '0';
                document.getElementById('following').textContent = data.following || '0';
            } catch (error) {
                console.log('Could not fetch GitHub data');
            }
        }
        
        fetchGitHubData();

        // Generate Contribution Graph
        function generateContributionGraph() {
            const graph = document.getElementById('contribution-graph');
            const weeks = 52;
            const days = 7;
            const colors = ['bg-gray-800', 'bg-green-900', 'bg-green-700', 'bg-green-500', 'bg-green-400'];
            
            for (let w = 0; w < weeks; w++) {
                const week = document.createElement('div');
                week.className = 'flex flex-col gap-1';
                
                for (let d = 0; d < days; d++) {
                    const day = document.createElement('div');
                    const intensity = Math.floor(Math.random() * 5);
                    day.className = `w-3 h-3 rounded-sm ${colors[intensity]} hover:ring-1 hover:ring-blue-400 transition-all cursor-pointer`;
                    day.title = `${Math.floor(Math.random() * 10)} contributions`;
                    week.appendChild(day);
                }
                
                graph.appendChild(week);
            }
        }
        
        generateContributionGraph();

        // Generate Particles
        function createParticles() {
            const container = document.getElementById('particles');
            for (let i = 0; i < 20; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.left = `${Math.random() * 100}%`;
                particle.style.top = `${Math.random() * 100 + 100}%`;
                particle.style.animationDelay = `${Math.random() * 10}s`;
                particle.style.animationDuration = `${10 + Math.random() * 10}s`;
                container.appendChild(particle);
            }
        }
        
        createParticles();

        // 3D Card Effect
        document.querySelectorAll('.card-3d').forEach(card => {
            card.addEventListener('mousemove', (e) => {
                const rect = card.getBoundingClientRect();
                const x = e.clientX - rect.left;
                const y = e.clientY - rect.top;
                const centerX = rect.width / 2;
                const centerY = rect.height / 2;
                const rotateX = (y - centerY) / 20;
                const rotateY = (centerX - x) / 20;
                
                card.style.transform = `perspective(1000px) rotateX(${rotateX}deg) rotateY(${rotateY}deg) translateZ(10px)`;
            });
            
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'perspective(1000px) rotateX(0) rotateY(0) translateZ(0)';
            });
        });
    </script>

</body></html>
