<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Analysis of Leadership Examples - Xiaomi's Dismissal of Wang Teng</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        // Tailwind配置
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#165DFF',
                        secondary: '#E8F3FF',
                        neutral: '#F5F7FA',
                        dark: '#333333',
                        medium: '#666666',
                        light: '#999999',
                        warning: '#F53F3F'
                    },
                    fontFamily: {
                        sans: ['Inter', 'system-ui', 'sans-serif'],
                    },
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .text-balance {
                text-wrap: balance;
            }
            .scrollbar-hide::-webkit-scrollbar {
                display: none;
            }
            .scrollbar-hide {
                -ms-overflow-style: none;
                scrollbar-width: none;
            }
            .section-fade {
                opacity: 0;
                transform: translateY(20px);
                transition: opacity 0.6s ease-out, transform 0.6s ease-out;
            }
            .section-fade.active {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
    <style>
        /* 导入Inter字体 */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        /* 基础样式 */
        html {
            scroll-behavior: smooth;
        }
        
        body {
            font-family: 'Inter', system-ui, sans-serif;
            color: #333333;
            background-color: #ffffff;
        }
        
        /* 导航栏滚动效果 */
        .nav-scrolled {
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }
        
        /* 引用样式 */
        blockquote {
            position: relative;
            padding-left: 1.5rem;
            border-left: 4px solid #165DFF;
            font-style: italic;
            color: #666666;
        }
        
        /* 代码块样式 */
        .code-block {
            background-color: #F5F7FA;
            border-radius: 0.375rem;
            padding: 1rem;
            font-family: 'Courier New', Courier, monospace;
            font-size: 0.9rem;
            overflow-x: auto;
        }
        
        /* 目录项激活状态 */
        .toc-item.active {
            color: #165DFF;
            font-weight: 600;
            border-left: 3px solid #165DFF;
        }
    </style>
</head>
<body class="antialiased">
    <!-- 顶部导航栏 -->
    <header id="main-header" class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 bg-white">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-4">
                <h1 class="text-xl sm:text-2xl font-bold text-primary">
                    <i class="fa fa-line-chart mr-2"></i>Leadership Analysis
                </h1>
                
                <!-- 桌面端导航 -->
                <nav class="hidden md:flex space-x-8">
                    <a href="#introduction" class="text-medium hover:text-primary transition-colors duration-200">Introduction</a>
                    <a href="#the-paper" class="text-medium hover:text-primary transition-colors duration-200">The Paper</a>
                    <a href="#guangming" class="text-medium hover:text-primary transition-colors duration-200">Guangming Online</a>
                    <a href="#comparative" class="text-medium hover:text-primary transition-colors duration-200">Comparative Analysis</a>
                    <a href="#lessons" class="text-medium hover:text-primary transition-colors duration-200">Lessons</a>
                </nav>
                
                <!-- 移动端汉堡菜单 -->
                <button id="menu-toggle" class="md:hidden text-medium hover:text-primary transition-colors duration-200">
                    <i class="fa fa-bars text-xl"></i>
                </button>
            </div>
        </div>
        
        <!-- 移动端导航菜单 -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100">
            <div class="container mx-auto px-4 py-3 space-y-3">
                <a href="#introduction" class="block py-2 text-medium hover:text-primary transition-colors duration-200">Introduction</a>
                <a href="#the-paper" class="block py-2 text-medium hover:text-primary transition-colors duration-200">The Paper's Reports</a>
                <a href="#guangming" class="block py-2 text-medium hover:text-primary transition-colors duration-200">Guangming Online's Reports</a>
                <a href="#comparative" class="block py-2 text-medium hover:text-primary transition-colors duration-200">Comparative Analysis</a>
                <a href="#lessons" class="block py-2 text-medium hover:text-primary transition-colors duration-200">Leadership Lessons</a>
            </div>
        </div>
    </header>

    <!-- 主要内容区 -->
    <main class="container mx-auto px-4 sm:px-6 lg:px-8 pt-24 pb-16">
        <div class="flex flex-col lg:flex-row gap-8">
            <!-- 侧边目录 (桌面端) -->
            <aside class="hidden lg:block w-64 flex-shrink-0">
                <div class="sticky top-24 bg-neutral rounded-lg p-5 shadow-sm">
                    <h2 class="text-lg font-semibold mb-4 text-dark border-b pb-2">Table of Contents</h2>
                    <nav class="space-y-2 overflow-y-auto max-h-[calc(100vh-12rem)] scrollbar-hide">
                        <a href="#introduction" class="toc-item block pl-3 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent">
                            I. Introduction
                        </a>
                        <a href="#the-paper" class="toc-item block pl-3 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent">
                            II. The Paper's Reports
                        </a>
                        <a href="#the-paper-1" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            2.1 Strict Discipline Enforcement
                        </a>
                        <a href="#the-paper-2" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            2.2 Lei Jun's Leadership
                        </a>
                        <a href="#the-paper-3" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            2.3 Wang Teng's Leadership Failure
                        </a>
                        <a href="#the-paper-4" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            2.4 Follow-up Handling
                        </a>
                        <a href="#guangming" class="toc-item block pl-3 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent">
                            III. Guangming Online's Reports
                        </a>
                        <a href="#guangming-1" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            3.1 Legal Perspective
                        </a>
                        <a href="#guangming-2" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            3.2 Employee Obligations
                        </a>
                        <a href="#guangming-3" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            3.3 Legal Consequences
                        </a>
                        <a href="#comparative" class="toc-item block pl-3 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent">
                            IV. Comparative Analysis
                        </a>
                        <a href="#comparative-1" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            4.1 Different Perspectives
                        </a>
                        <a href="#comparative-2" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            4.2 Common Emphases
                        </a>
                        <a href="#comparative-3" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            4.3 Different Leadership Models
                        </a>
                        <a href="#lessons" class="toc-item block pl-3 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent">
                            V. Leadership Lessons
                        </a>
                        <a href="#lessons-1" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            5.1 Leadership Self-Discipline
                        </a>
                        <a href="#lessons-2" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            5.2 Confidentiality Management
                        </a>
                        <a href="#lessons-3" class="toc-item block pl-6 py-1.5 text-medium hover:text-primary transition-colors duration-200 border-l-3 border-transparent text-sm">
                            5.3 Balance Between Trust and Supervision
                        </a>
                    </nav>
                </div>
            </aside>

            <!-- 主要内容 -->
            <article class="flex-1 max-w-3xl">
                <!-- 标题区 -->
                <div class="mb-12 text-center section-fade">
                    <h1 class="text-3xl sm:text-4xl font-bold text-dark mb-6 leading-tight text-balance">
                        Analysis of Leadership Examples Shown in News Reports on Xiaomi's Dismissal of Wang Teng
                    </h1>
                    <div class="flex items-center justify-center text-light text-sm space-x-4">
                        <span><i class="fa fa-calendar-o mr-1"></i> September 13, 2025</span>
                        <span><i class="fa fa-clock-o mr-1"></i> 25 min read</span>
                        <span><i class="fa fa-tag mr-1"></i> Leadership Analysis</span>
                    </div>
                </div>

                <!-- 第一部分：引言 -->
                <section id="introduction" class="mb-12 section-fade">
                    <div class="bg-white rounded-xl p-6 sm:p-8 shadow-sm border border-gray-100">
                        <h2 class="text-2xl font-bold text-dark mb-6 flex items-center">
                            <span class="inline-flex items-center justify-center w-8 h-8 rounded-full bg-primary text-white mr-3 text-sm">I</span>
                            Introduction: Leadership Manifestations in Corporate Crisis Events
                        </h2>
                        <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                            <p class="mb-4">
                                The dismissal of Wang Teng, the former General Manager of Xiaomi's China Region Marketing Department and REDMI brand, due to disciplinary violations has attracted widespread attention. This incident not only involves corporate internal management but also prominently demonstrates different leadership styles and behaviors from various perspectives.
                            </p>
                            <p class="mb-4">
                                Leadership is not merely about position or authority; it is more about the ability to influence others through one's own behavior, decision-making, and values. In this case, the reactions and handling methods of Xiaomi Group, its founder Lei Jun, and Wang Teng himself all show different forms of leadership examples, whether positive or negative.
                            </p>
                            <blockquote class="my-6">
                                This article will analyze in detail how two authoritative news sources - The Paper and Guangming Online - present these leadership examples, exploring how different leadership styles influence organizational culture and individual career development.
                            </blockquote>
                            <p>
                                Through this analysis, we can better understand the importance of leadership in corporate governance and the profound impact it has on organizational and individual development.
                            </p>
                        </div>
                    </div>
                </section>

                <!-- 第二部分：澎湃新闻报道中的领导力案例 -->
                <section id="the-paper" class="mb-12 section-fade">
                    <div class="bg-white rounded-xl p-6 sm:p-8 shadow-sm border border-gray-100">
                        <h2 class="text-2xl font-bold text-dark mb-6 flex items-center">
                            <span class="inline-flex items-center justify-center w-8 h-8 rounded-full bg-primary text-white mr-3 text-sm">II</span>
                            Leadership Examples Demonstrated in The Paper's Reports
                        </h2>
                        
                        <!-- 2.1 严格执行纪律 -->
                        <div id="the-paper-1" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">2.1</span>
                                Strict Discipline Enforcement: Xiaomi's Zero-Tolerance Policy Leadership Style
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    The Paper's reports show that Xiaomi Group demonstrated a strict, rule-based leadership style in handling Wang Teng's disciplinary violations. According to internal company emails disclosed in the reports, Xiaomi adheres to a "zero-tolerance, full coverage, no exceptions" attitude toward disciplinary violations, and made this disciplinary decision in accordance with relevant regulations such as the "Xiaomi Group Employee Violations and Disciplinary Measures".
                                </p>
                                <div class="bg-secondary rounded-lg p-4 my-5 border-l-4 border-primary">
                                    <p class="text-primary font-medium">
                                        This clear position and decisive action reflect Xiaomi's top management team's emphasis on corporate culture and values, demonstrating a leadership style that prioritizes organizational discipline and standardized management.
                                    </p>
                                </div>
                                <p class="mb-4">
                                    This leadership style is not only reflected in words but more importantly in practical actions. The Paper's reports mention that Xiaomi's Professional Ethics Committee clearly stated in its internal email that Wang Teng was dismissed due to "leaking company-confidential information" and "conflict of interest".
                                </p>
                                <p>
                                    This strict, zero-tolerance leadership style helps maintain the seriousness of corporate rules and regulations, ensuring that employees at all levels understand that there are clear boundaries that cannot be crossed. It also demonstrates the company's determination to protect core business secrets, which is crucial for technology companies like Xiaomi in an increasingly competitive market environment.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 2.2 雷军的领导力 -->
                        <div id="the-paper-2" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">2.2</span>
                                Lei Jun's Leadership: Combining Reminders with Trust
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    The Paper's reports also show Lei Jun, Xiaomi's founder and chairman, demonstrating a unique leadership style. Although Lei Jun publicly reminded Wang Teng to pay attention to confidentiality discipline on multiple occasions, he also expressed trust and support for Wang Teng.
                                </p>
                                <blockquote class="my-6">
                                    For example, in a live broadcast in August 2024, Lei Jun mentioned humorously: "Except for our General Teng (Wang Teng) who often leaks secrets and gets fined, my reputation is pretty good".
                                </blockquote>
                                <p class="mb-4">
                                    This combination of reminders and trust reflects Lei Jun's leadership approach of both emphasizing discipline and encouraging growth.
                                </p>
                                <p class="mb-4">
                                    Lei Jun's leadership style is further demonstrated in Wang Teng's career development within Xiaomi. Wang Teng joined Xiaomi in 2016 and quickly rose from a product manager to the General Manager of the China Region Marketing Department and REDMI brand, reaching level 21, just one step away from top management.
                                </p>
                                <p>
                                    However, when Wang Teng violated company regulations, Lei Jun did not show favoritism. Xiaomi made a fair and just decision to dismiss Wang Teng in accordance with regulations, demonstrating Lei Jun's leadership principles of "principles above personal relationships". This balanced approach helps maintain the authority of organizational rules while encouraging employees to develop their capabilities, creating a healthy organizational culture.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 2.3 王腾的领导力失败 -->
                        <div id="the-paper-3" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">2.3</span>
                                Wang Teng's Leadership Failure: Repeated Boundary Violations
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    In contrast, Wang Teng's performance in this incident demonstrates negative examples of leadership. As a senior executive, Wang Teng should have set an example by abiding by company regulations, but he had a history of confidentiality violations.
                                </p>
                                <div class="bg-neutral rounded-lg p-5 my-5">
                                    <h4 class="font-medium text-dark mb-2">Wang Teng's Previous Violation (April 2022):</h4>
                                    <ul class="list-disc list-inside space-y-1 text-medium">
                                        <li>Prematurely disclosed the release time of the Redmi K50 standard version on Weibo</li>
                                        <li>Identified as a second-level leak incident by Xiaomi</li>
                                        <li>Received an internal warning</li>
                                        <li>Disqualified from promotion that year</li>
                                        <li>5,000 yuan deducted from performance bonus</li>
                                        <li>10 points deducted from quarterly assessment</li>
                                    </ul>
                                </div>
                                <p class="mb-4">
                                    Wang Teng's repeated violations of confidentiality regulations reflect his insufficient understanding of leadership responsibilities and the importance of organizational discipline. As a leader, he should not only understand the importance of company secrets but also set an example by abiding by relevant regulations.
                                </p>
                                <p>
                                    The Paper's reports show that Wang Teng may have initially brought some popularity to Xiaomi products through his "leaking" behavior, playing a role in product promotion. However, this approach over-relied on traffic logic, resulting in blurred information disclosure boundaries and potential risks to the company.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 2.4 后续处理 -->
                        <div id="the-paper-4">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">2.4</span>
                                Follow-up Handling: Demonstrating Leadership's Decisiveness and Accountability
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    The Paper's reports also show Xiaomi's follow-up handling of this incident, demonstrating the leadership style of decisiveness and accountability. After Wang Teng's dismissal, his Weibo certification was quickly canceled, and his Kuaishou account was banned, showing the company's determination to implement disciplinary decisions.
                                </p>
                                <p class="mb-4">
                                    This decisive action sends a clear message to the entire organization that violations of company regulations will inevitably be punished, maintaining the seriousness of the rules.
                                </p>
                                <p>
                                    Additionally, Xiaomi's internal email called on cadres in the China region to take this as a warning, maintain a sense of awe, and adhere to the red line of company systems. This kind of educational guidance reflects the company's emphasis on preventive education, not just relying on punitive measures but also focusing on cultivating employees' awareness of compliance.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- 第三部分：光明网报道中的领导力案例 -->
                <section id="guangming" class="mb-12 section-fade">
                    <div class="bg-white rounded-xl p-6 sm:p-8 shadow-sm border border-gray-100">
                        <h2 class="text-2xl font-bold text-dark mb-6 flex items-center">
                            <span class="inline-flex items-center justify-center w-8 h-8 rounded-full bg-primary text-white mr-3 text-sm">III</span>
                            Leadership Examples Demonstrated in Guangming Online's Reports
                        </h2>
                        
                        <!-- 3.1 法律视角 -->
                        <div id="guangming-1" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">3.1</span>
                                Legal Perspective: Demonstrating Leadership's Risk Prevention Awareness
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    Guangming Online's reports analyze Wang Teng's case from a legal perspective, demonstrating the importance of risk prevention awareness in leadership. The report cites Li Bo, a member of the "Legal Daily" lawyer expert database and Director of the Environmental Energy and Resources Law Research Center at Beijing Jingdu Law Firm, explaining the legal definition of "company-confidential information".
                                </p>
                                <div class="bg-secondary rounded-lg p-4 my-5 border-l-4 border-primary">
                                    <p class="text-primary font-medium">
                                        According to legal expert Li Bo, commercial secrets include technical information, business information, and other business information, and their identification requires meeting three legal standards: "not being generally known to the public," having "commercial value," and the company taking necessary "confidentiality measures".
                                    </p>
                                </div>
                                <p>
                                    For business leaders, understanding the legal boundaries of commercial secrets and ensuring the company's confidentiality measures meet legal requirements is an important part of risk management. This legal perspective helps leaders establish more comprehensive and effective confidentiality systems, rather than just staying on the surface, demonstrating the leadership style of combining legal compliance with practical operations.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 3.2 员工义务 -->
                        <div id="guangming-2" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">3.2</span>
                                Employee Obligations: Demonstrating Leadership's Educational Guidance Function
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    Guangming Online's reports discuss from the perspective of employee obligations, demonstrating the educational guidance function in leadership. The report points out that employees' confidentiality obligations are divided into two types: legal confidentiality obligations and contractual confidentiality obligations.
                                </p>
                                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 my-5">
                                    <div class="bg-neutral rounded-lg p-4">
                                        <h4 class="font-medium text-dark mb-2">Legal Confidentiality Obligations</h4>
                                        <p class="text-medium text-sm">Come from legal provisions and apply to all employees regardless of specific agreements.</p>
                                    </div>
                                    <div class="bg-neutral rounded-lg p-4">
                                        <h4 class="font-medium text-dark mb-2">Contractual Confidentiality Obligations</h4>
                                        <p class="text-medium text-sm">Come from confidentiality agreements, labor contract clauses, and company rules.</p>
                                    </div>
                                </div>
                                <p>
                                    This analysis of employee obligations reflects the importance of leadership in educating and guiding subordinates. Effective leadership not only requires establishing clear rules but also ensuring employees truly understand these obligations and the consequences of violating them.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 3.3 法律后果 -->
                        <div id="guangming-3">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">3.3</span>
                                Legal Consequences: Demonstrating Leadership's Sense of Responsibility and Deterrence
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    Guangming Online's reports also analyze the legal consequences of different levels of disclosure behaviors, demonstrating the sense of responsibility and deterrence in leadership. The report points out that the legal responsibilities for employees' violation of confidentiality obligations are usually divided into two types: civil legal responsibility and criminal legal responsibility.
                                </p>
                                <blockquote class="my-6">
                                    The report also points out that to determine that an employee constitutes the crime of infringing on commercial secrets, three conditions need to be met: the disclosed "company-confidential information" can be identified as a trade secret in the legal sense; the employee implemented the act of infringing on commercial secrets; and the consequences are serious.
                                </blockquote>
                                <p>
                                    This legal threshold reminds leaders to handle disclosure incidents carefully, balancing between protecting company interests and respecting employee rights, demonstrating the leadership style of handling problems with both firmness and flexibility.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- 第四部分：比较分析 -->
                <section id="comparative" class="mb-12 section-fade">
                    <div class="bg-white rounded-xl p-6 sm:p-8 shadow-sm border border-gray-100">
                        <h2 class="text-2xl font-bold text-dark mb-6 flex items-center">
                            <span class="inline-flex items-center justify-center w-8 h-8 rounded-full bg-primary text-white mr-3 text-sm">IV</span>
                            Comparative Analysis of Leadership Styles in Two News Sources
                        </h2>
                        
                        <!-- 4.1 不同视角 -->
                        <div id="comparative-1" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">4.1</span>
                                Different Perspectives: Management Practice vs. Legal Compliance
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    The reports from The Paper and Guangming Online demonstrate different leadership perspectives: The Paper focuses more on management practices, while Guangming Online emphasizes legal compliance. This difference in perspective reflects the multifaceted nature of leadership, which needs to simultaneously consider both internal management needs and external legal compliance requirements.
                                </p>
                                <div class="overflow-x-auto my-5">
                                    <table class="min-w-full bg-neutral rounded-lg overflow-hidden">
                                        <thead class="bg-primary text-white">
                                            <tr>
                                                <th class="py-3 px-4 text-left">News Source</th>
                                                <th class="py-3 px-4 text-left">Perspective</th>
                                                <th class="py-3 px-4 text-left">Key Focus</th>
                                            </tr>
                                        </thead>
                                        <tbody class="divide-y divide-gray-200">
                                            <tr class="bg-white">
                                                <td class="py-3 px-4 font-medium">The Paper</td>
                                                <td class="py-3 px-4">Management Practice</td>
                                                <td class="py-3 px-4">Internal management, disciplinary enforcement, educational guidance</td>
                                            </tr>
                                            <tr class="bg-white">
                                                <td class="py-3 px-4 font-medium">Guangming Online</td>
                                                <td class="py-3 px-4">Legal Compliance</td>
                                                <td class="py-3 px-4">Risk prevention, legal obligations, legal consequences</td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>
                                <p>
                                    This difference in perspective reminds leaders that effective leadership must consider both internal management needs and external legal requirements, achieving a balance between the two.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 4.2 共同强调 -->
                        <div id="comparative-2" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">4.2</span>
                                Common Emphases: Integrity and Compliance
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    Despite their different perspectives, the reports from both news sources emphasize the importance of integrity and compliance in leadership. The Paper's reports show Xiaomi's "zero-tolerance" attitude toward violations, emphasizing the seriousness of organizational discipline. Guangming Online's reports analyze the legal responsibilities of employees' confidentiality obligations, emphasizing the importance of compliance.
                                </p>
                                <div class="bg-secondary rounded-lg p-4 my-5 border-l-4 border-primary">
                                    <p class="text-primary font-medium">
                                        This common emphasis reflects the core values that leadership should possess in modern enterprises - integrity and compliance. In an increasingly competitive market environment, maintaining integrity and compliance is not only an ethical requirement but also a necessary condition for the sustainable development of enterprises.
                                    </p>
                                </div>
                                <p>
                                    The reports from both news sources show that whether through management practices or legal compliance, integrity and compliance are the cornerstones of effective leadership. Only by adhering to these values can leaders guide the organization through various challenges and maintain long-term stable development.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 4.3 不同领导模式 -->
                        <div id="comparative-3">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">4.3</span>
                                Different Leadership Models: Task-Oriented vs. People-Oriented
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    Further analysis shows that the two news sources also reflect different leadership models: The Paper's reports show Xiaomi's task-oriented leadership style, while Guangming Online's reports emphasize a people-oriented leadership approach.
                                </p>
                                <div class="grid grid-cols-1 md:grid-cols-2 gap-6 my-5">
                                    <div class="bg-neutral rounded-lg p-5">
                                        <h4 class="font-medium text-dark mb-3 flex items-center">
                                            <i class="fa fa-bullseye text-primary mr-2"></i>
                                            Task-Oriented Leadership
                                        </h4>
                                        <ul class="list-disc list-inside space-y-2 text-medium">
                                            <li>Emphasizes goal achievement</li>
                                            <li>Focuses on rule compliance</li>
                                            <li>Clear roles and responsibilities</li>
                                            <li>Strict supervision and assessment</li>
                                            <li>Suitable for maintaining efficiency</li>
                                        </ul>
                                    </div>
                                    <div class="bg-neutral rounded-lg p-5">
                                        <h4 class="font-medium text-dark mb-3 flex items-center">
                                            <i class="fa fa-users text-primary mr-2"></i>
                                            People-Oriented Leadership
                                        </h4>
                                        <ul class="list-disc list-inside space-y-2 text-medium">
                                            <li>Focuses on employee needs</li>
                                            <li>Emphasizes education and guidance</li>
                                            <li>Promotes self-discipline</li>
                                            <li>Cultivates responsibility and loyalty</li>
                                            <li>Suitable for sustainable culture</li>
                                        </ul>
                                    </div>
                                </div>
                                <p>
                                    In reality, effective leadership often needs to combine both models, balancing task requirements with people management. The reports from both news sources together present a more comprehensive leadership picture, showing how leaders can achieve organizational goals while promoting employee development through different methods.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- 第五部分：领导力教训与启示 -->
                <section id="lessons" class="mb-12 section-fade">
                    <div class="bg-white rounded-xl p-6 sm:p-8 shadow-sm border border-gray-100">
                        <h2 class="text-2xl font-bold text-dark mb-6 flex items-center">
                            <span class="inline-flex items-center justify-center w-8 h-8 rounded-full bg-primary text-white mr-3 text-sm">V</span>
                            Leadership Lessons and Enlightenments
                        </h2>
                        
                        <!-- 5.1 领导力自律 -->
                        <div id="lessons-1" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">5.1</span>
                                Leadership Self-Discipline: Setting an Example
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    The Wang Teng incident provides an important leadership lesson: leaders must set an example and strictly discipline themselves. As a leader, Wang Teng's repeated violations of confidentiality regulations set a bad example for subordinates, potentially undermining the overall compliance culture of the organization.
                                </p>
                                <blockquote class="my-6">
                                    Leaders must understand that they are not only managers but also role models. Their every move is watched by subordinates, and any violation of discipline may lead to a breakdown of the entire organizational discipline system.
                                </blockquote>
                                <p>
                                    Xiaomi's handling of this incident also demonstrates the importance of leadership self-discipline from the opposite side. When leaders discover problems with their subordinates, they must deal with them fairly and justly in accordance with regulations, without showing favoritism or hesitation. Only such an attitude can maintain the seriousness of organizational rules and ensure the effective operation of the entire management system.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 5.2 保密管理 -->
                        <div id="lessons-2" class="mb-8">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">5.2</span>
                                Confidentiality Management: Building a Culture of Compliance
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    This incident also highlights the importance of confidentiality management in leadership. In an era of intense market competition, company-confidential information is an important asset of the enterprise, and any disclosure may cause significant damage to the company's interests. Leaders must attach great importance to confidentiality management, establishing a sound confidentiality system and ensuring its effective implementation.
                                </p>
                                <div class="bg-neutral rounded-lg p-5 my-5">
                                    <h4 class="font-medium text-dark mb-3">Key Elements of Effective Confidentiality Management:</h4>
                                    <ol class="list-decimal list-inside space-y-2 text-medium">
                                        <li>Establish perfect confidentiality systems and regulations</li>
                                        <li>Conduct regular education and training for employees</li>
                                        <li>Help employees understand the importance of confidentiality</li>
                                        <li>Clarify the consequences of confidentiality violations</li>
                                        <li>Establish effective supervision and early warning mechanisms</li>
                                        <li>Discover and handle potential risks in a timely manner</li>
                                    </ol>
                                </div>
                                <p>
                                    Lei Jun's reminders to Wang Teng in the early stages demonstrate the importance of proactive management in leadership. Leaders should be good at discovering potential problems, promptly reminding subordinates to correct them, rather than waiting until problems become serious before taking action. This proactive leadership approach helps prevent problems before they occur, reducing potential losses to the company.
                                </p>
                            </div>
                        </div>
                        
                        <!-- 5.3 信任与监督的平衡 -->
                        <div id="lessons-3">
                            <h3 class="text-xl font-semibold text-dark mb-4 flex items-center">
                                <span class="inline-flex items-center justify-center w-7 h-7 rounded-full bg-secondary text-primary mr-2 text-sm">5.3</span>
                                Balance Between Trust and Supervision: The Art of Leadership
                            </h3>
                            <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                                <p class="mb-4">
                                    The Wang Teng incident also reflects the balance between trust and supervision in leadership. Xiaomi's rapid promotion of Wang Teng demonstrates the company's trust in his abilities. However, this trust should not mean relaxing supervision. Wang Teng's repeated violations of regulations suggest that there may be loopholes in the company's supervision mechanism.
                                </p>
                                <div class="bg-secondary rounded-lg p-4 my-5 border-l-4 border-primary">
                                    <p class="text-primary font-medium">
                                        This reminds leaders that trust and supervision are not mutually exclusive but complementary. While trusting subordinates' abilities, leaders should also establish appropriate supervision mechanisms to ensure that work proceeds within the correct scope.
                                    </p>
                                </div>
                                <p>
                                    Excessive trust may lead to indulgence, while excessive supervision may stifle employees' initiative. The art of leadership lies in finding the right balance between the two, creating an environment where employees feel trusted while understanding that there are clear boundaries and expectations. This balance is crucial for fostering both employee development and organizational integrity.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- 结论 -->
                <section class="mb-8 section-fade">
                    <div class="bg-primary/5 rounded-xl p-6 sm:p-8 shadow-sm border border-primary/10">
                        <h2 class="text-2xl font-bold text-primary mb-6">Conclusion</h2>
                        <div class="prose prose-lg max-w-none text-medium leading-relaxed">
                            <p class="mb-4">
                                The analysis of Xiaomi's dismissal of Wang Teng through the reports of The Paper and Guangming Online reveals multiple dimensions of leadership in corporate crisis management. From Xiaomi's strict disciplinary enforcement to Lei Jun's balanced approach of reminders and trust, and from the legal perspective of confidentiality management to the educational guidance of employee obligations, these examples collectively present a comprehensive picture of modern corporate leadership.
                            </p>
                            <p>
                                The key lessons from this incident emphasize that effective leadership requires self-discipline, sound confidentiality management, and a balance between trust and supervision. In today's complex business environment, leaders must integrate both management practices and legal compliance, combining task-oriented and people-oriented approaches to build a culture of integrity and compliance. By doing so, leaders can not only navigate corporate crises effectively but also foster sustainable organizational development and employee growth.
                            </p>
                        </div>
                    </div>
                </section>
            </article>
        </div>
    </main>

    <!-- 页脚 -->
    <footer class="bg-dark text-white py-8">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <h3 class="text-xl font-bold mb-2">Leadership Analysis Report</h3>
                    <p class="text-light text-sm">Analysis of Leadership Examples in Xiaomi's Dismissal of Wang Teng</p>
                </div>
                <div class="flex space-x-4">
                    <a href="#" class="text-light hover:text-white transition-colors duration-200">
                        <i class="fa fa-file-text-o text-xl"></i>
                    </a>
                    <a href="#" class="text-light hover:text-white transition-colors duration-200">
                        <i class="fa fa-share-alt text-xl"></i>
                    </a>
                    <a href="#" class="text-light hover:text-white transition-colors duration-200">
                        <i class="fa fa-download text-xl"></i>
                    </a>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-6 pt-6 text-center text-light text-sm">
                <p>© 2025 Leadership Analysis Research. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <!-- 回到顶部按钮 -->
    <button id="back-to-top" class="fixed bottom-6 right-6 bg-primary text-white w-12 h-12 rounded-full flex items-center justify-center shadow-lg opacity-0 invisible transition-all duration-300 hover:bg-primary/90">
        <i class="fa fa-arrow-up"></i>
    </button>

    <!-- JavaScript -->
    <script>
        // 移动端菜单切换
        const menuToggle = document.getElementById('menu-toggle');
        const mobileMenu = document.getElementById('mobile-menu');
        
        menuToggle.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            const icon = menuToggle.querySelector('i');
            if (mobileMenu.classList.contains('hidden')) {
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars');
            } else {
                icon.classList.remove('fa-bars');
                icon.classList.add('fa-times');
            }
        });
        
        // 导航栏滚动效果
        const header = document.getElementById('main-header');
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                header.classList.add('nav-scrolled');
            } else {
                header.classList.remove('nav-scrolled');
            }
        });
        
        // 回到顶部按钮
        const backToTopButton = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', () => {
            if (window.scrollY > 300) {
                backToTopButton.classList.remove('opacity-0', 'invisible');
                backToTopButton.classList.add('opacity-100', 'visible');
            } else {
                backToTopButton.classList.add('opacity-0', 'invisible');
                backToTopButton.classList.remove('opacity-100', 'visible');
            }
        });
        
        backToTopButton.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // 目录项激活状态
        const sections = document.querySelectorAll('section[id]');
        const tocItems = document.querySelectorAll('.toc-item');
        
        function highlightTocItem() {
            let scrollPosition = window.scrollY + 100;
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop - 100;
                const sectionBottom = sectionTop + section.offsetHeight;
                const sectionId = section.getAttribute('id');
                
                if (scrollPosition >= sectionTop && scrollPosition < sectionBottom) {
                    tocItems.forEach(item => {
                        item.classList.remove('active');
                        if (item.getAttribute('href') === `#${sectionId}`) {
                            item.classList.add('active');
                            
                            // 高亮父级目录项（如果有）
                            const parentItem = item.closest('.toc-item')?.parentNode?.previousElementSibling;
                            if (parentItem && parentItem.classList.contains('toc-item')) {
                                parentItem.classList.add('active');
                            }
                        }
                    });
                }
            });
        }
        
        // 页面加载时和滚动时更新目录激活状态
        window.addEventListener('load', highlightTocItem);
        window.addEventListener('scroll', highlightTocItem);
        
        // 滚动动画
        function fadeInSections() {
            const fadeElements = document.querySelectorAll('.section-fade');
            
            fadeElements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('active');
                }
            });
        }
        
        // 页面加载时和滚动时触发动画
        window.addEventListener('load', fadeInSections);
        window.addEventListener('scroll', fadeInSections);
        
        // 移动端菜单点击后关闭
        const mobileMenuLinks = mobileMenu.querySelectorAll('a');
        mobileMenuLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                const icon = menuToggle.querySelector('i');
                icon.classList.remove('fa-times');
                icon.classList.add('fa-bars');
            });
        });
    </script>
</body>
</html>
