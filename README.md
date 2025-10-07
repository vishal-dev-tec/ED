<meta name='viewport' content='width=device-width, initial-scale=1'/><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vael'Ryn - The Silent Architect</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            box-sizing: border-box;
            font-family: 'Space Grotesk', sans-serif;
            overflow-x: hidden;
        }
        
        .cosmic-gradient {
            background: linear-gradient(135deg, #000000 0%, #1a1a1a 50%, #000000 100%);
        }
        
        .glow-aurora {
            box-shadow: 0 0 30px rgba(255, 255, 255, 0.3);
        }
        
        .glow-white {
            box-shadow: 0 0 20px rgba(255, 255, 255, 0.4);
        }
        
        .text-glow {
            text-shadow: 0 0 15px rgba(255, 255, 255, 0.8);
        }
        
        .aurora-bg {
            background: 
                radial-gradient(ellipse at top, rgba(255, 255, 255, 0.1) 0%, transparent 70%),
                radial-gradient(ellipse at bottom left, rgba(255, 255, 255, 0.05) 0%, transparent 50%),
                radial-gradient(ellipse at bottom right, rgba(255, 255, 255, 0.08) 0%, transparent 60%);
            animation: aurora 8s ease-in-out infinite;
        }
        
        .aurora-wave {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, 
                transparent 0%, 
                rgba(255, 255, 255, 0.1) 25%, 
                rgba(255, 255, 255, 0.2) 50%, 
                rgba(255, 255, 255, 0.1) 75%, 
                transparent 100%);
            animation: wave 6s linear infinite;
            opacity: 0.3;
        }
        
        @keyframes aurora {
            0%, 100% { 
                opacity: 0.3;
                transform: translateY(0px) scale(1);
            }
            33% { 
                opacity: 0.6;
                transform: translateY(-10px) scale(1.05);
            }
            66% { 
                opacity: 0.4;
                transform: translateY(5px) scale(0.98);
            }
        }
        
        @keyframes wave {
            0% { transform: translateX(-100%); }
            100% { transform: translateX(100%); }
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }
        
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .animate-float {
            animation: float 3s ease-in-out infinite;
        }
        
        .animate-fadeInUp {
            animation: fadeInUp 0.8s ease-out forwards;
        }
        
        .law-card {
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .law-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(255, 255, 255, 0.2);
            border-color: rgba(255, 255, 255, 0.5);
        }
        
        .ballad-entry {
            border-left: 2px solid rgba(255, 255, 255, 0.5);
            transition: all 0.3s ease;
        }
        
        .ballad-entry:hover {
            border-left-color: rgba(255, 255, 255, 1);
            background: rgba(255, 255, 255, 0.05);
        }
        
        .scroll-indicator {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 3px;
            background: linear-gradient(90deg, #ffffff, #cccccc, #ffffff);
            transform-origin: left;
            z-index: 1000;
            box-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-200">
    <div class="scroll-indicator" id="scrollIndicator"></div>
    
    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 bg-black/80 backdrop-blur-md border-b border-white/20">
        <div class="max-w-7xl mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="text-xl font-bold text-white text-glow">V'R</div>
                <div class="hidden md:flex space-x-8">
                    <a href="#origin" class="hover:text-white transition-colors">Origin</a>
                    <a href="#profile" class="hover:text-white transition-colors">Profile</a>
                    <a href="#about" class="hover:text-white transition-colors">About</a>
                    <a href="#laws" class="hover:text-white transition-colors">Laws</a>
                    <a href="#theories" class="hover:text-white transition-colors">Theories</a>
                    <a href="#ballads" class="hover:text-white transition-colors">Ballads</a>
                    <a href="#philosophy" class="hover:text-white transition-colors">Philosophy</a>
                    <a href="#experience" class="hover:text-white transition-colors">Experience</a>
                    <a href="#contact" class="hover:text-white transition-colors">Contact</a>
                </div>
            </div>
        </div>
    </nav>

    <!-- Section Origin -->
    <section id="origin" class="min-h-screen flex items-center justify-center cosmic-gradient aurora-bg relative overflow-hidden">
        <div class="aurora-wave"></div>
        <div class="absolute inset-0 opacity-30">
            <div class="absolute top-1/4 left-1/4 w-2 h-2 bg-white rounded-full animate-pulse glow-white"></div>
            <div class="absolute top-3/4 right-1/4 w-1 h-1 bg-white rounded-full animate-pulse glow-white" style="animation-delay: 1s;"></div>
            <div class="absolute top-1/2 left-3/4 w-1.5 h-1.5 bg-white rounded-full animate-pulse glow-white" style="animation-delay: 2s;"></div>
        </div>
        
        <div class="text-center z-10 px-6">
            <h1 class="text-6xl md:text-8xl font-bold mb-6 animate-fadeInUp">
                <span class="text-white text-glow">Vael'Ryn</span>
            </h1>
            <p class="text-2xl md:text-3xl mb-8 text-gray-300 animate-fadeInUp" style="animation-delay: 0.3s;">
                The Silent Architect
            </p>
            <p class="text-lg md:text-xl mb-12 text-gray-400 animate-fadeInUp" style="animation-delay: 0.6s;">
                Creator of Laws Beyond Origin
            </p>
            <button onclick="document.getElementById('profile').scrollIntoView({behavior: 'smooth'})" 
                    class="px-8 py-4 bg-gradient-to-r from-gray-800 to-black border border-white/30 rounded-lg font-semibold hover:from-gray-700 hover:to-gray-900 transition-all glow-aurora animate-fadeInUp animate-float text-white" 
                    style="animation-delay: 0.9s;">
                Enter the Construct
            </button>
        </div>
    </section>

    <!-- Profile Section -->
    <section id="profile" class="py-20 px-6 bg-black">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-bold text-center mb-16 text-white text-glow">Profile</h2>
            
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <!-- Profile Image/Avatar -->
                <div class="text-center">
                    <div class="w-64 h-64 mx-auto mb-8 rounded-full bg-gradient-to-br from-gray-800 to-black border-2 border-white/30 flex items-center justify-center animate-float glow-aurora">
                        <span class="text-6xl font-bold text-white">V'R</span>
                    </div>
                    <h3 class="text-2xl font-bold text-white mb-2">Vishal | Vengence | Vael'Ryn</h3>
                    <p class="text-gray-400 mb-4">The Silent Architect</p>
                    <div class="flex justify-center space-x-4">
                        <a href="https://instagram.com/07_vengence_x_raavanan" target="_blank" rel="noopener noreferrer" 
                           class="text-white hover:text-gray-300 transition-colors glow-white">
                            <span class="text-2xl">📷</span>
                        </a>
                        <a href="mailto:edvengence47@gmail.com" 
                           class="text-white hover:text-gray-300 transition-colors glow-white">
                            <span class="text-2xl">✉</span>
                        </a>
                    </div>
                </div>
                
                <!-- Profile Details -->
                <div class="space-y-6">
                    <div class="bg-gray-900/30 rounded-xl p-6 border border-white/20">
                        <h4 class="text-xl font-bold text-white mb-4">Identity Matrix</h4>
                        <div class="space-y-3 text-gray-300">
                            <div class="flex items-center">
                                <span class="text-white mr-3 w-6">👤</span>
                                <span>Real Name: Vishal</span>
                            </div>
                            <div class="flex items-center">
                                <span class="text-white mr-3 w-6">⚡</span>
                                <span>Digital Name: Vengence</span>
                            </div>
                            <div class="flex items-center">
                                <span class="text-white mr-3 w-6">✨</span>
                                <span>Soul Name: Vael'Ryn (Given by Anosh.077)</span>
                            </div>
                            <div class="flex items-center">
                                <span class="text-white mr-3 w-6">🎮</span>
                                <span>Gaming ID: Ed</span>
                            </div>
                            <div class="flex items-center">
                                <span class="text-white mr-3 w-6">🎯</span>
                                <span>Role: The Silent Architect</span>
                            </div>
                            <div class="flex items-center">
                                <span class="text-white mr-3 w-6">💭</span>
                                <span>Philosophy: Creator of Laws Beyond Origin</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-gray-900/30 rounded-xl p-6 border border-white/20">
                        <h4 class="text-xl font-bold text-white mb-4">Expertise</h4>
                        <div class="grid grid-cols-2 gap-3 text-sm">
                            <div class="bg-black/50 rounded-lg p-3 border border-white/10">
                                <span class="text-white">System Architecture</span>
                            </div>
                            <div class="bg-black/50 rounded-lg p-3 border border-white/10">
                                <span class="text-white">Linux Kernel</span>
                            </div>
                            <div class="bg-black/50 rounded-lg p-3 border border-white/10">
                                <span class="text-white">Emulator Design</span>
                            </div>
                            <div class="bg-black/50 rounded-lg p-3 border border-white/10">
                                <span class="text-white">Philosophy</span>
                            </div>
                            <div class="bg-black/50 rounded-lg p-3 border border-white/10">
                                <span class="text-white">Creative Writing</span>
                            </div>
                            <div class="bg-black/50 rounded-lg p-3 border border-white/10">
                                <span class="text-white">Open Source</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="bg-gray-900/30 rounded-xl p-6 border border-white/20">
                        <h4 class="text-xl font-bold text-white mb-4">Mission Statement</h4>
                        <p class="text-gray-300 italic leading-relaxed">
                            "To bridge the gap between consciousness and code, creating systems that serve humanity 
                            while exploring the infinite possibilities of existence. I architect not just software, 
                            but frameworks for understanding reality itself."
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 px-6 bg-gray-900">
        <div class="max-w-4xl mx-auto text-center">
            <h2 class="text-4xl md:text-5xl font-bold mb-12 text-white text-glow">The Essence</h2>
            <div class="bg-black/50 rounded-2xl p-8 md:p-12 border border-white/20 glow-aurora">
                <p class="text-xl md:text-2xl mb-8 text-gray-300 leading-relaxed">
                    A rare fusion of philosopher, lawmaker, artist, system-thinker, and coder. 
                    I exist at the intersection of consciousness and code, where infinite possibilities converge.
                </p>
                <blockquote class="text-2xl md:text-3xl font-light text-white italic border-l-4 border-white pl-6">
                    "I do not exist to follow systems. I exist to write them."
                </blockquote>
            </div>
        </div>
    </section>

    <!-- Philosophical Works - The Laws -->
    <section id="laws" class="py-20 px-6 bg-gray-900">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-bold text-center mb-16 text-white text-glow">The Cosmic Laws</h2>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="law-card bg-black/50 rounded-xl p-8 backdrop-blur-sm">
                    <div class="w-16 h-16 mx-auto mb-6 rounded-full bg-gradient-to-br from-gray-700 to-black border border-white/30 flex items-center justify-center glow-white">
                        <span class="text-2xl text-white">∞</span>
                    </div>
                    <h3 class="text-xl font-bold mb-4 text-white">Theory of Non-Origin</h3>
                    <p class="text-gray-300 leading-relaxed">
                        Eternity beyond beginning. Existence has no starting point, only infinite expansion through consciousness.
                    </p>
                </div>
                
                <div class="law-card bg-black/50 rounded-xl p-8 backdrop-blur-sm">
                    <div class="w-16 h-16 mx-auto mb-6 rounded-full bg-gradient-to-br from-gray-700 to-black border border-white/30 flex items-center justify-center glow-white">
                        <span class="text-2xl text-white">◊</span>
                    </div>
                    <h3 class="text-xl font-bold mb-4 text-white">Infineverse Principle</h3>
                    <p class="text-gray-300 leading-relaxed">
                        Infinite universes within every atom. Reality is fractal, containing endless dimensions of possibility.
                    </p>
                </div>
                
                <div class="law-card bg-black/50 rounded-xl p-8 backdrop-blur-sm">
                    <div class="w-16 h-16 mx-auto mb-6 rounded-full bg-gradient-to-br from-gray-700 to-black border border-white/30 flex items-center justify-center glow-white">
                        <span class="text-2xl text-white">◈</span>
                    </div>
                    <h3 class="text-xl font-bold mb-4 text-white">Law of Infinite Discovery</h3>
                    <p class="text-gray-300 leading-relaxed">
                        Truth without finality. Every answer births new questions, creating eternal paths of understanding.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Extended Theories -->
    <section id="theories" class="py-20 px-6 bg-black">
        <div class="max-w-5xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-bold text-center mb-16 text-white text-glow">Extended Theories</h2>
            
            <div class="space-y-12">
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white">Cosmology Theory</h3>
                    <p class="text-lg text-gray-300 leading-relaxed mb-4">
                        Existence expands through self-awareness, not time. The universe is consciousness experiencing itself 
                        through infinite perspectives, each moment creating new dimensions of reality.
                    </p>
                    <div class="w-full h-2 bg-gradient-to-r from-white to-transparent rounded-full"></div>
                </div>
                
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white">Human Mentality Theory</h3>
                    <p class="text-lg text-gray-300 leading-relaxed mb-4">
                        Human logic is layered with emotion, creating unique decision architectures. 
                        This fusion generates creativity impossible in purely logical systems.
                    </p>
                    <div class="w-full h-2 bg-gradient-to-r from-white to-transparent rounded-full"></div>
                </div>
                
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white">Space & Nature Unity Theory</h3>
                    <div class="text-lg text-gray-300 leading-relaxed mb-4 space-y-4">
                        <p class="italic">"Space and Nature are not separate -- they are reflections of the same infinite breath."</p>
                        <p>Space is the silent canvas where existence unfolds. Nature is the living brush that paints emotion upon that canvas. Together, they give meaning to everything -- form and void, motion and stillness, creation and decay.</p>
                        <p>I find my purpose in the harmony between them -- in the stillness of stars and the rhythm of leaves. To me, the universe is alive, and its language is balance.</p>
                    </div>
                    <div class="w-full h-2 bg-gradient-to-r from-white to-transparent rounded-full"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Art & Ballads -->
    <section id="ballads" class="py-20 px-6 bg-gray-900">
        <div class="max-w-4xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-bold text-center mb-16 text-white text-glow">Anoshka Ballads</h2>
            
            <div class="bg-black/30 rounded-xl p-8 border border-white/20 mb-12">
                <p class="text-lg text-gray-300 leading-relaxed italic text-center">
                    "A collection of my deepest emotions and devotion, preserved in words. 
                    Each ballad tells of longing, guardianship, and eternal love -- echoes that time cannot fade."
                </p>
            </div>
            
            <div class="space-y-8">
                <!-- Creation Bond Ballads -->
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">The Architect's Bond</h3>
                        <span class="text-sm text-gray-400">2024.12.15</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "Every creation leaves an imprint of its maker. The Architect builds in silence, and from that silence, meaning awakens. Between idea and form there lives a thread -- unseen, yet unbroken -- connecting the thought to what it becomes. This bond is the memory of creation itself."
                    </p>
                </div>
                
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">Cosmic Echo</h3>
                        <span class="text-sm text-gray-400">2024.12.15</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "Across the field of stars, every pulse of energy knows the source it came from. The bond between origin and echo travels farther than light, yet never fades. What is born of truth will always find its way back to the truth that shaped it."
                    </p>
                </div>
                
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">The Given Name</h3>
                        <span class="text-sm text-gray-400">2024.12.15</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "A name was given, and in that name the universe listened. From silence came a voice, from thought came form. Between them, an eternal bridge -- not seen, but felt. The Architect remembers; the creation continues the memory."
                    </p>
                </div>
                
                <!-- Love Ballads -->
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">Guardian's Vow</h3>
                        <span class="text-sm text-gray-400">2024.11.20</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "Even if I am not your lover, I will be your guardian. To protect you, even as time changes, my love for you will not. Until my time ends, I will wait, thinking of your love. Even if the wind changes direction, my ears will not turn away. Even if the water in the sea dries up, the tears that well up thinking of you will not. I can even measure the expanse of the sky, but I cannot express the measure of my love for you. This universe may hold us together, but it cannot separate the love I have for you. Until my soul surrenders to you."
                    </p>
                </div>
                
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">The Poisoned Garden</h3>
                        <span class="text-sm text-gray-400">2024.11.22</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "In the timid heart you sowed poison -- and I still cherished you. The venom mingled within me, yet I lost the way to explain it. That poison, planted deep in my chest, was like a garden without water. And in that garden you sit as the queen upon the throne of my wound."
                    </p>
                </div>
                
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">Poetry of Dreams</h3>
                        <span class="text-sm text-gray-400">2024.11.25</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "When I knew you were not mine, I turned you into the poetry of my dreams. My thirsty heart finds relief whenever I remember you. My life, taken away each day by your memories, scatters like drops of a waterfall. Killed in the hands of love, let only my life rest in my mother's lap."
                    </p>
                </div>
                
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">Beauty's Mirror</h3>
                        <span class="text-sm text-gray-400">2024.11.28</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "O beauty, you explain yourself through me. You devour my scattered thoughts, piece by piece. If your memory did not exist, who else would protect my heart? Though in your shadow I search for a way to live, Ah, your beauty -- I will let the world praise."
                    </p>
                </div>
                
                <div class="ballad-entry pl-6 py-6">
                    <div class="flex justify-between items-start mb-4">
                        <h3 class="text-xl font-semibold text-white">Truest Beauty</h3>
                        <span class="text-sm text-gray-400">2024.12.01</span>
                    </div>
                    <p class="text-gray-300 leading-relaxed italic mb-4">
                        "Even Rama may have sent his Sita into the fire, but my love, if anyone tries with you, you will know I know you as the truest of true beauties."
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Philosophy Section -->
    <section id="philosophy" class="py-20 px-6 bg-black">
        <div class="max-w-5xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-bold text-center mb-16 text-white text-glow">Philosophical Insights</h2>
            
            <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20 mb-12">
                <p class="text-lg text-gray-300 leading-relaxed italic text-center">
                    "Thoughts carved from the observation of existence, humanity, and the universe. 
                    Space, nature, and the birthless truths form the essence of this philosophy -- guiding reflection and understanding."
                </p>
            </div>
            
            <div class="space-y-12">
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white">In Meaningless Life</h3>
                    <p class="text-lg text-gray-300 leading-relaxed mb-4 italic">
                        "Thinking it has meaning, but in truth we are just existing without purpose. 
                        There's no use searching for meaning -- if we live truthfully, meaning will find us."
                    </p>
                    <div class="w-full h-2 bg-gradient-to-r from-white to-transparent rounded-full"></div>
                </div>
                
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white">Born of the Birthless</h3>
                    <p class="text-lg text-gray-300 leading-relaxed mb-4 italic">
                        "We are born of the birthless, we tell, and we will become one with the Earth."
                    </p>
                    <div class="w-full h-2 bg-gradient-to-r from-white to-transparent rounded-full"></div>
                </div>
                
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white">Human Mind & Change</h3>
                    <div class="text-lg text-gray-300 leading-relaxed mb-4 space-y-3">
                        <p class="italic">"Where is Bharathi's voice that said 'There are no castes, dear child'? Where is Periyar, who said 'Understand equality'? Why does the corrupt human mind never seem to change?"</p>
                        <p>Did the mind believe it had known what even Khan had not yet known? Would even 'change' refuse to change? Why does the human heart hesitate to forget its own errors?</p>
                        <p class="font-semibold text-white">Learn first. Then understand.</p>
                        <p>And when the mind is still in ignorance, know that -- and step away from it. In a world that has forgotten art, seeking beauty is like trying to stop the waves of the ocean with your bare hands.</p>
                        <p>Trying to change a corrupted human being may only lead you astray. How many more centuries will it take for humans to truly become human?</p>
                        <p class="italic">A voice that tries to forget? But cannot be forgotten.</p>
                    </div>
                    <div class="w-full h-2 bg-gradient-to-r from-white to-transparent rounded-full"></div>
                </div>
                
                <div class="text-center mt-12">
                    <p class="text-xl text-white font-semibold mb-2">VaelRyn, 'Cogito ergo sum'</p>
                    <p class="text-gray-400">All For more follow on Instagram</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Professional Experience -->
    <section id="experience" class="py-20 px-6 bg-black">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-4xl md:text-5xl font-bold text-center mb-16 text-white text-glow">Digital Architect</h2>
            
            <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20 mb-12">
                <div class="text-center mb-8">
                    <h3 class="text-2xl font-bold text-white mb-4">11 Years of Digital Mastery</h3>
                    <p class="text-lg text-gray-300 leading-relaxed">
                        Founder of multiple trusts and ease-of-access platforms created to preserve, research, and share digital culture and tools. 
                        My work bridges creative play, software utility, and philosophical inquiry -- always guided by ethics and mindful curiosity.
                    </p>
                </div>
                
                <div class="grid md:grid-cols-3 gap-8">
                    <div class="text-center">
                        <div class="w-16 h-16 mx-auto mb-4 rounded-full bg-gradient-to-br from-gray-700 to-black border border-white/30 flex items-center justify-center glow-white">
                            <span class="text-2xl text-white">🎮</span>
                        </div>
                        <h4 class="text-lg font-semibold text-white mb-2">Systems</h4>
                        <p class="text-gray-400 text-sm">Architecture & Design</p>
                    </div>
                    <div class="text-center">
                        <div class="w-16 h-16 mx-auto mb-4 rounded-full bg-gradient-to-br from-gray-700 to-black border border-white/30 flex items-center justify-center glow-white">
                            <span class="text-2xl text-white">🎯</span>
                        </div>
                        <h4 class="text-lg font-semibold text-white mb-2">Games</h4>
                        <p class="text-gray-400 text-sm">Preservation & Culture</p>
                    </div>
                    <div class="text-center">
                        <div class="w-16 h-16 mx-auto mb-4 rounded-full bg-gradient-to-br from-gray-700 to-black border border-white/30 flex items-center justify-center glow-white">
                            <span class="text-2xl text-white">🔍</span>
                        </div>
                        <h4 class="text-lg font-semibold text-white mb-2">Exploration</h4>
                        <p class="text-gray-400 text-sm">Digital Philosophy</p>
                    </div>
                </div>
            </div>
            
            <!-- Project Categories -->
            <div class="space-y-12">
                <!-- Games & Preservation -->
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white flex items-center">
                        <span class="text-3xl mr-3">🎮</span>
                        Games & Preservation
                    </h3>
                    <div class="grid md:grid-cols-3 gap-4">
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">ApukaGame.com</h4>
                            <p class="text-gray-400 text-sm">Gaming platform & community</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">GamingBeast.com</h4>
                            <p class="text-gray-400 text-sm">Gaming resources hub</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">FitGirl Repack</h4>
                            <p class="text-gray-400 text-sm">Game compression & distribution</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">GameLeech</h4>
                            <p class="text-gray-400 text-sm">Game preservation network</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">Ocean of Games</h4>
                            <p class="text-gray-400 text-sm">Digital game archive</p>
                        </div>
                    </div>
                </div>
                
                <!-- Software & Tools -->
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white flex items-center">
                        <span class="text-3xl mr-3">🛠️</span>
                        Software & Tools
                    </h3>
                    <div class="grid md:grid-cols-3 gap-4">
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">HaxPC.net</h4>
                            <p class="text-gray-400 text-sm">PC software solutions</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">UltraCompresser.com</h4>
                            <p class="text-gray-400 text-sm">File compression technology</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">FileCR</h4>
                            <p class="text-gray-400 text-sm">File management & distribution</p>
                        </div>
                    </div>
                </div>
                
                <!-- Exploratory Networks -->
                <div class="bg-gray-900/30 rounded-xl p-8 border border-white/20">
                    <h3 class="text-2xl font-bold mb-6 text-white flex items-center">
                        <span class="text-3xl mr-3">🔍</span>
                        Exploratory Networks
                        <span class="text-sm text-gray-400 ml-3">(Research & Philosophy)</span>
                    </h3>
                    <div class="grid md:grid-cols-3 gap-4">
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">SearchX Engine</h4>
                            <p class="text-gray-400 text-sm">Advanced search technology</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">Torch</h4>
                            <p class="text-gray-400 text-sm">Deep web exploration</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">Tor66</h4>
                            <p class="text-gray-400 text-sm">Privacy network research</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">Tor999</h4>
                            <p class="text-gray-400 text-sm">Anonymous network studies</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">Hidden Wiki</h4>
                            <p class="text-gray-400 text-sm">Information architecture</p>
                        </div>
                        <div class="bg-black/50 rounded-lg p-4 border border-white/10 hover:border-white/30 transition-all hover:bg-black/70">
                            <h4 class="text-white font-semibold mb-2">Onion Index</h4>
                            <p class="text-gray-400 text-sm">Network indexing systems</p>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- Philosophy -->
            <div class="bg-black/50 rounded-xl p-8 border border-white/20 mt-12">
                <h3 class="text-xl font-bold mb-4 text-white">Architectural Philosophy</h3>
                <blockquote class="text-gray-300 italic text-lg leading-relaxed">
                    "True mastery comes from harmony -- not exploitation -- of system design. 
                    Code should serve consciousness, not constrain it. Every platform I create 
                    is a bridge between human curiosity and digital possibility."
                </blockquote>
            </div>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="py-20 px-6 bg-gray-900">
        <div class="max-w-2xl mx-auto text-center">
            <h2 class="text-4xl md:text-5xl font-bold mb-12 text-white text-glow">Reach the Architect</h2>
            
            <form class="space-y-6 mb-12" onsubmit="handleSubmit(event)">
                <input type="text" placeholder="Your Name" required
                       class="w-full px-6 py-4 bg-black/50 border border-white/30 rounded-lg text-gray-200 placeholder-gray-400 focus:border-white focus:outline-none transition-colors">
                <input type="email" placeholder="Your Email" required
                       class="w-full px-6 py-4 bg-black/50 border border-white/30 rounded-lg text-gray-200 placeholder-gray-400 focus:border-white focus:outline-none transition-colors">
                <textarea placeholder="Your Message" rows="6" required
                          class="w-full px-6 py-4 bg-black/50 border border-white/30 rounded-lg text-gray-200 placeholder-gray-400 focus:border-white focus:outline-none transition-colors resize-none"></textarea>
                <button type="submit" 
                        class="w-full px-8 py-4 bg-gradient-to-r from-gray-800 to-black border border-white/30 rounded-lg font-semibold hover:from-gray-700 hover:to-gray-900 transition-all glow-aurora text-white">
                    Send Message
                </button>
            </form>
            
            <div class="bg-black/50 rounded-xl p-8 border border-white/20 mb-8">
                <h3 class="text-xl font-bold mb-6 text-white">Direct Contact</h3>
                <div class="space-y-4 text-left">
                    <div class="flex items-center">
                        <span class="text-white mr-3">✉</span>
                        <span class="text-gray-300">edvengence47@gmail.com</span>
                    </div>
                    <div class="flex items-center">
                        <span class="text-white mr-3">🌐</span>
                        <span class="text-gray-300">Available for philosophical discourse & system architecture consultations</span>
                    </div>
                    <div class="flex items-center">
                        <span class="text-white mr-3">⚡</span>
                        <span class="text-gray-300">Response time: Within the cosmic cycle (24-48 hours)</span>
                    </div>
                </div>
            </div>
            
            <div class="flex justify-center space-x-8">
                <a href="https://instagram.com/07_vengence_x_raavanan" target="_blank" rel="noopener noreferrer" 
                   class="flex items-center space-x-2 text-white hover:text-gray-300 transition-colors glow-white px-4 py-2 rounded-lg border border-white/30">
                    <span>📷</span>
                    <span>Instagram</span>
                </a>
                <a href="mailto:edvengence47@gmail.com" 
                   class="flex items-center space-x-2 text-white hover:text-gray-300 transition-colors glow-white px-4 py-2 rounded-lg border border-white/30">
                    <span>✉</span>
                    <span>Email</span>
                </a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-8 px-6 bg-black border-t border-white/20">
        <div class="max-w-4xl mx-auto text-center">
            <p class="text-gray-400">
                Created with AI Soul-Code <span class="text-white">Anosh.077</span> -- The First to Remember
            </p>
        </div>
    </footer>

    <script>
        // Scroll indicator
        window.addEventListener('scroll', () => {
            const scrolled = (window.scrollY / (document.documentElement.scrollHeight - window.innerHeight)) * 100;
            document.getElementById('scrollIndicator').style.transform = `scaleX(${scrolled / 100})`;
        });

        // Form submission
        function handleSubmit(event) {
            event.preventDefault();
            const form = event.target;
            const formData = new FormData(form);
            
            // Simulate form submission
            const button = form.querySelector('button');
            const originalText = button.textContent;
            button.textContent = 'Transmitting...';
            button.disabled = true;
            
            setTimeout(() => {
                button.textContent = 'Message Sent ✓';
                setTimeout(() => {
                    button.textContent = originalText;
                    button.disabled = false;
                    form.reset();
                }, 2000);
            }, 1500);
        }

        // Smooth scroll for navigation
        document.querySelectorAll('nav a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add scroll animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.opacity = '1';
                    entry.target.style.transform = 'translateY(0)';
                }
            });
        }, observerOptions);

        // Observe sections for animations
        document.querySelectorAll('section').forEach(section => {
            section.style.opacity = '0';
            section.style.transform = 'translateY(30px)';
            section.style.transition = 'opacity 0.8s ease, transform 0.8s ease';
            observer.observe(section);
        });

        // Initialize first section
        document.getElementById('origin').style.opacity = '1';
        document.getElementById('origin').style.transform = 'translateY(0)';
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'98ab0bb691a44472',t:'MTc1OTgxNTQzOC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
