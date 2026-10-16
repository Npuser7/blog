# blog<!DOCTYPE html>
<html lang="ko" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>김개발 | 소프트웨어 엔지니어 & 크리에이터 포트폴리오</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'Noto Sans KR', 'sans-serif'],
                    },
                    colors: {
                        brand: {
                            50: '#eef2ff',
                            100: '#e0e7ff',
                            500: '#6366f1',
                            600: '#4f46e5',
                            700: '#4338ca',
                        }
                    }
                }
            }
        }
    </script>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Noto+Sans+KR:wght@300;400;500;700&display=swap" rel="stylesheet">
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Inter', 'Noto Sans KR', sans-serif;
        }
        /* Custom smooth transition for dark mode */
        body, * {
            transition: background-color 0.3s ease, border-color 0.3s ease, color 0.3s ease;
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 dark:bg-slate-950 dark:text-slate-100 antialiased selection:bg-brand-500 selection:text-white">

    <!-- 상단 네비게이션 바 -->
    <header class="fixed top-0 left-0 right-0 z-50 backdrop-blur-md bg-white/80 dark:bg-slate-900/80 border-b border-slate-200 dark:border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 h-16 flex items-center justify-between">
            <!-- 로고 -->
            <a href="#hero" class="text-xl font-bold tracking-tight bg-gradient-to-r from-brand-500 to-indigo-400 bg-clip-text text-transparent">
                Dev.Kim
            </a>

            <!-- 데스크탑 메뉴 -->
            <nav class="hidden md:flex items-center space-x-8 text-sm font-medium">
                <a href="#about" class="hover:text-brand-500 transition-colors">소개</a>
                <a href="#skills" class="hover:text-brand-500 transition-colors">기술 스택</a>
                <a href="#projects" class="hover:text-brand-500 transition-colors">프로젝트</a>
                <a href="#timeline" class="hover:text-brand-500 transition-colors">타임라인</a>
                <a href="#contact" class="hover:text-brand-500 transition-colors">연락처</a>
            </nav>

            <!-- 우측 액션 (다크모드 토글 & 모바일 메뉴 버튼) -->
            <div class="flex items-center space-x-4">
                <button id="theme-toggle" aria-label="다크모드 토글" class="p-2 rounded-full hover:bg-slate-100 dark:hover:bg-slate-800 text-slate-600 dark:text-slate-300 transition-colors">
                    <i id="theme-icon" class="fa-solid fa-moon text-lg"></i>
                </button>
                <button id="mobile-menu-button" aria-label="메뉴 열기" class="md:hidden p-2 rounded-lg hover:bg-slate-100 dark:hover:bg-slate-800 text-slate-600 dark:text-slate-300">
                    <i class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- 모바일 드롭다운 메뉴 -->
        <div id="mobile-menu" class="hidden md:hidden px-4 pt-2 pb-4 space-y-2 border-t border-slate-200 dark:border-slate-800 bg-white dark:bg-slate-900">
            <a href="#about" class="block py-2 px-3 rounded-md hover:bg-slate-100 dark:hover:bg-slate-850">소개</a>
            <a href="#skills" class="block py-2 px-3 rounded-md hover:bg-slate-100 dark:hover:bg-slate-850">기술 스택</a>
            <a href="#projects" class="block py-2 px-3 rounded-md hover:bg-slate-100 dark:hover:bg-slate-850">프로젝트</a>
            <a href="#timeline" class="block py-2 px-3 rounded-md hover:bg-slate-100 dark:hover:bg-slate-850">타임라인</a>
            <a href="#contact" class="block py-2 px-3 rounded-md hover:bg-slate-100 dark:hover:bg-slate-850">연락처</a>
        </div>
    </header>

    <!-- 메인 콘텐츠 영역 -->
    <main>
        <!-- Hero 섹션 -->
        <section id="hero" class="min-h-screen flex items-center justify-center pt-16 relative overflow-hidden">
            <div class="absolute inset-0 -z-10 bg-[radial-gradient(ellipse_at_top,_var(--tw-gradient-stops))] from-brand-100 via-transparent dark:from-brand-950/30 dark:via-transparent"></div>
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20 text-center">
                <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full text-xs font-semibold bg-brand-50 text-brand-600 dark:bg-brand-950/60 dark:text-brand-400 mb-6 border border-brand-200 dark:border-brand-800">
                    <span class="relative flex h-2 w-2">
                      <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-brand-400 opacity-75"></span>
                      <span class="relative inline-flex rounded-full h-2 w-2 bg-brand-500"></span>
                    </span>
                    새로운 도전을 기다리고 있습니다
                </div>
                <h1 class="text-4xl sm:text-6xl lg:text-7xl font-extrabold tracking-tight mb-6">
                    안녕하세요, <br class="sm:hidden" /><span class="bg-gradient-to-r from-brand-500 via-indigo-500 to-purple-500 bg-clip-text text-transparent">소프트웨어 엔지니어</span><br />김개발입니다.
                </h1>
                <p class="max-w-2xl mx-auto text-lg sm:text-xl text-slate-600 dark:text-slate-400 mb-10 leading-relaxed">
                    사용자 경험을 최우선으로 생각하며, 견고하고 확장 가능한 웹 서비스를 만드는 것을 즐깁니다. 최신 기술로 가치를 창출합니다.
                </p>
                <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
                    <a href="#projects" class="w-full sm:w-auto px-8 py-4 rounded-xl bg-brand-600 hover:bg-brand-700 text-white font-medium shadow-lg shadow-brand-500/25 transition-all transform hover:-translate-y-0.5">
                        프로젝트 보기 <i class="fa-solid fa-arrow-right ml-2 text-sm"></i>
                    </a>
                    <a href="#contact" class="w-full sm:w-auto px-8 py-4 rounded-xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 hover:bg-slate-50 dark:hover:bg-slate-800 font-medium transition-all">
                        연락하기
                    </a>
                </div>
            </div>
        </section>

        <!-- About Me 섹션 -->
        <section id="about" class="py-24 bg-white dark:bg-slate-900/50 border-t border-slate-200 dark:border-slate-800">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-16">
                    <h2 class="text-3xl font-bold tracking-tight mb-4">About Me</h2>
                    <p class="text-slate-600 dark:text-slate-400 max-w-xl mx-auto">저를 소개하고 지향하는 가치관을 공유합니다.</p>
                </div>
                <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
                    <!-- 프로필 이미지 대체 카드 -->
                    <div class="lg:col-span-5 flex justify-center">
                        <div class="relative w-72 h-72 sm:w-80 sm:h-80 rounded-2xl overflow-hidden shadow-2xl bg-gradient-to-tr from-brand-500 to-indigo-400 p-2">
                            <div class="w-full h-full bg-slate-100 dark:bg-slate-900 rounded-xl flex flex-col items-center justify-center text-center p-6">
                                <i class="fa-solid fa-code text-6xl text-brand-500 mb-4"></i>
                                <h3 class="font-bold text-xl mb-1">김개발 (Kim Dev)</h3>
                                <p class="text-xs text-slate-500 dark:text-slate-400">Full-Stack Engineer</p>
                            </div>
                        </div>
                    </div>
                    <!-- 자기소개 상세 텍스트 -->
                    <div class="lg:col-span-7 space-y-6">
                        <h3 class="text-2xl font-semibold">문제 해결을 즐기는 개발자, 사용자 중심의 가치를 만듭니다.</h3>
                        <p class="text-slate-600 dark:text-slate-400 leading-relaxed">
                            웹 표준과 클린 코드를 지향하며, 프론트엔드와 백엔드를 아우르는 폭넓은 시야를 가지고 있습니다. 단순히 동작하는 코드를 넘어, 유지보수가 용이하고 성능이 최적화된 아키텍처 구성을 고민합니다.
                        </p>
                        <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-2">
                            <div class="p-4 rounded-xl bg-slate-50 dark:bg-slate-800 border border-slate-100 dark:border-slate-700/50">
                                <div class="text-brand-500 font-bold text-xl mb-1">3+ 년</div>
                                <div class="text-sm text-slate-600 dark:text-slate-400">실무 개발 경력</div>
                            </div>
                            <div class="p-4 rounded-xl bg-slate-50 dark:bg-slate-800 border border-slate-100 dark:border-slate-700/50">
                                <div class="text-brand-500 font-bold text-xl mb-1">20+ 건</div>
                                <div class="text-sm text-slate-600 dark:text-slate-400">완료된 프로젝트 및 서비스</div>
                            </div>
                        </div>
                        <div class="pt-4 flex flex-wrap gap-3">
                            <span class="px-3 py-1 bg-slate-100 dark:bg-slate-800 rounded-full text-xs font-medium">#협업지향적</span>
                            <span class="px-3 py-1 bg-slate-100 dark:bg-slate-800 rounded-full text-xs font-medium">#클린코드</span>
                            <span class="px-3 py-1 bg-slate-100 dark:bg-slate-800 rounded-full text-xs font-medium">#지속적성장</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Skills 섹션 -->
        <section id="skills" class="py-24">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-16">
                    <h2 class="text-3xl font-bold tracking-tight mb-4">Tech Stack</h2>
                    <p class="text-slate-600 dark:text-slate-400 max-w-xl mx-auto">주로 다루는 기술 및 도구들입니다.</p>
                </div>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    <!-- Frontend -->
                    <div class="p-6 rounded-2xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 shadow-sm">
                        <div class="w-12 h-12 rounded-xl bg-brand-50 dark:bg-brand-950/50 flex items-center justify-center text-brand-500 mb-6 text-xl">
                            <i class="fa-solid fa-laptop-code"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Frontend</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">HTML5 / CSS3</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">JavaScript (ES6+)</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">TypeScript</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">React / Next.js</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Tailwind CSS</span>
                        </div>
                    </div>
                    <!-- Backend -->
                    <div class="p-6 rounded-2xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 shadow-sm">
                        <div class="w-12 h-12 rounded-xl bg-brand-50 dark:bg-brand-950/50 flex items-center justify-center text-brand-500 mb-6 text-xl">
                            <i class="fa-solid fa-server"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Backend</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Node.js</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Express</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Python</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">FastAPI</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">PostgreSQL / MongoDB</span>
                        </div>
                    </div>
                    <!-- Tools & DevOps -->
                    <div class="p-6 rounded-2xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 shadow-sm">
                        <div class="w-12 h-12 rounded-xl bg-brand-50 dark:bg-brand-950/50 flex items-center justify-center text-brand-500 mb-6 text-xl">
                            <i class="fa-solid fa-toolbox"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-4">Tools & DevOps</h3>
                        <div class="flex flex-wrap gap-2">
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Git / GitHub</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Docker</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">AWS (EC2, S3)</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Vercel</span>
                            <span class="px-3 py-1.5 rounded-lg bg-slate-100 dark:bg-slate-800 text-sm font-medium">Figma</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Projects 섹션 -->
        <section id="projects" class="py-24 bg-white dark:bg-slate-900/50 border-t border-slate-200 dark:border-slate-800">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-12">
                    <h2 class="text-3xl font-bold tracking-tight mb-4">Featured Projects</h2>
                    <p class="text-slate-600 dark:text-slate-400 max-w-xl mx-auto">주요 프로젝트 작업물들을 소개합니다.</p>
                </div>

                <!-- 필터 버튼 -->
                <div class="flex justify-center gap-2 mb-12 flex-wrap">
                    <button class="project-filter px-4 py-2 rounded-full text-sm font-medium bg-brand-600 text-white shadow-sm transition-all" data-filter="all">전체</button>
                    <button class="project-filter px-4 py-2 rounded-full text-sm font-medium bg-slate-100 dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition-all" data-filter="web">웹 서비스</button>
                    <button class="project-filter px-4 py-2 rounded-full text-sm font-medium bg-slate-100 dark:bg-slate-800 text-slate-600 dark:text-slate-300 hover:bg-slate-200 dark:hover:bg-slate-700 transition-all" data-filter="app">모바일/앱</button>
                </div>

                <!-- 프로젝트 카드 그리드 -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- 프로젝트 1 -->
                    <div class="project-card group rounded-2xl overflow-hidden bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-800 flex flex-col transition-all hover:shadow-xl" data-category="web">
                        <div class="h-48 bg-gradient-to-br from-indigo-500 to-purple-600 relative overflow-hidden flex items-center justify-center p-6">
                            <i class="fa-solid fa-bag-shopping text-white/30 text-7xl absolute -bottom-4 -right-4 group-hover:scale-110 transition-transform"></i>
                            <span class="relative z-10 text-white font-bold text-2xl tracking-wider">E-Commerce Platform</span>
                        </div>
                        <div class="p-6 flex-1 flex flex-col justify-between">
                            <div>
                                <div class="flex gap-2 mb-3">
                                    <span class="text-xs px-2.5 py-1 rounded-md bg-brand-50 dark:bg-brand-950/60 text-brand-600 dark:text-brand-400 font-medium">React</span>
                                    <span class="text-xs px-2.5 py-1 rounded-md bg-slate-200/60 dark:bg-slate-800 text-slate-600 dark:text-slate-300 font-medium">Node.js</span>
                                </div>
                                <h3 class="text-xl font-bold mb-2">모던 이커머스 쇼핑몰</h3>
                                <p class="text-sm text-slate-600 dark:text-slate-400 mb-4 line-clamp-3">
                                    결제 시스템 연동 및 장바구니 기능을 포함한 반응형 쇼핑몰 웹 어플리케이션입니다. 사용자 친화적 UI를 구현했습니다.
                                </p>
                            </div>
                            <div class="flex items-center gap-4 pt-4 border-t border-slate-200 dark:border-slate-800 text-sm font-medium">
                                <a href="#" class="text-brand-600 dark:text-brand-400 hover:underline flex items-center gap-1.5">
                                    <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i> 라이브 Demo
                                </a>
                                <a href="#" class="text-slate-600 dark:text-slate-400 hover:text-slate-900 dark:hover:text-white flex items-center gap-1.5">
                                    <i class="fa-brands fa-github">></i> GitHub
                                </a>
                            </div>
                        </div>
                    </div>

                    <!-- 프로젝트 2 -->
                    <div class="project-card group rounded-2xl overflow-hidden bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-800 flex flex-col transition-all hover:shadow-xl" data-category="app">
                        <div class="h-48 bg-gradient-to-br from-blue-500 to-cyan-500 relative overflow-hidden flex items-center justify-center p-6">
                            <i class="fa-solid fa-chart-line text-white/30 text-7xl absolute -bottom-4 -right-4 group-hover:scale-110 transition-transform"></i>
                            <span class="relative z-10 text-white font-bold text-2xl tracking-wider">Dashboard & Analytics</span>
                        </div>
                        <div class="p-6 flex-1 flex flex-col justify-between">
                            <div>
                                <div class="flex gap-2 mb-3">
                                    <span class="text-xs px-2.5 py-1 rounded-md bg-brand-50 dark:bg-brand-950/60 text-brand-600 dark:text-brand-400 font-medium">Next.js</span>
                                    <span class="text-xs px-2.5 py-1 rounded-md bg-slate-200/60 dark:bg-slate-800 text-slate-600 dark:text-slate-300 font-medium">Tailwind</span>
                                </div>
                                <h3 class="text-xl font-bold mb-2">실시간 데이터 분석 대시보드</h3>
                                <p class="text-sm text-slate-600 dark:text-slate-400 mb-4 line-clamp-3">
                                    다양한 지표와 통계를 실시간으로 차트 시각화하여 제공하는 관리자용 웹 대시보드 프로젝트입니다.
                                </p>
                            </div>
                            <div class="flex items-center gap-4 pt-4 border-t border-slate-200 dark:border-slate-800 text-sm font-medium">
                                <a href="#" class="text-brand-600 dark:text-brand-400 hover:underline flex items-center gap-1.5">
                                    <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i> 라이브 Demo
                                </a>
                                <a href="#" class="text-slate-600 dark:text-slate-400 hover:text-slate-900 dark:hover:text-white flex items-center gap-1.5">
                                    <i class="fa-brands fa-github"></i> GitHub
                                </a>
                            </div>
                        </div>
                    </div>

                    <!-- 프로젝트 3 -->
                    <div class="project-card group rounded-2xl overflow-hidden bg-slate-50 dark:bg-slate-900 border border-slate-200 dark:border-slate-800 flex flex-col transition-all hover:shadow-xl" data-category="web">
                        <div class="h-48 bg-gradient-to-br from-emerald-500 to-teal-600 relative overflow-hidden flex items-center justify-center p-6">
                            <i class="fa-solid fa-comments text-white/30 text-7xl absolute -bottom-4 -right-4 group-hover:scale-110 transition-transform"></i>
                            <span class="relative z-10 text-white font-bold text-2xl tracking-wider">Chat Community</span>
                        </div>
                        <div class="p-6 flex-1 flex flex-col justify-between">
                            <div>
                                <div class="flex gap-2 mb-3">
                                    <span class="text-xs px-2.5 py-1 rounded-md bg-brand-50 dark:bg-brand-950/60 text-brand-600 dark:text-brand-400 font-medium">TypeScript</span>
                                    <span class="text-xs px-2.5 py-1 rounded-md bg-slate-200/60 dark:bg-slate-800 text-slate-600 dark:text-slate-300 font-medium">Socket.io</span>
                                </div>
                                <h3 class="text-xl font-bold mb-2">실시간 채팅 커뮤니티</h3>
                                <p class="text-sm text-slate-600 dark:text-slate-400 mb-4 line-clamp-3">
                                    웹소켓 기술을 활용하여 지연 없는 실시간 메시징과 채널 기능을 지원하는 커뮤니티 플랫폼입니다.
                                </p>
                            </div>
                            <div class="flex items-center gap-4 pt-4 border-t border-slate-200 dark:border-slate-800 text-sm font-medium">
                                <a href="#" class="text-brand-600 dark:text-brand-400 hover:underline flex items-center gap-1.5">
                                    <i class="fa-solid fa-arrow-up-right-from-square text-xs"></i> 라이브 Demo
                                </a>
                                <a href="#" class="text-slate-600 dark:text-slate-400 hover:text-slate-900 dark:hover:text-white flex items-center gap-1.5">
                                    <i class="fa-brands fa-github"></i> GitHub
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 타임라인 섹션 (경력/학력) -->
        <section id="timeline" class="py-24">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-16">
                    <h2 class="text-3xl font-bold tracking-tight mb-4">Experience & Education</h2>
                    <p class="text-slate-600 dark:text-slate-400">발자취와 성장 과정입니다.</p>
                </div>

                <div class="relative border-l border-slate-200 dark:border-slate-800 ml-4 sm:ml-32 space-y-12">
                    <!-- 경력 1 -->
                    <div class="relative pl-8 sm:pl-10">
                        <div class="absolute -left-3.5 top-1.5 w-7 h-7 rounded-full bg-brand-500 border-4 border-white dark:border-slate-950 flex items-center justify-center text-white text-xs">
                            <i class="fa-solid fa-briefcase"></i>
                        </div>
                        <div class="absolute left-[-160px] top-1.5 hidden sm:block text-right w-28 text-sm font-semibold text-slate-400">
                            2022.03 ~ 현재
                        </div>
                        <div class="p-6 rounded-2xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 shadow-sm">
                            <span class="sm:hidden text-xs font-semibold text-brand-500 mb-1 block">2022.03 ~ 현재</span>
                            <h3 class="text-xl font-bold">프론트엔드/백엔드 엔지니어</h3>
                            <div class="text-brand-600 dark:text-brand-400 font-medium text-sm mb-3">(주) 테크노베이션</div>
                            <p class="text-sm text-slate-600 dark:text-slate-400 leading-relaxed">
                                사내 핵심 웹 서비스의 프론트엔드 아키텍처 개선 및 레거시 코드 리팩토링을 주도하였으며, 서버 성능 최적화를 통해 로딩 속도를 35% 단축했습니다.
                            </p>
                        </div>
                    </div>

                    <!-- 경력 2 -->
                    <div class="relative pl-8 sm:pl-10">
                        <div class="absolute -left-3.5 top-1.5 w-7 h-7 rounded-full bg-brand-500 border-4 border-white dark:border-slate-950 flex items-center justify-center text-white text-xs">
                            <i class="fa-solid fa-briefcase"></i>
                        </div>
                        <div class="absolute left-[-160px] top-1.5 hidden sm:block text-right w-28 text-sm font-semibold text-slate-400">
                            2021.01 ~ 2022.02
                        </div>
                        <div class="p-6 rounded-2xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 shadow-sm">
                            <span class="sm:hidden text-xs font-semibold text-brand-500 mb-1 block">2021.01 ~ 2022.02</span>
                            <h3 class="text-xl font-bold">주니어 웹 개발자</h3>
                            <div class="text-brand-600 dark:text-brand-400 font-medium text-sm mb-3">웹크리에이터스</div>
                            <p class="text-sm text-slate-600 dark:text-slate-400 leading-relaxed">
                                반응형 기업 홈페이지 제작 및 관리, RESTful API 연동 기능 구현 및 크로스 브라우징 이슈 대응 업무를 담당했습니다.
                            </p>
                        </div>
                    </div>

                    <!-- 학력 -->
                    <div class="relative pl-8 sm:pl-10">
                        <div class="absolute -left-3.5 top-1.5 w-7 h-7 rounded-full bg-slate-400 border-4 border-white dark:border-slate-950 flex items-center justify-center text-white text-xs">
                            <i class="fa-solid fa-graduation-cap"></i>
                        </div>
                        <div class="absolute left-[-160px] top-1.5 hidden sm:block text-right w-28 text-sm font-semibold text-slate-400">
                            2017.03 ~ 2021.02
                        </div>
                        <div class="p-6 rounded-2xl bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 shadow-sm">
                            <span class="sm:hidden text-xs font-semibold text-slate-400 mb-1 block">2017.03 ~ 2021.02</span>
                            <h3 class="text-xl font-bold">컴퓨터공학과 학사 졸업</h3>
                            <div class="text-brand-600 dark:text-brand-400 font-medium text-sm mb-3">한국대학교</div>
                            <p class="text-sm text-slate-600 dark:text-slate-400 leading-relaxed">
                                자료구조, 알고리즘, 데이터베이스 등 컴퓨터공학 기초 이론을 탄탄히 다지고 팀 프로젝트 역량을 함양했습니다.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact & 소셜 링크 섹션 -->
        <section id="contact" class="py-24 bg-white dark:bg-slate-900/50 border-t border-slate-200 dark:border-slate-800">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center mb-16">
                    <h2 class="text-3xl font-bold tracking-tight mb-4">Get In Touch</h2>
                    <p class="text-slate-600 dark:text-slate-400">협업 제안이나 문의사항이 있으시면 아래 폼을 통해 연락주세요.</p>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
                    <!-- 연락처 정보 및 소셜 -->
                    <div class="lg:col-span-5 space-y-6">
                        <div class="p-6 rounded-2xl bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700/50 space-y-6">
                            <div class="flex items-center space-x-4">
                                <div class="w-10 h-10 rounded-xl bg-brand-50 dark:bg-brand-950 flex items-center justify-center text-brand-500">
                                    <i class="fa-solid fa-envelope"></i>
                                </div>
                                <div>
                                    <div class="text-xs text-slate-500">이메일</div>
                                    <div class="text-sm font-semibold">dev.kim@example.com</div>
                                </div>
                            </div>
                            <div class="flex items-center space-x-4">
                                <div class="w-10 h-10 rounded-xl bg-brand-50 dark:bg-brand-950 flex items-center justify-center text-brand-500">
                                    <i class="fa-solid fa-location-dot"></i>
                                </div>
                                <div>
                                    <div class="text-xs text-slate-500">위치</div>
                                    <div class="text-sm font-semibold">서울시 강남구</div>
                                </div>
                            </div>
                        </div>

                        <!-- 소셜 링크 아이콘 -->
                        <div class="flex items-center justify-center space-x-4 pt-2">
                            <a href="https://github.com" target="_blank" rel="noopener noreferrer" aria-label="GitHub" class="w-12 h-12 rounded-xl bg-slate-100 dark:bg-slate-800 hover:bg-brand-600 hover:text-white dark:hover:bg-brand-600 flex items-center justify-center text-lg transition-all shadow-sm">
                                <i class="fa-brands fa-github"></i>
                            </a>
                            <a href="https://linkedin.com" target="_blank" rel="noopener noreferrer" aria-label="LinkedIn" class="w-12 h-12 rounded-xl bg-slate-100 dark:bg-slate-800 hover:bg-brand-600 hover:text-white dark:hover:bg-brand-600 flex items-center justify-center text-lg transition-all shadow-sm">
                                <i class="fa-brands fa-linkedin-in"></i>
                            </a>
                            <a href="https://velog.io" target="_blank" rel="noopener noreferrer" aria-label="Blog" class="w-12 h-12 rounded-xl bg-slate-100 dark:bg-slate-800 hover:bg-brand-600 hover:text-white dark:hover:bg-brand-600 flex items-center justify-center text-lg transition-all shadow-sm">
                                <i class="fa-solid fa-blog"></i>
                            </a>
                        </div>
                    </div>

                    <!-- 이메일 폼 -->
                    <div class="lg:col-span-7">
                        <form id="contact-form" class="space-y-4">
                            <div>
                                <label for="name" class="block text-xs font-semibold uppercase tracking-wider mb-2 text-slate-500">이름</label>
                                <input type="text" id="name" required class="w-full px-4 py-3 rounded-xl bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 focus:outline-none focus:ring-2 focus:ring-brand-500 text-sm" placeholder="홍길동" />
                            </div>
                            <div>
                                <label for="email" class="block text-xs font-semibold uppercase tracking-wider mb-2 text-slate-500">이메일</label>
                                <input type="email" id="email" required class="w-full px-4 py-3 rounded-xl bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 focus:outline-none focus:ring-2 focus:ring-brand-500 text-sm" placeholder="example@domain.com" />
                            </div>
                            <div>
                                <label for="message" class="block text-xs font-semibold uppercase tracking-wider mb-2 text-slate-500">메시지 내용</label>
                                <textarea id="message" rows="4" required class="w-full px-4 py-3 rounded-xl bg-slate-50 dark:bg-slate-800 border border-slate-200 dark:border-slate-700 focus:outline-none focus:ring-2 focus:ring-brand-500 text-sm resize-none" placeholder="프로젝트 협업 및 문의 내용을 남겨주세요..."></textarea>
                            </div>
                            <button type="submit" class="w-full py-4 rounded-xl bg-brand-600 hover:bg-brand-700 text-white font-medium shadow-lg shadow-brand-500/25 transition-all">
                                메시지 전송하기
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- 푸터 -->
    <footer class="py-8 bg-white dark:bg-slate-900 border-t border-slate-200 dark:border-slate-800 text-center text-xs text-slate-500">
        <div class="max-w-7xl mx-auto px-4">
            &copy; 2026 Dev.Kim. All rights reserved.
        </div>
    </footer>

    <!-- 커스텀 알림 모달 컴포넌트 -->
    <div id="custom-modal" class="fixed inset-0 z-50 hidden items-center justify-center bg-slate-900/60 backdrop-blur-sm">
        <div class="bg-white dark:bg-slate-900 border border-slate-200 dark:border-slate-800 rounded-2xl p-6 max-w-sm w-full mx-4 shadow-2xl text-center">
            <div id="modal-icon" class="w-12 h-12 rounded-full bg-emerald-100 dark:bg-emerald-950 text-emerald-500 flex items-center justify-center mx-auto mb-4 text-xl">
                <i class="fa-solid fa-check"></i>
            </div>
            <h3 id="modal-title" class="text-lg font-bold mb-2">전송 완료</h3>
            <p id="modal-message" class="text-sm text-slate-600 dark:text-slate-400 mb-6">메시지가 성공적으로 전송되었습니다. 빠른 시일 내에 회신드리겠습니다.</p>
            <button id="modal-close" class="w-full py-2.5 rounded-xl bg-brand-600 hover:bg-brand-700 text-white font-medium text-sm transition-all">
                확인
            </button>
        </div>
    </div>

    <!-- 스크립트 로직 -->
    <script>
        // 1. 다크 모드 토글 로직
        const themeToggleBtn = document.getElementById('theme-toggle');
        const themeIcon = document.getElementById('theme-icon');
        const htmlElement = document.documentElement;

        // 초기 시스템 선호도 및 로컬 스토리지 확인
        if (localStorage.theme === 'dark' || (!('theme' in localStorage) && window.matchMedia('(prefers-color-scheme: dark)').matches)) {
            htmlElement.classList.add('dark');
            themeIcon.className = 'fa-solid fa-sun text-lg';
        } else {
            htmlElement.classList.remove('dark');
            themeIcon.className = 'fa-solid fa-moon text-lg';
        }

        themeToggleBtn.addEventListener('click', () => {
            if (htmlElement.classList.contains('dark')) {
                htmlElement.classList.remove('dark');
                localStorage.theme = 'light';
                themeIcon.className = 'fa-solid fa-moon text-lg';
            } else {
                htmlElement.classList.add('dark');
                localStorage.theme = 'dark';
                themeIcon.className = 'fa-solid fa-sun text-lg';
            }
        });

        // 2. 모바일 메뉴 토글 로직
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // 모바일 메뉴 내 링크 클릭 시 자동 닫힘
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });

        // 3. 프로젝트 필터링 로직
        const filterButtons = document.querySelectorAll('.project-filter');
        const projectCards = document.querySelectorAll('.project-card');

        filterButtons.forEach(btn => {
            btn.addEventListener('click', () => {
                // 활성 버튼 스타일 변경
                filterButtons.forEach(b => {
                    b.classList.remove('bg-brand-600', 'text-white', 'shadow-sm');
                    b.classList.add('bg-slate-100', 'dark:bg-slate-800', 'text-slate-600', 'dark:text-slate-300');
                });
                btn.classList.remove('bg-slate-100', 'dark:bg-slate-800', 'text-slate-600', 'dark:text-slate-300');
                btn.classList.add('bg-brand-600', 'text-white', 'shadow-sm');

                const filterValue = btn.getAttribute('data-filter');

                projectCards.forEach(card => {
                    if (filterValue === 'all' || card.getAttribute('data-category') === filterValue) {
                        card.style.display = 'flex';
                    } else {
                        card.style.display = 'none';
                    }
                });
            });
        });

        // 4. 모달 메시지 제어 함수 (alert 대신 사용)
        const customModal = document.getElementById('custom-modal');
        const modalCloseBtn = document.getElementById('modal-close');

        function showModal(title, message) {
            document.getElementById('modal-title').innerText = title;
            document.getElementById('modal-message').innerText = message;
            customModal.classList.remove('hidden');
            customModal.classList.add('flex');
        }

        modalCloseBtn.addEventListener('click', () => {
            customModal.classList.add('hidden');
            customModal.classList.remove('flex');
        });

        // 5. 연락처 폼 제출 인터랙션
        const contactForm = document.getElementById('contact-form');
        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            // 폼 입력 초기화
            contactForm.reset();
            showModal('전송 완료', '메시지가 성공적으로 전송되었습니다. 빠른 시일 내에 회신드리겠습니다.');
        });
    </script>
</body>
</html>
