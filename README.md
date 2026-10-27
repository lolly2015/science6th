[index (1).html](https://github.com/user-attachments/files/34026660/index.1.html)
# science6th<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- Google Search Engine Meta Tags -->
    <title>منصة التفهيم الذكية - المرجع الشامل والكامل للصف السادس الابتدائي (موقع كتبي)</title>
    <meta name="description" content="منصة تفاعلية وشاملة تحتوي على كل دروس وموضوعات كتب الصف السادس الابتدائي لجميع الفصول الدراسية والمواد بالكامل بدون اختصار.">
    <meta name="keywords" content="علوم السادس, لغتي السادس, المهارات الرقمية سادس, رياضيات سادس, منصة التفهيم الذكية, موقع كتبي, منهج سادس ابتدائي">
    <meta name="robots" content="index, follow">

    <!-- Open Graph for Social Media & Site Recognition -->
    <meta property="og:site_name" content="منصة التفهيم الذكية">
    <meta property="og:title" content="منصة التفهيم الذكية - المرجع التفاعلي الشامل لجميع مواد الصف السادس">
    <meta property="og:description" content="تعلم كافة مواد الصف السادس بالتفصيل الكامل من كتب وزارة التعليم وموقع كتبي! دروس مفصلة واختبارات تفاعلية.">
    <meta property="og:type" content="website">

    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts (Cairo & Tajawal) -->
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@500;700;800;900;1000&family=Tajawal:wght@500;700;900&display=swap" rel="stylesheet">
    <!-- Canvas Confetti for Celebrations -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>
    
    <style>
        * {
            font-family: 'Cairo', 'Tajawal', sans-serif;
        }
        body {
            background: linear-gradient(135deg, #0f172a 0%, #1e1b4b 40%, #2e1065 70%, #0284c7 100%);
            background-attachment: fixed;
        }
        .custom-scrollbar::-webkit-scrollbar {
            width: 8px;
        }
        .custom-scrollbar::-webkit-scrollbar-track {
            background: rgba(15, 23, 42, 0.6);
            border-radius: 8px;
        }
        .custom-scrollbar::-webkit-scrollbar-thumb {
            background: linear-gradient(to bottom, #818cf8, #c084fc);
            border-radius: 8px;
        }
        .glow-effect {
            box-shadow: 0 0 25px rgba(168, 85, 247, 0.4);
        }
        .glow-effect:hover {
            box-shadow: 0 0 40px rgba(236, 72, 153, 0.6);
        }
        .card-bounce {
            transition: all 0.3s cubic-bezier(0.34, 1.56, 0.64, 1);
        }
        .card-bounce:hover {
            transform: translateY(-8px) scale(1.02);
        }
        .vibrant-card-1 { background: linear-gradient(135deg, #4f46e5 0%, #7c3aed 100%); }
        .vibrant-card-2 { background: linear-gradient(135deg, #d97706 0%, #ea580c 100%); }
        .vibrant-card-3 { background: linear-gradient(135deg, #0284c7 0%, #2563eb 100%); }
        .vibrant-card-4 { background: linear-gradient(135deg, #059669 0%, #10b981 100%); }
        .vibrant-card-5 { background: linear-gradient(135deg, #0d9488 0%, #06b6d4 100%); }
        .vibrant-card-6 { background: linear-gradient(135deg, #e11d48 0%, #f43f5e 100%); }
        .vibrant-card-7 { background: linear-gradient(135deg, #9333ea 0%, #c084fc 100%); }
        .vibrant-card-8 { background: linear-gradient(135deg, #db2777 0%, #f472b6 100%); }
        .vibrant-card-9 { background: linear-gradient(135deg, #ca8a04 0%, #facc15 100%); }

        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(236, 72, 153, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 15px rgba(236, 72, 153, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(236, 72, 153, 0); }
        }
        .pulse-btn {
            animation: pulse-ring 2.5s infinite;
        }
    </style>
</head>
<body class="text-slate-100 min-h-screen flex flex-col justify-between custom-scrollbar selection:bg-pink-500 selection:text-white">

    <!-- Gamification Top Stats Bar -->
    <div class="bg-slate-900/90 border-b border-indigo-500/30 px-4 py-2 backdrop-blur-md sticky top-0 z-50 text-xs md:text-sm">
        <div class="max-w-7xl mx-auto flex justify-between items-center flex-wrap gap-2">
            <!-- Level & XP -->
            <div class="flex items-center gap-4">
                <div class="flex items-center gap-1.5 bg-gradient-to-r from-amber-500 to-yellow-400 text-slate-950 font-black px-3 py-1 rounded-full shadow-lg">
                    <i class="fa-solid fa-crown text-amber-900"></i>
                    <span>المستوى: <span id="user-level-txt">1 (بطل)</span></span>
                </div>
                <div class="flex items-center gap-1.5 bg-indigo-950 border border-indigo-500/50 px-3 py-1 rounded-full text-indigo-300 font-bold">
                    <i class="fa-solid fa-star text-yellow-400"></i>
                    <span>نقاط الخبرة: <span id="user-xp-txt" class="text-white font-black">0</span> XP</span>
                </div>
            </div>

            <!-- Streak & Motivation Badges -->
            <div class="flex items-center gap-3">
                <div class="flex items-center gap-1.5 bg-rose-500/20 text-rose-300 border border-rose-500/40 px-3 py-1 rounded-full font-extrabold animate-pulse">
                    <i class="fa-solid fa-fire text-rose-500"></i>
                    <span>حماس اليوم: 1 🔥</span>
                </div>
                <div class="hidden sm:flex items-center gap-1 bg-purple-900/50 border border-purple-500/30 px-3 py-1 rounded-full text-purple-200">
                    <i class="fa-solid fa-medal text-amber-300"></i>
                    <span>الأوسمة: <span id="badges-count">0</span> / 6</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Header Navigation -->
    <header class="bg-slate-900/70 backdrop-blur-lg border-b border-indigo-500/20 px-4 py-3 shadow-xl">
        <div class="max-w-7xl mx-auto flex flex-wrap justify-between items-center gap-4">
            <div class="flex items-center gap-3 cursor-pointer group" onclick="switchTab('home')">
                <div class="bg-gradient-to-tr from-pink-500 via-purple-600 to-indigo-500 p-3 rounded-2xl shadow-lg shadow-pink-500/30 group-hover:rotate-12 transition-transform">
                    <i class="fa-solid fa-rocket text-2xl text-white"></i>
                </div>
                <div>
                    <h1 class="text-xl md:text-3xl font-black bg-gradient-to-r from-pink-400 via-purple-300 to-cyan-300 bg-clip-text text-transparent flex items-center gap-2">
                        منصة التفهيم الذكية ⚡
                    </h1>
                    <p class="text-xs text-cyan-300 font-semibold">رحلتك الممتعة لتفوق المنهج الكامل (موقع كتبي)</p>
                </div>
            </div>

            <!-- Main Navigation Buttons -->
            <nav class="flex items-center gap-2 overflow-x-auto pb-1 md:pb-0 w-full md:w-auto">
                <button onclick="switchTab('home')" id="nav-home" class="nav-btn px-4 py-2.5 rounded-xl text-xs md:text-sm font-extrabold bg-gradient-to-r from-indigo-600 to-purple-600 text-white shadow-lg shadow-indigo-600/30 transition-all flex items-center gap-2 whitespace-nowrap">
                    <i class="fa-solid fa-house"></i> الرئيسية
                </button>
                <button onclick="switchTab('curriculum')" id="nav-curriculum" class="nav-btn px-4 py-2.5 rounded-xl text-xs md:text-sm font-extrabold bg-slate-800/80 text-slate-300 hover:bg-slate-700 transition-all flex items-center gap-2 whitespace-nowrap">
                    <i class="fa-solid fa-book-sparkles text-yellow-400"></i> الكتب والدروس 📚
                </button>
                <button onclick="switchTab('interactive')" id="nav-interactive" class="nav-btn px-4 py-2.5 rounded-xl text-xs md:text-sm font-extrabold bg-slate-800/80 text-slate-300 hover:bg-slate-700 transition-all flex items-center gap-2 whitespace-nowrap pulse-btn">
                    <i class="fa-solid fa-vial-circle-check text-emerald-400"></i> المعمل التفاعلي 🧪
                </button>
                <button onclick="switchTab('dictionary')" id="nav-dictionary" class="nav-btn px-4 py-2.5 rounded-xl text-xs md:text-sm font-extrabold bg-slate-800/80 text-slate-300 hover:bg-slate-700 transition-all flex items-center gap-2 whitespace-nowrap">
                    <i class="fa-solid fa-wand-magic-sparkles text-cyan-400"></i> معجم التفهيم 📖
                </button>
                <button onclick="switchTab('quiz')" id="nav-quiz" class="nav-btn px-4 py-2.5 rounded-xl text-xs md:text-sm font-extrabold bg-slate-800/80 text-slate-300 hover:bg-slate-700 transition-all flex items-center gap-2 whitespace-nowrap">
                    <i class="fa-solid fa-gamepad text-pink-400"></i> تحدي الأبطال 🎯
                </button>
            </nav>
        </div>
    </header>

    <!-- Main Content Dynamic Container -->
    <main class="max-w-7xl mx-auto px-4 py-6 flex-grow w-full">

        <!-- SECTION: HOME / WELCOME WITH ALL SUBJECT SELECTION -->
        <section id="tab-home" class="space-y-8">
            <!-- Banner with Vivid Gradient and Motivation -->
            <div class="relative overflow-hidden rounded-3xl bg-gradient-to-r from-indigo-900 via-purple-900 to-pink-900 p-8 md:p-10 border-2 border-pink-500/40 shadow-2xl glow-effect">
                <div class="relative z-10 max-w-4xl space-y-4">
                    <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full text-xs font-black bg-gradient-to-r from-amber-400 to-pink-500 text-slate-950 shadow-md">
                        <i class="fa-solid fa-bolt"></i> خوض تجربة التعلم باللعب والإبداع!
                    </div>
                    <h2 class="text-3xl md:text-5xl font-black text-white leading-tight">
                        جميع مناهج الصف السادس الابتدائي بطريقة ممتعة وتفاعلية! 🌟🚀
                    </h2>
                    <p class="text-purple-100 text-sm md:text-base leading-relaxed">
                        اختر أي مادة دراسية واستكشف الدروس المفصلة، التجارب العلمية التفاعلية، وحل الألغاز للحصول على النقاط والأوسمة الذهبية!
                    </p>
                    <div class="pt-2 flex flex-wrap gap-3">
                        <button onclick="switchTab('quiz')" class="px-6 py-3 rounded-2xl bg-gradient-to-r from-amber-400 to-amber-500 text-slate-950 font-black text-sm shadow-xl hover:scale-105 active:scale-95 transition flex items-center gap-2">
                            <i class="fa-solid fa-trophy"></i> ابدأ التحدي واجمع النقاط الآن!
                        </button>
                        <button onclick="switchTab('interactive')" class="px-6 py-3 rounded-2xl bg-white/10 hover:bg-white/20 border border-white/30 text-white font-bold text-sm transition flex items-center gap-2">
                            <i class="fa-solid fa-microscope text-cyan-300"></i> جرب المعمل التفاعلي
                        </button>
                    </div>
                </div>
            </div>

            <!-- All Subject Selection Cards Grid (Vibrant Cards) -->
            <div class="space-y-6">
                <div class="text-center space-y-1">
                    <h3 class="text-2xl md:text-3xl font-black text-white flex items-center justify-center gap-2">
                        <i class="fa-solid fa-sparkles text-amber-400"></i> المناهج الكاملة للمواد الدراسية
                    </h3>
                    <p class="text-xs text-indigo-200">اضغط على أي مادة للانتقال إلى دروسها الكاملة فوراً</p>
                </div>

                <div class="grid grid-cols-2 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-5 max-w-6xl mx-auto">
                    <!-- Subject 1: Science -->
                    <div onclick="selectSubject('science')" class="vibrant-card-1 p-6 rounded-3xl border-2 border-indigo-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🔬</div>
                        <h3 class="text-xl font-black">العلوم بالكامل</h3>
                        <p class="text-xs text-indigo-100">الخلايا، الوراثة، عمليات الحياة، الأنظمة البيئية، الأرض والموارد، المادة والطاقة.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 2: Arabic -->
                    <div onclick="selectSubject('arabic')" class="vibrant-card-2 p-6 rounded-3xl border-2 border-amber-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">📖</div>
                        <h3 class="text-xl font-black">لغتي الجميلة</h3>
                        <p class="text-xs text-amber-100">الوظائف النحوية، الإملائية، المشتقات، الأفعال الخمسة والنصوص القرائية.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 3: Digital Skills -->
                    <div onclick="selectSubject('digital')" class="vibrant-card-3 p-6 rounded-3xl border-2 border-blue-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">💻</div>
                        <h3 class="text-xl font-black">المهارات الرقمية</h3>
                        <p class="text-xs text-blue-100">برمجة Scratch، الجداول الإلكترونية Excel، الأمن الرقمي والمستندات.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 4: Mathematics -->
                    <div onclick="selectSubject('math')" class="vibrant-card-4 p-6 rounded-3xl border-2 border-emerald-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🔢</div>
                        <h3 class="text-xl font-black">الرياضيات الشاملة</h3>
                        <p class="text-xs text-emerald-100">12 فصلاً: الأسس، الكسور، النسبة، الجبر، الهندسة والقياس والإحصاء.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 5: Islamic Studies -->
                    <div onclick="selectSubject('islamic')" class="vibrant-card-5 p-6 rounded-3xl border-2 border-teal-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🕋</div>
                        <h3 class="text-xl font-black">الدراسات الإسلامية</h3>
                        <p class="text-xs text-teal-100">التوحيد، الفقه والسلوك، الحديث والسيرة النبوية، التفسير والتجويد.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 6: Social Studies -->
                    <div onclick="selectSubject('social')" class="vibrant-card-6 p-6 rounded-3xl border-2 border-rose-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🌍</div>
                        <h3 class="text-xl font-black">الدراسات الاجتماعية</h3>
                        <p class="text-xs text-rose-100">تاريخ الدولة السعودية الأولى والثانية، جغرافية الوطن، ورؤية 2030.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 7: English -->
                    <div onclick="selectSubject('english')" class="vibrant-card-7 p-6 rounded-3xl border-2 border-purple-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🇬🇧</div>
                        <h3 class="text-xl font-black">اللغة الإنجليزية</h3>
                        <p class="text-xs text-purple-100">We Can: Chores, Careers, Food, Weather, Grammar & Phonics.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 8: Art -->
                    <div onclick="selectSubject('art')" class="vibrant-card-8 p-6 rounded-3xl border-2 border-pink-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-white">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-white/20 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🎨</div>
                        <h3 class="text-xl font-black">التربية الفنية</h3>
                        <p class="text-xs text-pink-100">الزخرفة الإسلامية، دائرة الألوان، النسيج والطباعة والتشكيل.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-white/20 hover:bg-white/30 font-black text-xs border border-white/30">ابدأ الآن ⬅️</span>
                    </div>

                    <!-- Subject 9: Life Skills -->
                    <div onclick="selectSubject('lifeskills')" class="vibrant-card-9 p-6 rounded-3xl border-2 border-yellow-300/40 shadow-xl card-bounce cursor-pointer text-center space-y-3 group text-slate-950">
                        <div class="w-16 h-16 mx-auto rounded-2xl bg-black/10 flex items-center justify-center text-4xl shadow-inner group-hover:rotate-12 transition-transform">🏠</div>
                        <h3 class="text-xl font-black">المهارات الحياتية</h3>
                        <p class="text-xs font-bold text-slate-800">صحتي وسلامتي، إدارة الوقت والمصروف، والغذاء والعناية بالملبس.</p>
                        <span class="inline-block px-4 py-1.5 rounded-xl bg-black/10 hover:bg-black/20 font-black text-xs border border-black/20">ابدأ الآن ⬅️</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- SECTION: CURRICULUM LESSONS (All Subjects - FULL CONTENT) -->
        <section id="tab-curriculum" class="hidden space-y-6">

            <!-- Subject Selection Navigation Pills -->
            <div class="flex gap-2 overflow-x-auto pb-2 border-b border-indigo-500/20 scrollbar-none">
                <button onclick="selectSubject('science')" id="sub-btn-science" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-gradient-to-r from-indigo-600 to-purple-600 text-white whitespace-nowrap shadow-md">🔬 العلوم</button>
                <button onclick="selectSubject('arabic')" id="sub-btn-arabic" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">📖 لغتي الجميلة</button>
                <button onclick="selectSubject('digital')" id="sub-btn-digital" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">💻 المهارات الرقمية</button>
                <button onclick="selectSubject('math')" id="sub-btn-math" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">🔢 الرياضيات</button>
                <button onclick="selectSubject('islamic')" id="sub-btn-islamic" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">🕋 الدراسات الإسلامية</button>
                <button onclick="selectSubject('social')" id="sub-btn-social" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">🌍 الدراسات الاجتماعية</button>
                <button onclick="selectSubject('english')" id="sub-btn-english" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">🇬🇧 English</button>
                <button onclick="selectSubject('art')" id="sub-btn-art" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">🎨 التربية الفنية</button>
                <button onclick="selectSubject('lifeskills')" id="sub-btn-lifeskills" class="sub-nav-btn px-4 py-2.5 rounded-xl font-black text-xs transition-all bg-slate-800/80 text-slate-300 whitespace-nowrap">🏠 المهارات الحياتية</button>
            </div>

            <!-- SCIENCE SECTION FULL -->
            <div id="curriculum-science" class="subject-curriculum space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-indigo-500/40 shadow-2xl space-y-4">
                    <div class="flex items-center justify-between border-b border-indigo-500/30 pb-3 flex-wrap gap-2">
                        <div class="flex items-center gap-3">
                            <span class="bg-indigo-500/20 text-indigo-300 text-xs font-black px-3 py-1 rounded-full border border-indigo-500/40">كتاب العلوم الشامل</span>
                            <h3 class="text-2xl font-black text-amber-300">محتويات كتاب العلوم بالكامل (6 وحدات)</h3>
                        </div>
                        <button onclick="addXP(10, 'استكشاف منهج العلوم!')" class="px-3 py-1 bg-amber-400 hover:bg-amber-300 text-slate-950 font-black rounded-xl text-xs shadow">
                            +10 XP أخذت نظرة سريعة! ⚡
                        </button>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 text-xs text-slate-200">
                        <div class="bg-indigo-950/70 p-5 rounded-2xl border border-indigo-500/40 space-y-2 card-bounce">
                            <span class="text-amber-400 font-extrabold block text-sm">الوحدة الأولى: تنوع الحياة</span>
                            <h4 class="font-black text-cyan-300 text-sm">الفصل الأول: الخلايا والوراثة</h4>
                            <ul class="list-disc list-inside space-y-1 text-slate-300">
                                <li><strong>الدرس الأول: الخلايا:</strong> النظرية الخلوية، مستويات التنظيم (خلية ⬅️ نسيج ⬅️ عضو ⬅️ جهاز)، الخلية النباتية والحيوانية.</li>
                                <li><strong>الدرس الثاني: الوراثة والصفات:</strong> الصفات السائدة والمتنحية ومربع بانيت لتوقع الصفات الوراثية.</li>
                            </ul>
                        </div>

                        <div class="bg-purple-950/70 p-5 rounded-2xl border border-purple-500/40 space-y-2 card-bounce">
                            <span class="text-amber-400 font-extrabold block text-sm">الوحدة الثانية: عمليات الحياة</span>
                            <h4 class="font-black text-pink-300 text-sm">الفصل الثاني: النباتات والحيوانات</h4>
                            <ul class="list-disc list-inside space-y-1 text-slate-300">
                                <li><strong>الدرس الأول: عمليات الحياة في النباتات:</strong> البناء الضوئي، النتح، والأوعية الخشبية واللحاء.</li>
                                <li><strong>الدرس الثاني: عمليات الحياة في الإنسان والحيوان:</strong> الهضم، التنفس، الدوران، والإخراج.</li>
                            </ul>
                        </div>

                        <div class="bg-blue-950/70 p-5 rounded-2xl border border-blue-500/40 space-y-2 card-bounce">
                            <span class="text-amber-400 font-extrabold block text-sm">الوحدة الثالثة: الأنظمة البيئية</span>
                            <h4 class="font-black text-cyan-300 text-sm">الفصل الثالث: الأنظمة والموارد</h4>
                            <ul class="list-disc list-inside space-y-1 text-slate-300">
                                <li><strong>الدرس الأول: السلاسل الغذائية:</strong> المنتجات والمستهلكات والمحللات وهرم الطاقة.</li>
                                <li><strong>الدرس الثاني: التغيرات في الأنظمة:</strong> التعاقب البيئي الأولوي والثانوي وحماية البيئة.</li>
                            </ul>
                        </div>

                        <div class="bg-emerald-950/70 p-5 rounded-2xl border border-emerald-500/40 space-y-2 card-bounce">
                            <span class="text-amber-400 font-extrabold block text-sm">الوحدة الرابعة: طقس الأرض</span>
                            <h4 class="font-black text-emerald-300 text-sm">الفصل الرابع: الأرض والمناخ</h4>
                            <ul class="list-disc list-inside space-y-1 text-slate-300">
                                <li><strong>الدرس الأول: الغلاف الجوي والطقس:</strong> الضغط الجوي، الرطوبة، والكتل الهوائية.</li>
                                <li><strong>الدرس الثاني: المناخ والموارد:</strong> دورة الماء والموارد الطبيعية المتجددة وغير المتجددة.</li>
                            </ul>
                        </div>

                        <div class="bg-pink-950/70 p-5 rounded-2xl border border-pink-500/40 space-y-2 card-bounce">
                            <span class="text-amber-400 font-extrabold block text-sm">الوحدة الخامسة: المادة</span>
                            <h4 class="font-black text-pink-300 text-sm">الفصل الخامس: خصائص المادة وتغيراتها</h4>
                            <ul class="list-disc list-inside space-y-1 text-slate-300">
                                <li><strong>الدرس الأول: الخصائص الفيزيائية:</strong> الكثافة، الحجم، الكتلة، حالات المادة الثلاث.</li>
                                <li><strong>الدرس الثاني: التغيرات الكيميائية:</strong> العناصر، المركبات والرموز والتفاعلات الكيميائية.</li>
                            </ul>
                        </div>

                        <div class="bg-rose-950/70 p-5 rounded-2xl border border-rose-500/40 space-y-2 card-bounce">
                            <span class="text-amber-400 font-extrabold block text-sm">الوحدة السادسة: القوى والطاقة</span>
                            <h4 class="font-black text-rose-300 text-sm">الفصل السادس: الحركة والكهرباء</h4>
                            <ul class="list-disc list-inside space-y-1 text-slate-300">
                                <li><strong>الدرس الأول: السرعة والقوة:</strong> قوانین نيوتن للحركة، الاحتكاك والسرعة المتجهة.</li>
                                <li><strong>الدرس الثاني: الكهرباء والمغناطيسية:</strong> الدوائر الكهربائية والمجال المغناطيسي.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ARABIC SECTION FULL -->
            <div id="curriculum-arabic" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-amber-500/40 shadow-2xl space-y-4">
                    <div class="flex items-center justify-between border-b border-amber-500/30 pb-3 flex-wrap gap-2">
                        <div class="flex items-center gap-3">
                            <span class="bg-amber-500/20 text-amber-300 text-xs font-black px-3 py-1 rounded-full border border-amber-500/40">لغتي الجميلة</span>
                            <h3 class="text-2xl font-black text-amber-300">جميع القواعد والوظائف النحوية والإملائية</h3>
                        </div>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 text-xs text-slate-200">
                        <div class="bg-amber-950/60 p-5 rounded-2xl border border-amber-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-amber-300 text-sm">📌 الوظيفة النحوية الكاملة</h4>
                            <ul class="list-disc list-inside space-y-1.5">
                                <li><strong>المبتدأ والخبر وكان/إن:</strong> رفعهما بالنواسخ والتغيرات الإعرابية.</li>
                                <li><strong>الأفعال الخمسة:</strong> ترفع بثبوت النون وتنصب وتجزم بحذفها (يفعلون، تفعلون...).</li>
                                <li><strong>الفاعل ونائب الفاعل:</strong> إعراب الفاعل والمفعول لم يسمى فاعله.</li>
                                <li><strong>المفاعيل المطلقة والمفعول لأجله وبه.</strong></li>
                            </ul>
                        </div>

                        <div class="bg-orange-950/60 p-5 rounded-2xl border border-orange-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-orange-300 text-sm">✒️ الظاهرة الإملائية والرسم</h4>
                            <ul class="list-disc list-inside space-y-1.5">
                                <li><strong>الهمزة المتوسطة:</strong> حسب أقوى الحركات (الكسرة ⬅️ الضمة ⬅️ الفتحة ⬅️ السكون).</li>
                                <li><strong>الهمزة المتطرفة:</strong> على الألف، الواو، الياء والسطر.</li>
                                <li><strong>الألف اللينة:</strong> في الأفعال والأسماء الثلاثية وغير الثلاثية (دعا، قضى).</li>
                                <li><strong>حروف الجر مع (ما) الاستفهامية:</strong> (عمَّ، فيمَ، علامَ).</li>
                            </ul>
                        </div>

                        <div class="bg-yellow-950/60 p-5 rounded-2xl border border-yellow-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-yellow-300 text-sm">💡 الصنف اللغوي والمشتقات</h4>
                            <ul class="list-disc list-inside space-y-1.5">
                                <li><strong>اسم الفاعل واسم المفعول:</strong> (كاتب، مكتوب).</li>
                                <li><strong>اسم الزمان والمكان:</strong> (مَشْرِق، مَلْعَب).</li>
                                <li><strong>اسم الآلة:</strong> (مِفْتَاح، مِغْرَفَة).</li>
                                <li><strong>المصادر الثلاثية وغير الثلاثية.</strong></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <!-- MATH SECTION FULL -->
            <div id="curriculum-math" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-emerald-500/40 shadow-2xl space-y-4">
                    <div class="flex items-center justify-between border-b border-emerald-500/30 pb-3">
                        <span class="bg-emerald-500/20 text-emerald-300 text-xs font-black px-3 py-1 rounded-full border border-emerald-500/40">الرياضيات الكاملة</span>
                        <h3 class="text-2xl font-black text-emerald-300">12 فصلاً بالكامل من الأساسيات للقياس والاحتساب</h3>
                    </div>

                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 text-xs text-slate-200">
                        <div class="bg-emerald-950/70 p-4 rounded-2xl border border-emerald-500/40 space-y-1 card-bounce">
                            <h4 class="font-black text-emerald-300 text-sm">1. الخطوات الأربع وتأصيل الأسس</h4>
                            <p>ترتيب العمليات بالأقواس، القوى والأسس، والتخمين والتحقق.</p>
                        </div>
                        <div class="bg-teal-950/70 p-4 rounded-2xl border border-teal-500/40 space-y-1 card-bounce">
                            <h4 class="font-black text-teal-300 text-sm">2. الإحصاء والبيانات</h4>
                            <p>المتوسط الحسابي، الوسيط، المنوال، والمدى والتمثيلات البيانية.</p>
                        </div>
                        <div class="bg-cyan-950/70 p-4 rounded-2xl border border-cyan-500/40 space-y-1 card-bounce">
                            <h4 class="font-black text-cyan-300 text-sm">3. الكسور العشرية</h4>
                            <p>جمع، طرح، ضرب وقسمة الكسور العشرية بالتقريب.</p>
                        </div>
                        <div class="bg-emerald-950/70 p-4 rounded-2xl border border-emerald-500/40 space-y-1 card-bounce">
                            <h4 class="font-black text-emerald-300 text-sm">4. الكسور الاعتيادية والتحليل</h4>
                            <p>التحليل العواملي، القاسم المشترك الأكبر (ق.م.أ) والمضاعف الأصغر.</p>
                        </div>
                        <div class="bg-teal-950/70 p-4 rounded-2xl border border-teal-500/40 space-y-1 card-bounce">
                            <h4 class="font-black text-teal-300 text-sm">5. العمليات على الكسور الاعتيادية</h4>
                            <p>جمع، طرح، ضرب وقسمة الكسور الاعتيادية والأعداد الكسرية.</p>
                        </div>
                        <div class="bg-cyan-950/70 p-4 rounded-2xl border border-cyan-500/40 space-y-1 card-bounce">
                            <h4 class="font-black text-cyan-300 text-sm">6. النسبة والتناسب</h4>
                            <p>معدل الوحدة، جدول النسبة والحل بالضرب التبادلي.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ISLAMIC SECTION FULL -->
            <div id="curriculum-islamic" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-teal-500/40 shadow-2xl space-y-4">
                    <h3 class="text-2xl font-black text-teal-300 border-b border-teal-500/30 pb-3">الدراسات الإسلامية (التوحيد، الفقه، الحديث، التفسير)</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-xs">
                        <div class="bg-teal-950/80 p-5 rounded-2xl border border-teal-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-teal-300 text-sm">✨ التوحيد والفقه</h4>
                            <p class="text-slate-200">أركان الإيمان الستة، أحكام الزكاة ومصارفها الثمانية، أحكام الصيام والحج والعمرة.</p>
                        </div>
                        <div class="bg-cyan-950/80 p-5 rounded-2xl border border-cyan-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-cyan-300 text-sm">📜 الحديث والتفسير والتجويد</h4>
                            <p class="text-slate-200">الأخلاق الإسلامية والشمائل النبوية، تفسير سور (الملك، القلم، الحاقة) وأحكام النون الساكنة.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- SOCIAL STUDIES SECTION FULL -->
            <div id="curriculum-social" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-rose-500/40 shadow-2xl space-y-4">
                    <h3 class="text-2xl font-black text-rose-300 border-b border-rose-500/30 pb-3">الدراسات الاجتماعية والرؤية 2030</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-xs">
                        <div class="bg-rose-950/80 p-5 rounded-2xl border border-rose-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-rose-300 text-sm">🇸🇦 تاريخ الوطن العظيم</h4>
                            <p class="text-slate-200">تأسيس الدولة السعودية الأولى (1139هـ)، الدولة الثانية والمملكة وتوحيدها على يد الملك عبدالعزيز.</p>
                        </div>
                        <div class="bg-pink-950/80 p-5 rounded-2xl border border-pink-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-pink-300 text-sm">🗺️ الجغرافيا ورؤية 2030</h4>
                            <p class="text-slate-200">تضاريس المملكة الخلابة، الخرائط، ومحاور رؤية 2030 والمشاريع الوطنية المبتكرة.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- DIGITAL SKILLS FULL -->
            <div id="curriculum-digital" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-blue-500/40 shadow-2xl space-y-4">
                    <h3 class="text-2xl font-black text-blue-300 border-b border-blue-500/30 pb-3">المهارات الرقمية والبرمجة</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-xs">
                        <div class="bg-blue-950/80 p-5 rounded-2xl border border-blue-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-blue-300 text-sm">👾 برمجة Scratch و Excel</h4>
                            <p class="text-slate-200">إنشاء الألعاب والقصص، الحلقات والشروط، الدوال الحسابية (SUM, AVERAGE) والمخططات البيانية.</p>
                        </div>
                        <div class="bg-indigo-950/80 p-5 rounded-2xl border border-indigo-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-indigo-300 text-sm">🔒 الأمن الرقمي و Word</h4>
                            <p class="text-slate-200">كلمات المرور القوية، الوقاية من التصيد الإلكتروني، وتنسيق المستندات وتصديرها بصيغة PDF.</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ENGLISH SECTION FULL -->
            <div id="curriculum-english" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-purple-500/40 shadow-2xl space-y-4">
                    <h3 class="text-2xl font-black text-purple-300 border-b border-purple-500/30 pb-3">English Curriculum (We Can)</h3>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4 text-xs">
                        <div class="bg-purple-950/80 p-5 rounded-2xl border border-purple-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-purple-300 text-sm">Unit 1 & 2: Life & Careers</h4>
                            <p class="text-slate-200">Chores, frequency adverbs (always, never), careers (doctor, pilot, architect, teacher).</p>
                        </div>
                        <div class="bg-fuchsia-950/80 p-5 rounded-2xl border border-fuchsia-500/40 space-y-2 card-bounce">
                            <h4 class="font-black text-fuchsia-300 text-sm">Unit 3 & 4: Grammar & Food</h4>
                            <p class="text-slate-200">Present Continuous, Past Simple, Comparative Adjectives (fast, faster, fastest).</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- ART SECTION FULL -->
            <div id="curriculum-art" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-pink-500/40 shadow-2xl space-y-4">
                    <h3 class="text-2xl font-black text-pink-300 border-b border-pink-500/30 pb-3">التربية الفنية والابتكار</h3>
                    <p class="text-xs text-slate-200">الزخارف الهندسيّة والنباتية، دائرة الألوان الحارة والباردة، النسيج السادة، وطباعة الاستنسل.</p>
                </div>
            </div>

            <!-- LIFE SKILLS SECTION FULL -->
            <div id="curriculum-lifeskills" class="subject-curriculum hidden space-y-6">
                <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-amber-500/40 shadow-2xl space-y-4">
                    <h3 class="text-2xl font-black text-amber-300 border-b border-amber-500/30 pb-3">المهارات الحياتية والأسرية</h3>
                    <p class="text-xs text-slate-200">الإسعافات الأولية (الحروق والرعاف)، ترتيب الوقت ومصروف الجيب، والعناية بالملابس والتغذية.</p>
                </div>
            </div>

        </section>

        <!-- SECTION: INTERACTIVE LAB (VIBRANT & GAMIFIED) -->
        <section id="tab-interactive" class="hidden space-y-6">
            <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-pink-500/40 shadow-2xl space-y-6">

                <!-- Tools Selector Tab -->
                <div class="flex gap-2 overflow-x-auto pb-2 border-b border-indigo-500/30">
                    <button onclick="switchInteractiveTool('microscope')" id="tool-btn-microscope" class="tool-tab-btn px-4 py-2.5 rounded-xl text-xs font-black bg-gradient-to-r from-pink-500 to-rose-500 text-white whitespace-nowrap shadow-md">
                        🔬 فحص العضيات بالمجهر
                    </button>
                    <button onclick="switchInteractiveTool('punnett')" id="tool-btn-punnett" class="tool-tab-btn px-4 py-2.5 rounded-xl text-xs font-black bg-slate-800/80 text-slate-300 whitespace-nowrap">
                        🧬 محاكي الوراثة وبانيت
                    </button>
                    <button onclick="switchInteractiveTool('grammar')" id="tool-btn-grammar" class="tool-tab-btn px-4 py-2.5 rounded-xl text-xs font-black bg-slate-800/80 text-slate-300 whitespace-nowrap">
                        📖 المحلل النحوي السحري
                    </button>
                    <button onclick="switchInteractiveTool('digital')" id="tool-btn-digital" class="tool-tab-btn px-4 py-2.5 rounded-xl text-xs font-black bg-slate-800/80 text-slate-300 whitespace-nowrap">
                        👾 استوديو سكراتش التفاعلي
                    </button>
                </div>

                <!-- TOOL 1: CELL MICROSCOPE INSPECTOR -->
                <div id="tool-microscope" class="tool-panel space-y-6">
                    <div class="flex items-center justify-between border-b border-slate-800 pb-3">
                        <div>
                            <h4 class="text-xl font-black text-pink-300 flex items-center gap-2">
                                <i class="fa-solid fa-microscope text-cyan-400"></i> المجهر الإلكتروني الفائق
                            </h4>
                            <p class="text-xs text-slate-300">انقر على العضية لاكتشاف أسرارها وكسب النقاط! ✨</p>
                        </div>
                    </div>

                    <!-- Organelle Selection Buttons Grid -->
                    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 gap-3">
                        <button onclick="inspectCell('nucleus')" class="p-4 vibrant-card-1 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">🎯</div>
                            <div class="font-black text-xs text-white">النواة</div>
                        </button>

                        <button onclick="inspectCell('mito')" class="p-4 vibrant-card-2 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">⚡</div>
                            <div class="font-black text-xs text-white">الميتوكندريا</div>
                        </button>

                        <button onclick="inspectCell('chloroplast')" class="p-4 vibrant-card-4 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">🍃</div>
                            <div class="font-black text-xs text-white">البلاستيدات الخضراء</div>
                        </button>

                        <button onclick="inspectCell('wall')" class="p-4 vibrant-card-5 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">🧱</div>
                            <div class="font-black text-xs text-white">الجدار الخلوي</div>
                        </button>

                        <button onclick="inspectCell('membrane')" class="p-4 vibrant-card-7 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">🛡️</div>
                            <div class="font-black text-xs text-white">الغشاء البلازمي</div>
                        </button>

                        <button onclick="inspectCell('vacuole')" class="p-4 vibrant-card-3 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">💧</div>
                            <div class="font-black text-xs text-white">الفجوة العصارية</div>
                        </button>

                        <button onclick="inspectCell('ribosome')" class="p-4 vibrant-card-8 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">⚙️</div>
                            <div class="font-black text-xs text-white">الرايبوسومات</div>
                        </button>

                        <button onclick="inspectCell('golgi')" class="p-4 vibrant-card-6 hover:brightness-110 rounded-2xl text-center space-y-1 transition hover:scale-105 active:scale-95 shadow-lg">
                            <div class="text-3xl">📦</div>
                            <div class="font-black text-xs text-white">أجسام جولجي</div>
                        </button>
                    </div>

                    <!-- Microscope View Result Screen -->
                    <div id="inspector-screen" class="bg-slate-950 p-6 rounded-3xl border-2 border-pink-500/50 flex flex-col md:flex-row items-center gap-6 shadow-2xl">
                        <div class="w-28 h-28 rounded-2xl bg-gradient-to-br from-indigo-500 to-purple-600 border border-indigo-400 flex items-center justify-center text-6xl shadow-xl" id="inspect-icon">
                            🔬
                        </div>
                        <div class="space-y-2 text-right flex-grow">
                            <span id="inspect-badge" class="px-3 py-1 bg-pink-500/20 text-pink-300 border border-pink-500/30 rounded-full text-xs font-black">المجهر الإلكتروني جاهز 🟢</span>
                            <h4 id="inspect-title" class="text-2xl font-black text-amber-300">اضغط على أي عضية بالأعلى!</h4>
                            <p id="inspect-desc" class="text-xs text-slate-200 leading-relaxed">ستظهر لك التشبيهات والمفاهيم العلمية بوضوح متناهٍ.</p>
                            <div id="inspect-tip" class="p-3 bg-indigo-900/60 border-r-4 border-amber-400 text-xs text-amber-200 rounded-xl font-black">💡 المعمل تحت تصرفك!</div>
                        </div>
                    </div>
                </div>

                <!-- TOOL 2: PUNNETT SQUARE SIMULATOR -->
                <div id="tool-punnett" class="tool-panel hidden space-y-6">
                    <div class="bg-slate-950 p-6 rounded-3xl border-2 border-amber-500/40 space-y-4 shadow-2xl">
                        <h4 class="font-black text-amber-300 text-lg flex items-center gap-2">
                            <i class="fa-solid fa-calculator text-amber-400"></i> محاكي الوراثة وتوقع ألوان الأزهار
                        </h4>

                        <div class="grid grid-cols-1 md:grid-cols-2 gap-4 bg-slate-900 p-4 rounded-2xl border border-slate-800">
                            <div>
                                <label class="text-xs text-cyan-300 font-bold block mb-1">جينات الأب:</label>
                                <select id="parent1" onchange="runPunnett()" class="w-full bg-slate-950 border border-indigo-500/40 text-amber-300 font-bold text-xs p-3 rounded-xl">
                                    <option value="PP">سائد نقي (PP) - أرجواني</option>
                                    <option value="Pp" selected>سائد هجين (Pp) - أرجواني</option>
                                    <option value="pp">متنحي نقي (pp) - أبيض</option>
                                </select>
                            </div>
                            <div>
                                <label class="text-xs text-cyan-300 font-bold block mb-1">جينات الأم:</label>
                                <select id="parent2" onchange="runPunnett()" class="w-full bg-slate-950 border border-indigo-500/40 text-amber-300 font-bold text-xs p-3 rounded-xl">
                                    <option value="PP">سائد نقي (PP) - أرجواني</option>
                                    <option value="Pp" selected>سائد هجين (Pp) - أرجواني</option>
                                    <option value="pp">متنحي نقي (pp) - أبيض</option>
                                </select>
                            </div>
                        </div>

                        <!-- Grid -->
                        <div class="max-w-md mx-auto bg-slate-900 p-5 rounded-2xl border-2 border-indigo-500/40">
                            <div class="grid grid-cols-3 gap-2 text-center text-xs font-black">
                                <div class="p-3 bg-slate-950 rounded-xl text-slate-400">الأم ⬅️<br>الأب ⬇️</div>
                                <div id="p2_a1" class="p-3 bg-indigo-900 text-indigo-200 rounded-xl text-lg">P</div>
                                <div id="p2_a2" class="p-3 bg-indigo-900 text-indigo-200 rounded-xl text-lg">p</div>

                                <div id="p1_a1" class="p-3 bg-purple-900 text-purple-200 rounded-xl text-lg flex items-center justify-center">P</div>
                                <div id="c1" class="p-3 bg-purple-950 border-2 border-emerald-400 text-emerald-300 rounded-xl text-base shadow">PP</div>
                                <div id="c2" class="p-3 bg-purple-950 border-2 border-emerald-400 text-emerald-300 rounded-xl text-base shadow">Pp</div>

                                <div id="p1_a2" class="p-3 bg-purple-900 text-purple-200 rounded-xl text-lg flex items-center justify-center">p</div>
                                <div id="c3" class="p-3 bg-purple-950 border-2 border-emerald-400 text-emerald-300 rounded-xl text-base shadow">Pp</div>
                                <div id="c4" class="p-3 bg-purple-950 border-2 border-rose-400 text-rose-300 rounded-xl text-base shadow">pp</div>
                            </div>
                        </div>
                        <div id="punnett-res" class="p-4 bg-indigo-950/80 border border-indigo-500/40 rounded-2xl text-xs text-center text-amber-200 font-black shadow-lg">
                            النتيجة المتوقعة: 75% أزهار أرجوانية (سائدة)، 25% أزهار بيضاء (متنحية).
                        </div>
                    </div>
                </div>

                <!-- TOOL 3: GRAMMAR ANALYZER -->
                <div id="tool-grammar" class="tool-panel hidden space-y-6">
                    <div class="bg-slate-950 p-6 rounded-3xl border-2 border-amber-500/40 space-y-4">
                        <h4 class="font-black text-amber-300 text-lg flex items-center gap-2">
                            <i class="fa-solid fa-spell-check text-amber-400"></i> المحلل النحوي السحري
                        </h4>
                        <div class="space-y-3">
                            <select id="grammar-sentence-select" onchange="runGrammarAnalysis()" class="w-full bg-slate-900 border-2 border-indigo-500/40 text-amber-300 font-bold text-xs md:text-sm p-3.5 rounded-2xl">
                                <option value="1">العلمُ نورٌ (جملة اسمية)</option>
                                <option value="2">كان العلمُ نوراً (كان وأخواتها)</option>
                                <option value="3">إنَّ العلمَ نورٌ (إنَّ وأخواتها)</option>
                                <option value="4">قرأ الطالبُ الكتابَ (جملة فعلية)</option>
                                <option value="5">المعلمون يكتبون الدرسَ (الأفعال الخمسة)</option>
                            </select>
                            <div id="grammar-result-box" class="p-4 bg-slate-900 rounded-2xl border border-slate-800 space-y-2 text-xs">
                                <!-- Dynamic Output -->
                            </div>
                        </div>
                    </div>
                </div>

                <!-- TOOL 4: SCRATCH CODE SIMULATOR -->
                <div id="tool-digital" class="tool-panel hidden space-y-6">
                    <div class="bg-slate-950 p-6 rounded-3xl border-2 border-cyan-500/40 space-y-4">
                        <h4 class="font-black text-cyan-300 text-lg flex items-center gap-2">
                            <i class="fa-solid fa-code text-cyan-400"></i> معمل البرمجة بسكراتش (Scratch Studio)
                        </h4>
                        <p class="text-xs text-slate-300">اضغط على اللبنات للتحكم بالحركة والحوار:</p>

                        <div class="flex flex-wrap gap-3">
                            <button onclick="runScratchAction('move')" class="px-5 py-2.5 bg-blue-600 hover:bg-blue-500 text-white font-black text-xs rounded-xl shadow-lg hover:scale-105 transition">تحرك 10 خطوات 🐱</button>
                            <button onclick="runScratchAction('say')" class="px-5 py-2.5 bg-purple-600 hover:bg-purple-500 text-white font-black text-xs rounded-xl shadow-lg hover:scale-105 transition">قل "أنا بطل سادس!" 💬</button>
                            <button onclick="runScratchAction('repeat')" class="px-5 py-2.5 bg-amber-500 hover:bg-amber-400 text-slate-950 font-black text-xs rounded-xl shadow-lg hover:scale-105 transition">شقلبة برمجية! 🔁</button>
                        </div>

                        <div id="scratch-stage" class="h-44 bg-slate-900 rounded-2xl border-2 border-cyan-500/30 flex items-center justify-center relative overflow-hidden shadow-inner">
                            <div id="scratch-cat" class="text-6xl transition-all duration-300">🐱</div>
                            <div id="scratch-bubble" class="absolute top-4 bg-white text-slate-950 text-xs font-black px-4 py-2 rounded-2xl shadow-xl border-2 border-indigo-500 hidden">أنا بطل سادس! 🚀</div>
                        </div>
                    </div>
                </div>

            </div>
        </section>

        <!-- SECTION: DICTIONARY OF ALL SUBJECTS -->
        <section id="tab-dictionary" class="hidden space-y-6">
            <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-cyan-500/40 shadow-2xl space-y-6">
                <div class="flex flex-wrap justify-between items-center gap-4">
                    <div>
                        <h3 class="text-2xl font-black text-amber-300">الموسوعة والشرح السريع لجميع المفاهيم 📖✨</h3>
                        <p class="text-xs text-slate-300">ابحث عن أي كلمة أو مصطلح في منهج سادس بالكامل!</p>
                    </div>
                </div>

                <!-- Search Input -->
                <div class="relative">
                    <input type="text" id="dict-search" onkeyup="filterDictionary()" placeholder="ابحث عن: ميتوكندريا، الأفعال الخمسة، الأسس، سكراتش، الدولة السعودية الأولى..." class="w-full bg-slate-950 border-2 border-indigo-500/40 rounded-2xl p-4 text-slate-100 placeholder-slate-400 text-sm focus:outline-none focus:border-pink-500 shadow-xl">
                    <i class="fa-solid fa-magnifying-glass absolute left-5 top-5 text-indigo-400 text-lg"></i>
                </div>

                <!-- Dictionary Grid -->
                <div id="dict-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 max-h-[600px] overflow-y-auto custom-scrollbar p-1">
                    <!-- Dynamic rendering via JS -->
                </div>
            </div>
        </section>

        <!-- SECTION: INTERACTIVE QUIZ (GAMIFIED) -->
        <section id="tab-quiz" class="hidden space-y-6">
            <div class="bg-slate-900/90 rounded-3xl p-6 border-2 border-pink-500/50 shadow-2xl space-y-6 max-w-3xl mx-auto relative overflow-hidden">
                <div class="flex justify-between items-center border-b border-indigo-500/30 pb-4 flex-wrap gap-2">
                    <div>
                        <h3 class="text-2xl font-black text-amber-300 flex items-center gap-2">
                            <i class="fa-solid fa-gamepad text-pink-400"></i> تحدي التفوق الشامل 🎯
                        </h3>
                        <p class="text-xs text-slate-300">أجب عن الأسئلة الممتعة لكسب الـ XP والأوسمة!</p>
                    </div>
                    <div class="bg-gradient-to-r from-indigo-900 to-purple-900 border-2 border-pink-500/40 px-5 py-2.5 rounded-2xl text-center shadow-lg">
                        <span class="text-xs text-slate-300 block font-bold">النقاط التي جمعتها</span>
                        <span id="quiz-score" class="text-2xl font-black text-amber-300">0 / 0</span>
                    </div>
                </div>

                <!-- Dynamic Quiz Question Box -->
                <div id="quiz-container" class="space-y-4">
                    <!-- Populated by JS -->
                </div>

                <div class="flex justify-between items-center pt-4 border-t border-indigo-500/20">
                    <button onclick="restartQuiz()" class="px-5 py-2.5 rounded-xl bg-slate-800 hover:bg-slate-700 text-xs font-black text-slate-200 transition">
                        <i class="fa-solid fa-rotate-right"></i> إعادة التحدي
                    </button>
                    <button id="next-btn" onclick="nextQuestion()" class="px-6 py-3 rounded-2xl bg-gradient-to-r from-pink-500 to-purple-600 hover:from-pink-600 hover:to-purple-700 text-sm font-black text-white transition shadow-xl hidden">
                        السؤال التالي <i class="fa-solid fa-arrow-left"></i>
                    </button>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-slate-950/80 border-t border-indigo-500/20 py-4 text-center text-xs text-indigo-300">
        <p>منصة التفهيم الذكية للصف السادس الابتدائي - مرجعك الممتع والشامل لكافة كتب ومواد المنهج ✨🚀</p>
    </footer>

    <!-- JavaScript Logic & Gamification Engine -->
    <script>
        // Gamification States
        let userXP = 0;
        let userLevel = 1;
        let badges = 0;

        function addXP(amount, reason) {
            userXP += amount;
            document.getElementById('user-xp-txt').innerText = userXP;

            // Level Up Condition
            if(userXP >= userLevel * 50) {
                userLevel++;
                document.getElementById('user-level-txt').innerText = `${userLevel} (بطل متفوق 👑)`;
                confetti({ particleCount: 100, spread: 70, origin: { y: 0.6 } });
            }
        }

        // Tab switching logic
        function switchTab(tabId) {
            document.querySelectorAll('main > section').forEach(sec => sec.classList.add('hidden'));
            const activeTab = document.getElementById('tab-' + tabId);
            if(activeTab) activeTab.classList.remove('hidden');

            document.querySelectorAll('.nav-btn').forEach(btn => {
                btn.classList.remove('bg-gradient-to-r', 'from-indigo-600', 'to-purple-600', 'text-white', 'shadow-lg');
                btn.classList.add('bg-slate-800/80', 'text-slate-300');
            });

            const currentNav = document.getElementById('nav-' + tabId);
            if(currentNav) {
                currentNav.classList.remove('bg-slate-800/80', 'text-slate-300');
                currentNav.classList.add('bg-gradient-to-r', 'from-indigo-600', 'to-purple-600', 'text-white', 'shadow-lg');
            }
        }

        // Subject Switching Logic
        function selectSubject(sub) {
            switchTab('curriculum');
            document.querySelectorAll('.subject-curriculum').forEach(el => el.classList.add('hidden'));
            
            const activeSub = document.getElementById('curriculum-' + sub);
            if(activeSub) activeSub.classList.remove('hidden');

            document.querySelectorAll('.sub-nav-btn').forEach(b => {
                b.classList.remove('bg-gradient-to-r', 'from-indigo-600', 'to-purple-600', 'text-white', 'shadow-md');
                b.classList.add('bg-slate-800/80', 'text-slate-300');
            });

            const activeBtn = document.getElementById('sub-btn-' + sub);
            if(activeBtn) {
                activeBtn.classList.remove('bg-slate-800/80', 'text-slate-300');
                activeBtn.classList.add('bg-gradient-to-r', 'from-indigo-600', 'to-purple-600', 'text-white', 'shadow-md');
            }

            addXP(5, "فتح مادة جديدة");
        }

        // Interactive Lab Tools Switching Logic
        function switchInteractiveTool(toolId) {
            document.querySelectorAll('.tool-panel').forEach(panel => panel.classList.add('hidden'));
            const activeTool = document.getElementById('tool-' + toolId);
            if(activeTool) activeTool.classList.remove('hidden');

            document.querySelectorAll('.tool-tab-btn').forEach(btn => {
                btn.classList.remove('bg-gradient-to-r', 'from-pink-500', 'to-rose-500', 'text-white', 'shadow-md');
                btn.classList.add('bg-slate-800/80', 'text-slate-300');
            });

            const activeBtn = document.getElementById('tool-btn-' + toolId);
            if(activeBtn) {
                activeBtn.classList.remove('bg-slate-800/80', 'text-slate-300');
                activeBtn.classList.add('bg-gradient-to-r', 'from-pink-500', 'to-rose-500', 'text-white', 'shadow-md');
            }

            if(toolId === 'grammar') runGrammarAnalysis();
            if(toolId === 'punnett') runPunnett();
        }

        // Organelle Inspection Data
        const cellData = {
            nucleus: {
                title: "النواة (Nucleus) - المركز الرئيسي",
                desc: "غرفة القيادة بالخلية! تحوي الـ DNA الملوّن وتدير كل الوظائف والوراثة.",
                icon: "🎯",
                tip: "💡 تشبيه ممتع: النواة مثل العقل المدبر أو كابتن الفريق!"
            },
            mito: {
                title: "الميتوكندريا - بيوت الطاقة",
                desc: "تأخذ الغذاء والأكسجين وتحوله لطاقة قوية تشغل الخلية بالكامل!",
                icon: "⚡",
                tip: "💡 تشبيه ممتع: الميتوكندريا هي الشاحن أو البطارية الفائقة!"
            },
            chloroplast: {
                title: "البلاستيدات الخضراء",
                desc: "توجد في الخلايا النباتية فقط، وتصنع السكر اللذيذ باستخدام ضوء الشمس.",
                icon: "🍃",
                tip: "💡 تشبيه ممتع: البلاستيدات مثل الألواح الشمسية ومطبخ النبات!"
            },
            wall: {
                title: "الجدار الخلوي الصلب",
                desc: "قلعة حماية صلبة تعطي الخلية النباتية قوّتها وشكلها المربع.",
                icon: "🧱",
                tip: "💡 تشبيه ممتع: الجدار الخلوي كـ الدروع الحصينة بالدرع!"
            },
            membrane: {
                title: "الغشاء البلازمي الذكي",
                desc: "بوابة ذكية تختار بدقة من يدخل ومن يخرج من الخلية.",
                icon: "🛡️",
                tip: "💡 تشبيه ممتع: الغشاء البلازمي كـ حارس البوابة الفطن!"
            },
            vacuole: {
                title: "الفجوة العصارية",
                desc: "مخزن ضخم للماء والمواد الغذائية (كبيرة بالنبات وصغيرة بالحيوان).",
                icon: "💧",
                tip: "💡 تشبيه ممتع: الفجوة العصارية هي الخزان الاحتياطي!"
            },
            ribosome: {
                title: "الرايبوسومات",
                desc: "مصانع متناهية الصغر لبناء البروتينات وتجديد أجزاء الخلية.",
                icon: "⚙️",
                tip: "💡 تشبيه ممتع: الرايبوسومات كـ عمال البناء الماهرين!"
            },
            golgi: {
                title: "أجسام جولجي الشاحنة",
                desc: "تغلف المواد وتجهزها للارسال إلى بقية أجزاء الخلية.",
                icon: "📦",
                tip: "💡 تشبيه ممتع: أجسام جولجي كـ شركة الشحن والتغليف السريع!"
            }
        };

        function inspectCell(key) {
            const data = cellData[key];
            if(!data) return;

            document.getElementById('inspect-icon').innerText = data.icon;
            document.getElementById('inspect-title').innerText = data.title;
            document.getElementById('inspect-desc').innerText = data.desc;
            document.getElementById('inspect-tip').innerText = data.tip;

            addXP(5, "فحص عضية بالخلية");
        }

        // Punnett Logic
        function runPunnett() {
            const p1 = document.getElementById('parent1').value;
            const p2 = document.getElementById('parent2').value;

            document.getElementById('p1_a1').innerText = p1[0];
            document.getElementById('p1_a2').innerText = p1[1];
            document.getElementById('p2_a1').innerText = p2[0];
            document.getElementById('p2_a2').innerText = p2[1];

            document.getElementById('c1').innerText = p1[0] + p2[0];
            document.getElementById('c2').innerText = p1[0] + p2[1];
            document.getElementById('c3').innerText = p1[1] + p2[0];
            document.getElementById('c4').innerText = p1[1] + p2[1];
        }

        // Grammar Logic
        function runGrammarAnalysis() {
            const val = document.getElementById('grammar-sentence-select').value;
            const box = document.getElementById('grammar-result-box');

            const parseMap = {
                "1": [
                    { word: "العلمُ", parse: "مبتدأ مرفوع وعلامة رفعه الضمة الظاهرة." },
                    { word: "نورٌ", parse: "خبر المبتدأ مرفوع وعلامة رفعه الضمة الظاهرة." }
                ],
                "2": [
                    { word: "كان", parse: "فعل ماضٍ ناقص ناسخ يرفع المبتدأ وينصب الخبر." },
                    { word: "العلمُ", parse: "اسم كان مرفوع وعلامة رفعه الضمة الظاهرة." },
                    { word: "نوراً", parse: "خبر كان منصوب وعلامة نصبه الفتحة الظاهرة." }
                ],
                "3": [
                    { word: "إنَّ", parse: "حرف ناسخ ينصب المبتدأ ويرفع الخبر." },
                    { word: "العلمَ", parse: "اسم إنَّ منصوب وعلامة نصبه الفتحة الظاهرة." },
                    { word: "نورٌ", parse: "خبر إنَّ مرفوع وعلامة رفعه الضمة الظاهرة." }
                ],
                "4": [
                    { word: "قرأ", parse: "فعل ماضٍ مبني على الفتح." },
                    { word: "الطالبُ", parse: "فاعل مرفوع وعلامة رفعه الضمة الظاهرة." },
                    { word: "الكتابَ", parse: "مفعول به منصوب وعلامة نصبه الفتحة الظاهرة." }
                ],
                "5": [
                    { word: "المعلمون", parse: "مبتدأ مرفوع بالواو لأنه جمع مذكر سالم." },
                    { word: "يكتبون", parse: "فعل مضارع مرفوع بثبوت النون لأنه من الأفعال الخمسة." },
                    { word: "الدرسَ", parse: "مفعول به منصوب وعلامة نصبه الفتحة." }
                ]
            };

            const items = parseMap[val] || [];
            let html = '';
            items.forEach(item => {
                html += `
                    <div class="p-3 bg-slate-950 rounded-xl border border-indigo-500/30 flex gap-3 items-center">
                        <span class="text-amber-400 font-black text-sm min-w-[80px]">${item.word}:</span>
                        <span class="text-slate-200 font-bold">${item.parse}</span>
                    </div>
                `;
            });
            box.innerHTML = html;
        }

        // Scratch Simulator Action
        let posX = 0;
        function runScratchAction(action) {
            const cat = document.getElementById('scratch-cat');
            const bubble = document.getElementById('scratch-bubble');

            if(action === 'move') {
                posX += 35;
                if(posX > 160) posX = -160;
                cat.style.transform = `translateX(${posX}px)`;
            } else if(action === 'say') {
                bubble.classList.remove('hidden');
                setTimeout(() => bubble.classList.add('hidden'), 2200);
            } else if(action === 'repeat') {
                cat.style.transform = `scale(1.4) rotate(360deg)`;
                setTimeout(() => cat.style.transform = `translateX(${posX}px) scale(1) rotate(0deg)`, 600);
            }
            addXP(5, "حركة برمجية جديدة");
        }

        // Comprehensive Dictionary Data
        const allSubjectsDict = [
            { sub: "علوم", title: "الخلية", desc: "الوحدة الأساسية لبناء كافة الكائنات الحية." },
            { sub: "علوم", title: "الميتوكندريا", desc: "مصنع توليد الطاقة في الخلية." },
            { sub: "علوم", title: "البناء الضوئي", desc: "صنع النبات لغنائه باستخدام الضوء." },
            { sub: "علوم", title: "التعاقب البيئي", desc: "التغير التدريجي الكائنات بمكان محدد." },
            { sub: "لغتي", title: "المبتدأ والخبر", desc: "ركنا الجملة الاسمية المرفوعان." },
            { sub: "لغتي", title: "الأفعال الخمسة", desc: "أفعال مضارعة اتصلت بألف اثنين أو واو جماعة أو ياء مخاطبة." },
            { sub: "لغتي", title: "اسم الفاعل والمفعول", desc: "مشتقات تدل على من قام بالفعل أو من وقع عليه." },
            { sub: "مهارات رقمية", title: "Scratch", desc: "لغة برمجة رسومية باللبنات الملونة." },
            { sub: "رياضيات", title: "ق.م.أ و م.م.أ", desc: "القاسم المشترك الأكبر والمضاعف المشترك الأصغر." },
            { sub: "رياضيات", title: "النسبة والتناسب", desc: "المقارنة بين كميتين واستخراج التكافؤ." },
            { sub: "دراسات إسلامية", title: "مصارف الزكاة", desc: "الجهات الثمان المستحقة للزكاة." },
            { sub: "دراسات اجتماعية", title: "الدولة السعودية الأولى", desc: "تأسست عام 1139 هـ على يد الإمام محمد بن سعود." }
        ];

        function renderAllDictionary() {
            const grid = document.getElementById('dict-grid');
            let html = '';
            allSubjectsDict.forEach(item => {
                html += `
                    <div class="dict-card bg-slate-950/80 p-4 rounded-2xl border border-indigo-500/30 space-y-2 card-bounce">
                        <div class="flex items-center justify-between">
                            <h4 class="font-black text-amber-300 text-sm">${item.title}</h4>
                            <span class="px-2.5 py-0.5 rounded-full text-[10px] font-black bg-pink-500/20 text-pink-300 border border-pink-500/30">${item.sub}</span>
                        </div>
                        <p class="text-xs text-slate-200 leading-relaxed">${item.desc}</p>
                    </div>
                `;
            });
            grid.innerHTML = html;
        }

        function filterDictionary() {
            const query = document.getElementById('dict-search').value.toLowerCase();
            const cards = document.querySelectorAll('.dict-card');
            cards.forEach(card => {
                const text = card.innerText.toLowerCase();
                card.style.display = text.includes(query) ? 'block' : 'none';
            });
        }

        // Comprehensive Quiz Data
        const quizList = [
            {
                q: "العضية المسؤولّة عن عملية البناء الضوئي في النبات هي:",
                opts: ["الميتوكندريا", "البلاستيدات الخضراء", "النواة", "الجدار الخلوي"],
                ans: 1,
                exp: "البلاستيدات تصنع السكر والغذاء بضوء الشمس!"
            },
            {
                q: "القاسم المشترك الأكبر (ق.م.أ) للعددين 12 و 18 هو:",
                opts: ["3", "6", "12", "36"],
                ans: 1,
                exp: "أكبر رقم يقبل القسمة عليهما بدون باقٍ هو 6."
            },
            {
                q: "إعراب كلمة (العلمُ) في جملة «كان العلمُ نوراً»:",
                opts: ["مبتدأ مرفوع", "اسم كان مرفوع", "خبر كان منصوب", "فاعل مرفوع"],
                ans: 1,
                exp: "كان تدخل وترفع الاسم ويسمى اسمها!"
            },
            {
                q: "تأسست الدولة السعودية الأولى عام 1139هـ على يد الإمام:",
                opts: ["تركي بن عبد الله", "محمد بن سعود", "عبد العزيز آل سعود", "سعود بن عبد العزيز"],
                ans: 1,
                exp: "أسسها الإمام محمد بن سعود رحمه الله عام 1139هـ."
            }
        ];

        let qIndex = 0;
        let scoreCount = 0;

        function loadQuizQ() {
            const container = document.getElementById('quiz-container');
            const q = quizList[qIndex];
            document.getElementById('next-btn').classList.add('hidden');

            let html = `
                <div class="space-y-4">
                    <span class="text-xs text-pink-400 font-black block">السؤال ${qIndex + 1} من ${quizList.length}</span>
                    <h4 class="text-base md:text-xl font-black text-white">${q.q}</h4>
                    <div class="grid grid-cols-1 gap-2.5 pt-2">
            `;

            q.opts.forEach((opt, i) => {
                html += `
                    <button onclick="submitQuizAns(${i})" class="quiz-opt-btn w-full text-right p-4 rounded-2xl bg-slate-950 hover:bg-slate-800 border-2 border-indigo-500/30 text-xs md:text-sm text-slate-100 font-bold transition flex items-center justify-between shadow-lg">
                        <span>${opt}</span>
                        <i class="fa-regular fa-circle text-indigo-400"></i>
                    </button>
                `;
            });

            html += `</div><div id="quiz-msg" class="mt-3"></div></div>`;
            container.innerHTML = html;
        }

        function submitQuizAns(selected) {
            const q = quizList[qIndex];
            const btns = document.querySelectorAll('.quiz-opt-btn');
            const msg = document.getElementById('quiz-msg');
            const nextBtn = document.getElementById('next-btn');

            btns.forEach(b => b.disabled = true);

            if(selected === q.ans) {
                scoreCount++;
                document.getElementById('quiz-score').innerText = `${scoreCount} / ${quizList.length}`;
                btns[selected].classList.add('bg-emerald-900', 'border-emerald-400', 'text-white');
                msg.innerHTML = `<div class="p-3 bg-emerald-950 border border-emerald-400 rounded-2xl text-xs text-emerald-300 font-black">🎉 إجابة رائعة وصحيحة! +20 XP</div>`;
                addXP(20, "إجابة اختبار صحيحة");
                confetti({ particleCount: 50, spread: 60, origin: { y: 0.7 } });
            } else {
                btns[selected].classList.add('bg-rose-900', 'border-rose-400', 'text-white');
                btns[q.ans].classList.add('bg-emerald-900', 'border-emerald-400', 'text-white');
                msg.innerHTML = `<div class="p-3 bg-rose-950 border border-rose-400 rounded-2xl text-xs text-rose-300 font-bold">❌ إجابة خاطئة. الشرح: ${q.exp}</div>`;
            }

            if(qIndex < quizList.length - 1) {
                nextBtn.classList.remove('hidden');
            }
        }

        function nextQuestion() {
            if(qIndex < quizList.length - 1) {
                qIndex++;
                loadQuizQ();
            }
        }

        function restartQuiz() {
            qIndex = 0;
            scoreCount = 0;
            document.getElementById('quiz-score').innerText = `0 / ${quizList.length}`;
            loadQuizQ();
        }

        // Init
        window.onload = function() {
            renderAllDictionary();
            loadQuizQ();
            runPunnett();
            runGrammarAnalysis();
            inspectCell('nucleus');
        };
    </script>
</body>
</html>
