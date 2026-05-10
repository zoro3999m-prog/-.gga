<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>UBARS - مملكة نقابات الأنمي</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800;900&family=Cairo:wght@400;600;700;800;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        'tajawal': ['Tajawal', 'sans-serif'],
                        'cairo': ['Cairo', 'sans-serif'],
                    },
                    colors: {
                        'royal-gold': '#D4AF37',
                        'deep-gold': '#B8860B',
                        'light-gold': '#FFD700',
                        'royal-purple': '#4B0082',
                        'deep-purple': '#2E0059',
                        'anime-red': '#DC143C',
                        'anime-blue': '#1E90FF',
                        'dark-void': '#0A0A0F',
                        'void-card': '#12121A',
                    },
                    animation: {
                        'float': 'float 6s ease-in-out infinite',
                        'pulse-glow': 'pulseGlow 3s ease-in-out infinite',
                        'shimmer': 'shimmer 3s linear infinite',
                        'fade-in-up': 'fadeInUp 0.8s ease-out forwards',
                        'glow-pulse': 'glowPulse 2s ease-in-out infinite',
                        'spin-slow': 'spin 8s linear infinite',
                        'bounce-gentle': 'bounceGentle 2s ease-in-out infinite',
                    },
                    keyframes: {
                        float: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-20px)' },
                        },
                        pulseGlow: {
                            '0%, 100%': { boxShadow: '0 0 20px rgba(212, 175, 55, 0.3)' },
                            '50%': { boxShadow: '0 0 40px rgba(212, 175, 55, 0.6)' },
                        },
                        shimmer: {
                            '0%': { backgroundPosition: '-1000px 0' },
                            '100%': { backgroundPosition: '1000px 0' },
                        },
                        fadeInUp: {
                            '0%': { opacity: '0', transform: 'translateY(30px)' },
                            '100%': { opacity: '1', transform: 'translateY(0)' },
                        },
                        glowPulse: {
                            '0%, 100%': { opacity: '0.5' },
                            '50%': { opacity: '1' },
                        },
                        bounceGentle: {
                            '0%, 100%': { transform: 'translateY(0)' },
                            '50%': { transform: 'translateY(-10px)' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        body { 
            font-family: 'Cairo', 'Tajawal', sans-serif; 
            background: #0A0A0F;
            overflow-x: hidden;
        }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar { width: 8px; }
        ::-webkit-scrollbar-track { background: #0A0A0F; }
        ::-webkit-scrollbar-thumb { background: #D4AF37; border-radius: 4px; }
        ::-webkit-scrollbar-thumb:hover { background: #FFD700; }

        .glass-card {
            background: rgba(18, 18, 26, 0.8);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(212, 175, 55, 0.15);
        }
        
        .glass-nav {
            background: rgba(10, 10, 15, 0.9);
            backdrop-filter: blur(20px);
            border-bottom: 1px solid rgba(212, 175, 55, 0.1);
        }

        .gradient-text {
            background: linear-gradient(135deg, #FFD700 0%, #D4AF37 50%, #B8860B 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .gradient-text-purple {
            background: linear-gradient(135deg, #9370DB 0%, #4B0082 50%, #8A2BE2 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .hero-gradient {
            background: 
                radial-gradient(ellipse at top right, rgba(75, 0, 130, 0.3) 0%, transparent 50%),
                radial-gradient(ellipse at bottom left, rgba(212, 175, 55, 0.15) 0%, transparent 50%),
                linear-gradient(to bottom, #0A0A0F 0%, #12121A 100%);
        }

        .gold-border {
            position: relative;
        }
        .gold-border::before {
            content: '';
            position: absolute;
            inset: -2px;
            background: linear-gradient(135deg, #D4AF37, #FFD700, #B8860B, #D4AF37);
            border-radius: inherit;
            z-index: -1;
            opacity: 0;
            transition: opacity 0.3s;
        }
        .gold-border:hover::before {
            opacity: 1;
        }

        .crown-icon {
            filter: drop-shadow(0 0 10px rgba(212, 175, 55, 0.5));
        }

        .anime-card {
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            overflow: hidden;
        }
        .anime-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 25px 50px rgba(212, 175, 55, 0.2);
        }
        .anime-card:hover .anime-overlay {
            opacity: 1;
        }
        .anime-card:hover img {
            transform: scale(1.1);
        }

        .guild-card {
            transition: all 0.4s ease;
            background: linear-gradient(135deg, rgba(18,18,26,0.9) 0%, rgba(46,0,89,0.3) 100%);
        }
        .guild-card:hover {
            transform: translateY(-8px);
            border-color: rgba(212, 175, 55, 0.4);
            box-shadow: 0 20px 40px rgba(75, 0, 130, 0.3);
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: #D4AF37;
            border-radius: 50%;
            animation: particle-float 10s infinite linear;
            opacity: 0.6;
        }
        @keyframes particle-float {
            0% { transform: translateY(100vh) translateX(0); opacity: 0; }
            10% { opacity: 0.6; }
            90% { opacity: 0.6; }
            100% { transform: translateY(-100px) translateX(100px); opacity: 0; }
        }

        .scroll-reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease-out;
        }
        .scroll-reveal.revealed {
            opacity: 1;
            transform: translateY(0);
        }

        .typing-cursor::after {
            content: '|';
            animation: blink 1s infinite;
            color: #D4AF37;
        }
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }

        .rank-badge {
            background: linear-gradient(135deg, #D4AF37, #B8860B);
            clip-path: polygon(0 0, 100% 0, 100% 75%, 50% 100%, 0 75%);
        }

        .mobile-menu {
            transform: translateX(100%);
            transition: transform 0.3s ease-in-out;
        }
        .mobile-menu.active {
            transform: translateX(0);
        }

        .whatsapp-btn {
            background: linear-gradient(135deg, #25D366, #128C7E);
            box-shadow: 0 10px 30px rgba(37, 211, 102, 0.3);
        }
        .whatsapp-btn:hover {
            box-shadow: 0 15px 40px rgba(37, 211, 102, 0.5);
            transform: translateY(-3px);
        }

        /* Glitch effect for title */
        .glitch {
            position: relative;
        }
        .glitch::before,
        .glitch::after {
            content: attr(data-text);
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
        }
        .glitch::before {
            animation: glitch-1 2s infinite linear alternate-reverse;
            color: #DC143C;
            z-index: -1;
        }
        .glitch::after {
            animation: glitch-2 3s infinite linear alternate-reverse;
            color: #1E90FF;
            z-index: -2;
        }
        @keyframes glitch-1 {
            0%, 100% { clip-path: inset(0 0 0 0); transform: translate(0); }
            20% { clip-path: inset(20% 0 60% 0); transform: translate(-3px, 3px); }
            40% { clip-path: inset(40% 0 40% 0); transform: translate(3px, -3px); }
            60% { clip-path: inset(60% 0 20% 0); transform: translate(-3px, 3px); }
            80% { clip-path: inset(80% 0 0% 0); transform: translate(3px, -3px); }
        }
        @keyframes glitch-2 {
            0%, 100% { clip-path: inset(0 0 0 0); transform: translate(0); }
            20% { clip-path: inset(60% 0 20% 0); transform: translate(3px, -3px); }
            40% { clip-path: inset(40% 0 40% 0); transform: translate(-3px, 3px); }
            60% { clip-path: inset(20% 0 60% 0); transform: translate(3px, -3px); }
            80% { clip-path: inset(0% 0 80% 0); transform: translate(-3px, 3px); }
        }
    </style>
</head>
<body class="text-white">

    <!-- Floating Particles -->
    <div id="particles" class="fixed inset-0 pointer-events-none z-0"></div>

    <!-- Navigation -->
    <nav class="fixed top-0 w-full z-50 glass-nav">
        <div class="container mx-auto px-6 py-4 flex justify-between items-center">
            <div class="flex items-center gap-3">
                <div class="w-12 h-12 bg-gradient-to-br from-royal-gold to-deep-gold rounded-xl flex items-center justify-center shadow-lg shadow-royal-gold/30 crown-icon">
                    <i class="fas fa-crown text-white text-xl"></i>
                </div>
                <div>
                    <span class="text-2xl font-black tracking-wider font-cairo gradient-text">UBARS</span>
                    <span class="block text-xs text-royal-gold/70 -mt-1">مملكة نقابات الأنمي</span>
                </div>
            </div>
            
            <div class="hidden lg:flex items-center gap-8 text-gray-300">
                <a href="#home" class="hover:text-royal-gold transition-colors duration-300 text-sm font-bold">الرئيسية</a>
                <a href="#about" class="hover:text-royal-gold transition-colors duration-300 text-sm font-bold">عن المملكة</a>
                <a href="#guilds" class="hover:text-royal-gold transition-colors duration-300 text-sm font-bold">النقابات</a>
                <a href="#ranking" class="hover:text-royal-gold transition-colors duration-300 text-sm font-bold">التصنيف</a>
                <a href="#events" class="hover:text-royal-gold transition-colors duration-300 text-sm font-bold">الفعاليات</a>
                <a href="#rules" class="hover:text-royal-gold transition-colors duration-300 text-sm font-bold">القوانين</a>
            </div>

            <div class="hidden lg:flex items-center gap-4">
                <button class="whatsapp-btn text-white px-6 py-2.5 rounded-full text-sm font-bold transition-all duration-300 flex items-center gap-2">
                    <i class="fab fa-whatsapp text-lg"></i>
                    انضم الآن
                </button>
            </div>

            <button id="mobile-menu-btn" class="lg:hidden text-royal-gold text-2xl">
                <i class="fas fa-bars"></i>
            </button>
        </div>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="mobile-menu fixed top-0 right-0 w-80 h-full bg-void-card z-50 p-8 shadow-2xl lg:hidden border-l border-royal-gold/20">
            <button id="close-menu" class="absolute top-6 left-6 text-gray-400 hover:text-royal-gold">
                <i class="fas fa-times text-2xl"></i>
            </button>
            <div class="mt-16 flex flex-col gap-6">
                <div class="flex items-center gap-3 mb-6">
                    <i class="fas fa-crown text-royal-gold text-2xl"></i>
                    <span class="text-xl font-bold gradient-text">UBARS</span>
                </div>
                <a href="#home" class="text-lg text-gray-300 hover:text-royal-gold transition-colors py-2 border-b border-white/5">الرئيسية</a>
                <a href="#about" class="text-lg text-gray-300 hover:text-royal-gold transition-colors py-2 border-b border-white/5">عن المملكة</a>
                <a href="#guilds" class="text-lg text-gray-300 hover:text-royal-gold transition-colors py-2 border-b border-white/5">النقابات</a>
                <a href="#ranking" class="text-lg text-gray-300 hover:text-royal-gold transition-colors py-2 border-b border-white/5">التصنيف</a>
                <a href="#events" class="text-lg text-gray-300 hover:text-royal-gold transition-colors py-2 border-b border-white/5">الفعاليات</a>
                <a href="#rules" class="text-lg text-gray-300 hover:text-royal-gold transition-colors py-2 border-b border-white/5">القوانين</a>
                <button class="whatsapp-btn w-full text-white py-3 rounded-xl font-bold mt-4 flex items-center justify-center gap-2">
                    <i class="fab fa-whatsapp"></i>
                    انضم للمملكة
                </button>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="relative min-h-screen hero-gradient overflow-hidden pt-24 flex items-center">
        <!-- Background Effects -->
        <div class="absolute top-20 right-10 w-96 h-96 bg-royal-purple/20 rounded-full blur-3xl animate-pulse-glow"></div>
        <div class="absolute bottom-20 left-10 w-72 h-72 bg-royal-gold/10 rounded-full blur-3xl animate-pulse-glow" style="animation-delay: 2s;"></div>
        
        <div class="container mx-auto px-6 lg:px-12 relative z-10">
            <div class="grid lg:grid-cols-2 gap-12 items-center">
                
                <!-- Text Content -->
                <div class="text-center lg:text-right space-y-8 order-2 lg:order-1">
                    <div class="inline-flex items-center gap-2 bg-royal-gold/10 border border-royal-gold/20 rounded-full px-5 py-2 animate-fade-in-up">
                        <span class="w-2 h-2 bg-green-400 rounded-full animate-pulse"></span>
                        <span class="text-sm text-royal-gold font-bold">+15,000 عضو نشط</span>
                    </div>

                    <h1 class="text-5xl md:text-6xl lg:text-7xl font-black leading-tight animate-fade-in-up font-cairo" style="animation-delay: 0.2s;">
                        <span class="glitch gradient-text" data-text="UBARS">UBARS</span><br>
                        <span class="text-3xl md:text-4xl lg:text-5xl text-gray-300">مملكة <span class="gradient-text-purple">نقابات الأنمي</span></span>
                    </h1>

                    <p class="text-gray-400 text-lg md:text-xl leading-relaxed max-w-xl mx-auto lg:mx-0 animate-fade-in-up" style="animation-delay: 0.3s;">
                        انضم لأكبر مجتمع عربي للأنمي على واتساب. نقابات متخصصة، مسابقات يومية، نقاشات محترمة، وعالم من الإثارة ينتظرك.
                    </p>

                    <div class="flex flex-col sm:flex-row gap-4 justify-center lg:justify-start animate-fade-in-up" style="animation-delay: 0.4s;">
                        <button class="group whatsapp-btn text-white px-8 py-4 rounded-full text-lg font-bold transition-all duration-300 transform hover:scale-105 flex items-center justify-center gap-3">
                            <i class="fab fa-whatsapp text-2xl"></i>
                            انضم للمملكة
                            <i class="fas fa-arrow-left group-hover:-translate-x-1 transition-transform"></i>
                        </button>
                        <button class="group bg-white/5 hover:bg-white/10 border border-royal-gold/30 text-white px-8 py-4 rounded-full text-lg font-medium transition-all flex items-center justify-center gap-2">
                            <i class="fas fa-play-circle text-royal-gold"></i>
                            شاهد الفعاليات
                        </button>
                    </div>

                    <!-- Quick Stats -->
                    <div class="grid grid-cols-3 gap-6 pt-8 border-t border-white/10 animate-fade-in-up" style="animation-delay: 0.5s;">
                        <div class="text-center lg:text-right">
                            <div class="text-3xl font-black gradient-text counter" data-target="15">15K+</div>
                            <div class="text-sm text-gray-400 mt-1">عضو نشط</div>
                        </div>
                        <div class="text-center lg:text-right">
                            <div class="text-3xl font-black text-anime-red counter" data-target="50">50+</div>
                            <div class="text-sm text-gray-400 mt-1">نقابة متخصصة</div>
                        </div>
                        <div class="text-center lg:text-right">
                            <div class="text-3xl font-black text-anime-blue">24/7</div>
                            <div class="text-sm text-gray-400 mt-1">نشاط مستمر</div>
                        </div>
                    </div>
                </div>

                <!-- Visual Content -->
                <div class="relative order-1 lg:order-2 flex justify-center">
                    <div class="relative w-full max-w-lg">
                        <!-- Main Crown/Emblem -->
                        <div class="relative animate-float">
                            <div class="absolute -inset-8 bg-gradient-to-r from-royal-gold/20 to-royal-purple/20 rounded-full blur-3xl"></div>
                            
                            <div class="relative glass-card rounded-3xl p-8 border-2 border-royal-gold/20 shadow-2xl shadow-royal-gold/10">
                                <!-- Kingdom Emblem -->
                                <div class="text-center mb-6">
                                    <div class="w-32 h-32 mx-auto bg-gradient-to-br from-royal-gold via-light-gold to-deep-gold rounded-full flex items-center justify-center shadow-2xl shadow-royal-gold/40 animate-pulse-glow mb-4 relative">
                                        <i class="fas fa-crown text-6xl text-white drop-shadow-lg"></i>
                                        <div class="absolute -top-2 -right-2 w-8 h-8 bg-anime-red rounded-full flex items-center justify-center text-xs font-bold border-2 border-dark-void">VIP</div>
                                    </div>
                                    <h3 class="text-2xl font-bold gradient-text mb-1">تاج المملكة</h3>
                                    <p class="text-gray-400 text-sm">الرمز الملكي لمجتمع UBARS</p>
                                </div>

                                <!-- Guild Preview Cards -->
                                <div class="space-y-3">
                                    <div class="bg-white/5 rounded-xl p-3 flex items-center gap-3 hover:bg-white/10 transition-colors cursor-pointer border border-white/5">
                                        <div class="w-10 h-10 bg-anime-red/20 rounded-lg flex items-center justify-center">
                                            <i class="fas fa-fire text-anime-red"></i>
                                        </div>
                                        <div class="flex-1">
                                            <div class="text-sm font-bold">نقابة الشونين</div>
                                            <div class="text-xs text-gray-400">1,240 عضو</div>
                                        </div>
                                        <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">نشط</span>
                                    </div>
                                    
                                    <div class="bg-white/5 rounded-xl p-3 flex items-center gap-3 hover:bg-white/10 transition-colors cursor-pointer border border-white/5">
                                        <div class="w-10 h-10 bg-anime-blue/20 rounded-lg flex items-center justify-center">
                                            <i class="fas fa-heart text-anime-blue"></i>
                                        </div>
                                        <div class="flex-1">
                                            <div class="text-sm font-bold">نقابة الشوجو</div>
                                            <div class="text-xs text-gray-400">980 عضو</div>
                                        </div>
                                        <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">نشط</span>
                                    </div>

                                    <div class="bg-white/5 rounded-xl p-3 flex items-center gap-3 hover:bg-white/10 transition-colors cursor-pointer border border-white/5">
                                        <div class="w-10 h-10 bg-purple-500/20 rounded-lg flex items-center justify-center">
                                            <i class="fas fa-ghost text-purple-400"></i>
                                        </div>
                                        <div class="flex-1">
                                            <div class="text-sm font-bold">نقابة الأعمال القصيرة</div>
                                            <div class="text-xs text-gray-400">756 عضو</div>
                                        </div>
                                        <span class="text-xs bg-yellow-500/20 text-yellow-400 px-2 py-1 rounded-full">مسابقة</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Floating Badges -->
                            <div class="absolute -top-4 -right-4 bg-anime-red text-white px-4 py-2 rounded-full text-sm font-bold shadow-lg animate-bounce-gentle">
                                <i class="fas fa-bolt mr-1"></i> حدث الآن!
                            </div>
                            
                            <div class="absolute -bottom-4 -left-6 glass-card rounded-xl p-3 shadow-xl border border-royal-gold/20">
                                <div class="flex items-center gap-2">
                                    <div class="flex -space-x-2">
                                        <div class="w-8 h-8 bg-blue-500 rounded-full border-2 border-dark-void flex items-center justify-center text-xs">أ</div>
                                        <div class="w-8 h-8 bg-red-500 rounded-full border-2 border-dark-void flex items-center justify-center text-xs">م</div>
                                        <div class="w-8 h-8 bg-green-500 rounded-full border-2 border-dark-void flex items-center justify-center text-xs">س</div>
                                    </div>
                                    <span class="text-xs text-gray-300">ينضمون الآن...</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Bottom Wave -->
        <div class="absolute bottom-0 left-0 right-0">
            <svg viewBox="0 0 1440 120" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M0 120L60 110C120 100 240 80 360 70C480 60 600 60 720 65C840 70 960 80 1080 85C1200 90 1320 90 1380 90L1440 90V120H1380C1320 120 1200 120 1080 120C960 120 840 120 720 120C600 120 480 120 360 120C240 120 120 120 60 120H0Z" fill="#0A0A0F"/>
            </svg>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-24 relative">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16 scroll-reveal">
                <span class="text-royal-gold font-bold text-sm tracking-wider uppercase">عن المملكة</span>
                <h2 class="text-3xl md:text-5xl font-black mt-4 mb-6 font-cairo">ما هي <span class="gradient-text">UBARS</span>؟</h2>
                <p class="text-gray-400 max-w-3xl mx-auto text-lg leading-relaxed">
                    UBARS هي أكبر مملكة عربية متخصصة في عالم الأنمي والمانجا على منصة واتساب. نجمع عشاق الأنمي من كل مكان في نقابات متخصصة تحت راية واحدة.
                </p>
            </div>

            <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
                <div class="glass-card rounded-2xl p-8 text-center scroll-reveal border border-royal-gold/10 hover:border-royal-gold/30 transition-all">
                    <div class="w-20 h-20 bg-gradient-to-br from-royal-gold to-deep-gold rounded-2xl flex items-center justify-center mx-auto mb-6 shadow-lg shadow-royal-gold/20">
                        <i class="fas fa-shield-alt text-white text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 gradient-text">نظام نقابات</h3>
                    <p class="text-gray-400 leading-relaxed">تنظيم متقن يضمن بيئة نقاشية محترمة ومنظمة لجميع الأعضاء عبر نقابات متخصصة حسب الذوق</p>
                </div>

                <div class="glass-card rounded-2xl p-8 text-center scroll-reveal border border-royal-gold/10 hover:border-royal-gold/30 transition-all" style="transition-delay: 0.1s;">
                    <div class="w-20 h-20 bg-gradient-to-br from-anime-red to-red-800 rounded-2xl flex items-center justify-center mx-auto mb-6 shadow-lg shadow-anime-red/20">
                        <i class="fas fa-trophy text-white text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-anime-red">مسابقات وأحداث</h3>
                    <p class="text-gray-400 leading-relaxed">فعاليات يومية وأسبوعية تشمل مسابقات تrivia، توقعات حلقات، ومسابقات فنية مع جوائز قيمة</p>
                </div>

                <div class="glass-card rounded-2xl p-8 text-center scroll-reveal border border-royal-gold/10 hover:border-royal-gold/30 transition-all" style="transition-delay: 0.2s;">
                    <div class="w-20 h-20 bg-gradient-to-br from-anime-blue to-blue-800 rounded-2xl flex items-center justify-center mx-auto mb-6 shadow-lg shadow-anime-blue/20">
                        <i class="fas fa-users text-white text-3xl"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3 text-anime-blue">مجتمع ودي</h3>
                    <p class="text-gray-400 leading-relaxed">أجواء عائلية تجمع محبي الأنمي بعيداً عن التعصب والتقليل من الأعمال، احترام كامل لجميع الأذواق</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Guilds Section -->
    <section id="guilds" class="py-24 bg-gradient-to-b from-dark-void to-void-card relative overflow-hidden">
        <div class="absolute top-0 right-0 w-96 h-96 bg-royal-purple/10 rounded-full blur-3xl"></div>
        
        <div class="container mx-auto px-6 relative z-10">
            <div class="text-center mb-16 scroll-reveal">
                <span class="text-royal-gold font-bold text-sm tracking-wider uppercase">النقابات</span>
                <h2 class="text-3xl md:text-5xl font-black mt-4 mb-6 font-cairo">نقابات <span class="gradient-text">المملكة</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-lg">اختر نقابتك المفضلة وانضم لعائلتك الأنمية</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6 max-w-6xl mx-auto">
                <!-- Shounen Guild -->
                <div class="guild-card rounded-2xl overflow-hidden border border-white/5 scroll-reveal">
                    <div class="h-48 bg-gradient-to-br from-orange-600 to-red-800 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-fist-raised text-8xl text-white/10 absolute"></i>
                        <div class="relative z-10 text-center">
                            <i class="fas fa-fire text-5xl text-orange-400 mb-2"></i>
                            <h3 class="text-2xl font-bold text-white">نقابة الشونين</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-4">
                            <span class="text-sm text-gray-400"><i class="fas fa-users mr-1"></i> 1,240 عضو</span>
                            <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">مفتوحة</span>
                        </div>
                        <p class="text-gray-400 text-sm mb-4">لعشاق أنمي القوة والمغامرة: ون بيس، ناروتو، هجوم العمالقة، دراغون بول، وجوجو...</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs bg-orange-500/10 text-orange-400 px-2 py-1 rounded">أكشن</span>
                            <span class="text-xs bg-orange-500/10 text-orange-400 px-2 py-1 rounded">مغامرة</span>
                            <span class="text-xs bg-orange-500/10 text-orange-400 px-2 py-1 rounded">قوى خارقة</span>
                        </div>
                        <button class="w-full py-3 rounded-xl bg-gradient-to-r from-orange-600 to-red-700 text-white font-bold hover:from-orange-500 hover:to-red-600 transition-all">
                            انضم للنقابة
                        </button>
                    </div>
                </div>

                <!-- Shoujo Guild -->
                <div class="guild-card rounded-2xl overflow-hidden border border-white/5 scroll-reveal" style="transition-delay: 0.1s;">
                    <div class="h-48 bg-gradient-to-br from-pink-500 to-purple-700 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-heart text-8xl text-white/10 absolute"></i>
                        <div class="relative z-10 text-center">
                            <i class="fas fa-sparkles text-5xl text-pink-300 mb-2"></i>
                            <h3 class="text-2xl font-bold text-white">نقابة الشوجو</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-4">
                            <span class="text-sm text-gray-400"><i class="fas fa-users mr-1"></i> 980 عضو</span>
                            <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">مفتوحة</span>
                        </div>
                        <p class="text-gray-400 text-sm mb-4">لعشاق الرومانسية والدراما: فروتس باسكت، سايلور مون، هوريميا، وكاغويا-ساما...</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs bg-pink-500/10 text-pink-400 px-2 py-1 rounded">رومانسي</span>
                            <span class="text-xs bg-pink-500/10 text-pink-400 px-2 py-1 rounded">دراما</span>
                            <span class="text-xs bg-pink-500/10 text-pink-400 px-2 py-1 rounded">مدرسي</span>
                        </div>
                        <button class="w-full py-3 rounded-xl bg-gradient-to-r from-pink-500 to-purple-600 text-white font-bold hover:from-pink-400 hover:to-purple-500 transition-all">
                            انضم للنقابة
                        </button>
                    </div>
                </div>

                <!-- Seinen Guild -->
                <div class="guild-card rounded-2xl overflow-hidden border border-white/5 scroll-reveal" style="transition-delay: 0.2s;">
                    <div class="h-48 bg-gradient-to-br from-gray-700 to-black flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-skull text-8xl text-white/10 absolute"></i>
                        <div class="relative z-10 text-center">
                            <i class="fas fa-chess-knight text-5xl text-gray-300 mb-2"></i>
                            <h3 class="text-2xl font-bold text-white">نقابة السينين</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-4">
                            <span class="text-sm text-gray-400"><i class="fas fa-users mr-1"></i> 650 عضو</span>
                            <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">مفتوحة</span>
                        </div>
                        <p class="text-gray-400 text-sm mb-4">لعشاق الأعمال الناضجة: بيرسيرك، فاينلاند ساغا، مونستر، وباراسايت...</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs bg-gray-500/10 text-gray-400 px-2 py-1 rounded">نفسي</span>
                            <span class="text-xs bg-gray-500/10 text-gray-400 px-2 py-1 rounded">غموض</span>
                            <span class="text-xs bg-gray-500/10 text-gray-400 px-2 py-1 rounded">تاريخي</span>
                        </div>
                        <button class="w-full py-3 rounded-xl bg-gradient-to-r from-gray-600 to-black text-white font-bold hover:from-gray-500 hover:to-gray-800 transition-all border border-white/10">
                            انضم للنقابة
                        </button>
                    </div>
                </div>

                <!-- Isekai Guild -->
                <div class="guild-card rounded-2xl overflow-hidden border border-white/5 scroll-reveal">
                    <div class="h-48 bg-gradient-to-br from-blue-600 to-indigo-800 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-dragon text-8xl text-white/10 absolute"></i>
                        <div class="relative z-10 text-center">
                            <i class="fas fa-hat-wizard text-5xl text-blue-300 mb-2"></i>
                            <h3 class="text-2xl font-bold text-white">نقابة الإيسيكاي</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-4">
                            <span class="text-sm text-gray-400"><i class="fas fa-users mr-1"></i> 1,100 عضو</span>
                            <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">مفتوحة</span>
                        </div>
                        <p class="text-gray-400 text-sm mb-4">لعشاق عوالم أخرى: ري زيرو، تينسلايم، موشوكو تينسي، وكونوسوبا...</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs bg-blue-500/10 text-blue-400 px-2 py-1 rounded">عالم آخر</span>
                            <span class="text-xs bg-blue-500/10 text-blue-400 px-2 py-1 rounded">سحر</span>
                            <span class="text-xs bg-blue-500/10 text-blue-400 px-2 py-1 rounded">مغامرة</span>
                        </div>
                        <button class="w-full py-3 rounded-xl bg-gradient-to-r from-blue-600 to-indigo-700 text-white font-bold hover:from-blue-500 hover:to-indigo-600 transition-all">
                            انضم للنقابة
                        </button>
                    </div>
                </div>

                <!-- Slice of Life Guild -->
                <div class="guild-card rounded-2xl overflow-hidden border border-white/5 scroll-reveal" style="transition-delay: 0.1s;">
                    <div class="h-48 bg-gradient-to-br from-green-500 to-teal-700 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-coffee text-8xl text-white/10 absolute"></i>
                        <div class="relative z-10 text-center">
                            <i class="fas fa-home text-5xl text-green-300 mb-2"></i>
                            <h3 class="text-2xl font-bold text-white">نقابة الحياة اليومية</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-4">
                            <span class="text-sm text-gray-400"><i class="fas fa-users mr-1"></i> 720 عضو</span>
                            <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">مفتوحة</span>
                        </div>
                        <p class="text-gray-400 text-sm mb-4">لعشاق الأعمال الهادئة: ك-أون، باراكامون، نون نون بيوري، ويايورويشي...</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs bg-green-500/10 text-green-400 px-2 py-1 rounded">كوميدي</span>
                            <span class="text-xs bg-green-500/10 text-green-400 px-2 py-1 rounded">حياة يومية</span>
                            <span class="text-xs bg-green-500/10 text-green-400 px-2 py-1 rounded">شفاء</span>
                        </div>
                        <button class="w-full py-3 rounded-xl bg-gradient-to-r from-green-500 to-teal-600 text-white font-bold hover:from-green-400 hover:to-teal-500 transition-all">
                            انضم للنقابة
                        </button>
                    </div>
                </div>

                <!-- Sports Guild -->
                <div class="guild-card rounded-2xl overflow-hidden border border-white/5 scroll-reveal" style="transition-delay: 0.2s;">
                    <div class="h-48 bg-gradient-to-br from-red-600 to-orange-700 flex items-center justify-center relative overflow-hidden">
                        <i class="fas fa-running text-8xl text-white/10 absolute"></i>
                        <div class="relative z-10 text-center">
                            <i class="fas fa-basketball-ball text-5xl text-orange-300 mb-2"></i>
                            <h3 class="text-2xl font-bold text-white">نقابة الرياضة</h3>
                        </div>
                    </div>
                    <div class="p-6">
                        <div class="flex justify-between items-center mb-4">
                            <span class="text-sm text-gray-400"><i class="fas fa-users mr-1"></i> 540 عضو</span>
                            <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">مفتوحة</span>
                        </div>
                        <p class="text-gray-400 text-sm mb-4">لعشاق الرياضة: هايكيو، كوروكو نو باسكت، بلو لوك، وسلام دانك...</p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span class="text-xs bg-red-500/10 text-red-400 px-2 py-1 rounded">رياضة</span>
                            <span class="text-xs bg-red-500/10 text-red-400 px-2 py-1 rounded">فريق</span>
                            <span class="text-xs bg-red-500/10 text-red-400 px-2 py-1 rounded">تحدي</span>
                        </div>
                        <button class="w-full py-3 rounded-xl bg-gradient-to-r from-red-600 to-orange-700 text-white font-bold hover:from-red-500 hover:to-orange-600 transition-all">
                            انضم للنقابة
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Ranking System -->
    <section id="ranking" class="py-24 relative">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16 scroll-reveal">
                <span class="text-royal-gold font-bold text-sm tracking-wider uppercase">نظام التصنيف</span>
                <h2 class="text-3xl md:text-5xl font-black mt-4 mb-6 font-cairo">المراتب <span class="gradient-text">الملكية</span></h2>
                <p class="text-gray-400 max-w-2xl mx-auto text-lg">تدرج في المراتب من خلال المشاركة والفعاليات</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6 max-w-6xl mx-auto">
                <div class="glass-card rounded-2xl p-6 text-center border-2 border-gray-600/30 scroll-reveal hover:border-gray-500/50 transition-all">
                    <div class="rank-badge w-16 h-20 mx-auto mb-4 flex items-start justify-center pt-3">
                        <i class="fas fa-user text-gray-400 text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-400 mb-2">مواطن</h3>
                    <p class="text-gray-500 text-sm">الرتبة الافتراضية عند الانضمام</p>
                    <div class="mt-4 text-xs text-gray-600">0 نقطة</div>
                </div>

                <div class="glass-card rounded-2xl p-6 text-center border-2 border-anime-blue/30 scroll-reveal hover:border-anime-blue/50 transition-all" style="transition-delay: 0.1s;">
                    <div class="rank-badge w-16 h-20 mx-auto mb-4 flex items-start justify-center pt-3 bg-gradient-to-b from-anime-blue to-blue-800">
                        <i class="fas fa-shield-alt text-white text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-anime-blue mb-2">فارس</h3>
                    <p class="text-gray-400 text-sm">مشاركة نشطة في النقابات</p>
                    <div class="mt-4 text-xs text-anime-blue">500 نقطة</div>
                </div>

                <div class="glass-card rounded-2xl p-6 text-center border-2 border-royal-gold/30 scroll-reveal hover:border-royal-gold/50 transition-all" style="transition-delay: 0.2s;">
                    <div class="rank-badge w-16 h-20 mx-auto mb-4 flex items-start justify-center pt-3 bg-gradient-to-b from-royal-gold to-deep-gold">
                        <i class="fas fa-crown text-white text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold gradient-text mb-2">نبيل</h3>
                    <p class="text-gray-400 text-sm">فائز في مسابقات وفعاليات</p>
                    <div class="mt-4 text-xs text-royal-gold">2,000 نقطة</div>
                </div>

                <div class="glass-card rounded-2xl p-6 text-center border-2 border-purple-500/30 scroll-reveal hover:border-purple-500/50 transition-all" style="transition-delay: 0.3s;">
                    <div class="rank-badge w-16 h-20 mx-auto mb-4 flex items-start justify-center pt-3 bg-gradient-to-b from-purple-500 to-royal-purple">
                        <i class="fas fa-gem text-white text-xl"></i>
                    </div>
                    <h3 class="text-xl font-bold text-purple-400 mb-2">ملك</h3>
                    <p class="text-gray-400 text-sm">قائد نقابة أو مسؤول مملكة</p>
                    <div class="mt-4 text-xs text-purple-400">5,000+ نقطة</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Events Section -->
    <section id="events" class="py-24 bg-gradient-to-b from-void-card to-dark-void relative">
        <div class="container mx-auto px-6">
            <div class="text-center mb-16 scroll-reveal">
                <span class="text-royal-gold font-bold text-sm tracking-wider uppercase">الفعاليات</span>
                <h2 class="text-3xl md:text-5xl font-black mt-4 mb-6 font-cairo">أحداث <span class="gradient-text">المملكة</span></h2>
            </div>

            <div class="grid md:grid-cols-2 gap-8 max-w-5xl mx-auto">
                <div class="glass-card rounded-2xl p-8 border border-royal-gold/20 scroll-reveal hover:border-royal-gold/40 transition-all">
                    <div class="flex items-start gap-4">
                        <div class="w-16 h-16 bg-gradient-to-br from-anime-red to-red-800 rounded-xl flex items-center justify-center flex-shrink-0">
                            <i class="fas fa-trophy text-white text-2xl"></i>
                        </div>
                        <div>
                            <div class="flex items-center gap-2 mb-2">
                                <h3 class="text-xl font-bold">بطولة المملكة السنوية</h3>
                                <span class="text-xs bg-anime-red/20 text-anime-red px-2 py-1 rounded-full">قادم</span>
                            </div>
                            <p class="text-gray-400 text-sm mb-4">مسابقة ضخمة تشمل جميع النقابات مع أسئلة عن الأنمي، توقعات، وتحديات فنية. الجائزة الكبرى: لقب "بطل المملكة"</p>
                            <div class="flex items-center gap-4 text-sm text-gray-500">
                                <span><i class="far fa-calendar mr-1"></i> 15 يونيو 2026</span>
                                <span><i class="fas fa-users mr-1"></i> 500+ مشارك</span>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="glass-card rounded-2xl p-8 border border-royal-gold/20 scroll-reveal hover:border-royal-gold/40 transition-all" style="transition-delay: 0.1s;">
                    <div class="flex items-start gap-4">
                        <div class="w-16 h-16 bg-gradient-to-br from-anime-blue to-blue-800 rounded-xl flex items-center justify-center flex-shrink-0">
                            <i class="fas fa-paint-brush text-white text-2xl"></i>
                        </div>
                        <div>
                            <div class="flex items-center gap-2 mb-2">
                                <h3 class="text-xl font-bold">أسبوع الفن الأنمي</h3>
                                <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">نشط</span>
                            </div>
                            <p class="text-gray-400 text-sm mb-4">عرض أعمال فنية من أعضاء المملكة: رسم، تصميم، كتابة، وتلوين. تصويت جماعي لاختيار الأفضل.</p>
                            <div class="flex items-center gap-4 text-sm text-gray-500">
                                <span><i class="far fa-calendar mr-1"></i> كل جمعة</span>
                                <span><i class="fas fa-image mr-1"></i> 200+ عمل</span>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="glass-card rounded-2xl p-8 border border-royal-gold/20 scroll-reveal hover:border-royal-gold/40 transition-all">
                    <div class="flex items-start gap-4">
                        <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-royal-purple rounded-xl flex items-center justify-center flex-shrink-0">
                            <i class="fas fa-question-circle text-white text-2xl"></i>
                        </div>
                        <div>
                            <div class="flex items-center gap-2 mb-2">
                                <h3 class="text-xl font-bold">تحدي التrivia الليلي</h3>
                                <span class="text-xs bg-green-500/20 text-green-400 px-2 py-1 rounded-full">يومي</span>
                            </div>
                            <p class="text-gray-400 text-sm mb-4">أسئلة يومية سريعة عن الأنمي في جميع النقابات. اجمع النقاط وارتقِ في المراتب الملكية.</p>
                            <div class="flex items-center gap-4 text-sm text-gray-500">
                                <span><i class="far fa-clock mr-1"></i> 9:00 مساءً</span>
                                <span><i class="fas fa-bolt mr-1"></i> 50 نقطة/إجابة</span>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="glass-card rounded-2xl p-8 border border-royal-gold/20 scroll-reveal hover:border-royal-gold/40 transition-all" style="transition-delay: 0.1s;">
                    <div class="flex items-start gap-4">
                        <div class="w-16 h-16 bg-gradient-to-br from-royal-gold to-deep-gold rounded-xl flex items-center justify-center flex-shrink-0">
                            <i class="fas fa-gift text-white text-2xl"></i>
                        </div>
                        <div>
                            <div class="flex items-center gap-2 mb-2">
                                <h3 class="text-xl font-bold">مواسم الأنمي الجديدة</h3>
                                <span class="text-xs bg-anime-blue/20 text-anime-blue px-2 py-1 rounded-full">موسمي</span>
                            </div>
                            <p class="text-gray-400 text-sm mb-4">متابعة جماعية لأنميات الموسم الجديد مع نقاشات حلقة بحلقة وتوقعات وتقييمات جماعية.</p>
                            <div class="flex items-center gap-4 text-sm text-gray-500">
                                <span><i class="fas fa-tv mr-1"></i> كل موسم</span>
                                <span><i class="fas fa-comments mr-1"></i> نقاش حي</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Rules Section -->
    <section id="rules" class="py-24 relative">
        <div class="container mx-auto px-6 max-w-4xl">
            <div class="text-center mb-16 scroll-reveal">
                <span class="text-royal-gold font-bold text-sm tracking-wider uppercase">القوانين</span>
                <h2 class="text-3xl md:text-5xl font-black mt-4 mb-6 font-cairo">دستور <span class="gradient-text">المملكة</span></h2>
                <p class="text-gray-400 text-lg">قوانين بسيطة لضمان بيئة صحية للجميع</p>
            </div>

            <div class="space-y-4">
                <div class="glass-card rounded-xl p-6 flex items-start gap-4 border border-white/5 scroll-reveal hover:border-royal-gold/20 transition-all">
                    <div class="w-12 h-12 bg-anime-red/20 rounded-xl flex items-center justify-center flex-shrink-0">
                        <span class="text-anime-red font-bold text-xl">1</span>
                    </div>
                    <div>
                        <h3 class="font-bold text-lg mb-2">احترام الأذواق</h3>
                        <p class="text-gray-400">ممنوع التقليل من أي عمل أنمي أو إهانة ذوق أي عضو. كل عمل له جمهوره واحترام الآخر واجب.</p>
                    </div>
                </div>

                <div class="glass-card rounded-xl p-6 flex items-start gap-4 border border-white/5 scroll-reveal hover:border-royal-gold/20 transition-all" style="transition-delay: 0.1s;">
                    <div class="w-12 h-12 bg-anime-blue/20 rounded-xl flex items-center justify-center flex-shrink-0">
                        <span class="text-anime-blue font-bold text-xl">2</span>
                    </div>
                    <div>
                        <h3 class="font-bold text-lg mb-2">لا حرق</h3>
                        <p class="text-gray-400">ممنوع حرق الأنميات في القنوات العامة. استخدم قنوات الحرق المخصصة مع تحذير واضح.</p>
                    </div>
                </div>

                <div class="glass-card rounded-xl p-6 flex items-start gap-4 border border-white/5 scroll-reveal hover:border-royal-gold/20 transition-all" style="transition-delay: 0.2s;">
                    <div class="w-12 h-12 bg-green-500/20 rounded-xl flex items-center justify-center flex-shrink-0">
                        <span class="text-green-400 font-bold text-xl">3</span>
                    </div>
                    <div>
                        <h3 class="font-bold text-lg mb-2">لغة محترمة</h3>
                        <p class="text-gray-400">ممنوع السب والشتم والتنمر. البيئة يجب أن تكون عائلية ومحترمة تجاه الجميع.</p>
                    </div>
                </div>

                <div class="glass-card rounded-xl p-6 flex items-start gap-4 border border-white/5 scroll-reveal hover:border-royal-gold/20 transition-all" style="transition-delay: 0.3s;">
                    <div class="w-12 h-12 bg-purple-500/20 rounded-xl flex items-center justify-center flex-shrink-0">
                        <span class="text-purple-400 font-bold text-xl">4</span>
                    </div>
                    <div>
                        <h3 class="font-bold text-lg mb-2">نشاط إيجابي</h3>
                        <p class="text-gray-400">المشاركة في الفعاليات والمسابقات مشجعة. الغياب الطويل قد يؤدي لإزالة العضوية.</p>
                    </div>
                </div>

                <div class="glass-card rounded-xl p-6 flex items-start gap-4 border border-white/5 scroll-reveal hover:border-royal-gold/20 transition-all" style="transition-delay: 0.4s;">
                    <div class="w-12 h-12 bg-royal-gold/20 rounded-xl flex items-center justify-center flex-shrink-0">
                        <span class="text-royal-gold font-bold text-xl">5</span>
                    </div>
                    <div>
                        <h3 class="font-bold text-lg mb-2">الولاء للمملكة</h3>
                        <p class="text-gray-400">الانضمام لنقابة واحدة على الأقل إلزامي. يمكنك المشاركة في فعاليات جميع النقابات.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Join CTA -->
    <section class="py-24 relative overflow-hidden">
        <div class="absolute inset-0 bg-gradient-to-r from-royal-purple/20 to-royal-gold/20"></div>
        <div class="absolute inset-0 bg-[url('data:image/svg+xml,%3Csvg width=\'60\' height=\'60\' viewBox=\'0 0 60 60\' xmlns=\'http://www.w3.org/2000/svg\'%3E%3Cg fill=\'none\' fill-rule=\'evenodd\'%3E%3Cg fill=\'%23D4AF37\' fill-opacity=\'0.03\'%3E%3Cpath d=\'M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z\'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E')]"></div>
        
        <div class="container mx-auto px-6 relative z-10 text-center scroll-reveal">
            <div class="w-24 h-24 bg-gradient-to-br from-royal-gold to-deep-gold rounded-full flex items-center justify-center mx-auto mb-8 shadow-2xl shadow-royal-gold/40 animate-pulse-glow">
                <i class="fas fa-crown text-5xl text-white"></i>
            </div>
            <h2 class="text-4xl md:text-6xl font-black mb-6 font-cairo">انضم لـ <span class="gradient-text">UBARS</span> الآن</h2>
            <p class="text-gray-300 text-lg max-w-2xl mx-auto mb-10">مملكة نقابات الأنمي تنتظرك. عالم من الإثارة، المنافسة الشريفة، والصداقات الأنمية بانتظارك.</p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <button class="whatsapp-btn text-white px-12 py-5 rounded-full text-xl font-bold transition-all transform hover:scale-105 flex items-center justify-center gap-3">
                    <i class="fab fa-whatsapp text-2xl"></i>
                    انضم عبر واتساب
                </button>
            </div>
            <p class="text-gray-500 text-sm mt-6">مجتمع عربي | +15,000 عضو | نقابات متخصصة</p>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark-void border-t border-royal-gold/10 pt-16 pb-8">
        <div class="container mx-auto px-6">
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-12 mb-12">
                <div>
                    <div class="flex items-center gap-3 mb-6">
                        <div class="w-10 h-10 bg-gradient-to-br from-royal-gold to-deep-gold rounded-xl flex items-center justify-center crown-icon">
                            <i class="fas fa-crown text-white text-lg"></i>
                        </div>
                        <span class="text-2xl font-black gradient-text font-cairo">UBARS</span>
                    </div>
                    <p class="text-gray-400 leading-relaxed mb-6">مملكة نقابات الأنمي العربية على واتساب. نجمع عشاق الأنمي في بيئة محترمة ومنظمة.</p>
                    <div class="flex gap-4">
                        <a href="#" class="w-10 h-10 bg-white/5 rounded-lg flex items-center justify-center text-gray-400 hover:bg-royal-gold hover:text-white transition-all">
                            <i class="fab fa-whatsapp"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-white/5 rounded-lg flex items-center justify-center text-gray-400 hover:bg-anime-blue hover:text-white transition-all">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-white/5 rounded-lg flex items-center justify-center text-gray-400 hover:bg-anime-red hover:text-white transition-all">
                            <i class="fab fa-instagram"></i>
                        </a>
                    </div>
                </div>

                <div>
                    <h4 class="font-bold text-lg mb-6 text-royal-gold">النقابات</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">نقابة الشونين</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">نقابة الشوجو</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">نقابة السينين</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">نقابة الإيسيكاي</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">نقابة الحياة اليومية</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="font-bold text-lg mb-6 text-royal-gold">روابط سريعة</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">عن المملكة</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">نظام التصنيف</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">الفعاليات</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">القوانين</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-royal-gold transition-colors">الدعم</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="font-bold text-lg mb-6 text-royal-gold">تواصل معنا</h4>
                    <p class="text-gray-400 mb-4">هل لديك استفسار أو اقتراح؟ تواصل مع المسؤولين</p>
                    <button class="w-full py-3 rounded-xl border border-royal-gold/30 text-royal-gold font-bold hover:bg-royal-gold/10 transition-all flex items-center justify-center gap-2">
                        <i class="fab fa-whatsapp"></i>
                        تواصل عبر واتساب
                    </button>
                </div>
            </div>

            <div class="border-t border-white/5 pt-8 flex flex-col md:flex-row justify-between items-center gap-4">
                <p class="text-gray-600 text-sm">© 2026 UBARS Kingdom. جميع الحقوق محفوظة.</p>
                <div class="flex gap-6 text-sm text-gray-600">
                    <span class="flex items-center gap-1"><i class="fas fa-heart text-anime-red"></i> صنع بعشق للأنمي</span>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Generate floating particles
        const particlesContainer = document.getElementById('particles');
        for (let i = 0; i < 30; i++) {
            const particle = document.createElement('div');
            particle.className = 'particle';
            particle.style.left = Math.random() * 100 + '%';
            particle.style.animationDelay = Math.random() * 10 + 's';
            particle.style.animationDuration = (10 + Math.random() * 10) + 's';
            particlesContainer.appendChild(particle);
        }

        // Mobile Menu
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const closeMenuBtn = document.getElementById('close-menu');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => mobileMenu.classList.add('active'));
        closeMenuBtn.addEventListener('click', () => mobileMenu.classList.remove('active'));
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => mobileMenu.classList.remove('active'));
        });

        // Scroll Reveal
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('revealed');
                    
                    // Animate counters
                    const counters = entry.target.querySelectorAll('.counter');
                    counters.forEach(counter => {
                        const target = parseFloat(counter.dataset.target);
                        if (target > 100) {
                            let current = 0;
                            const step = target / 50;
                            const update = () => {
                                current += step;
                                if (current < target) {
                                    counter.textContent = Math.floor(current) + 'K+';
                                    requestAnimationFrame(update);
                                } else {
                                    counter.textContent = target + 'K+';
                                }
                            };
                            update();
                        }
                    });
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.scroll-reveal').forEach(el => observer.observe(el));

        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) target.scrollIntoView({ behavior: 'smooth', block: 'start' });
            });
        });

        // Typing effect for hero subtitle
        const typingText = "مملكة نقابات الأنمي";
        const typingElement = document.querySelector('.typing-cursor');
        if (typingElement) {
            let i = 0;
            const type = () => {
                if (i < typingText.length) {
                    typingElement.textContent += typingText.charAt(i);
                    i++;
                    setTimeout(type, 100);
                }
            };
            setTimeout(type, 1000);
        }
    </script>
</body>
</html>
