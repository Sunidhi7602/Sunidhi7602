<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sunidhi J - Full Stack Developer & Cybersecurity Enthusiast</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;700&family=Poppins:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #f0f4e8 0%, #e8f0e0 50%, #d4e4c8 100%);
            color: #2d4a2d;
            line-height: 1.6;
            padding: 20px;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 30px;
            box-shadow: 0 20px 60px rgba(45, 74, 45, 0.15);
            padding: 40px;
            position: relative;
            overflow: hidden;
        }
        
        .container::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: linear-gradient(90deg, #4a7c59, #6b8e23, #8fbc8f, #90ee90);
        }
        
        .header-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin-bottom: 30px;
            justify-content: center;
        }
        
        .badge {
            padding: 8px 16px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 500;
            font-size: 14px;
            transition: all 0.3s ease;
            border: 2px solid transparent;
            background: linear-gradient(45deg, #f5f1df, #e9c785);
            color: #5d4037;
            box-shadow: 0 4px 15px rgba(233, 199, 133, 0.3);
        }
        
        .badge:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(233, 199, 133, 0.4);
            background: linear-gradient(45deg, #e9c785, #f5f1df);
        }
        
        .whoami-box {
            background: linear-gradient(135deg, #e8f5e8 0%, #f0f8f0 100%);
            border: 2px solid #a8d5a8;
            border-radius: 25px;
            padding: 40px;
            margin-bottom: 40px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .whoami-box::before {
            content: '🌿';
            position: absolute;
            top: 20px;
            right: 30px;
            font-size: 48px;
            opacity: 0.3;
        }
        
        .whoami-title {
            font-family: 'Dancing Script', cursive;
            font-size: 3rem;
            color: #2d4a2d;
            margin-bottom: 20px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.1);
        }
        
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        
        .info-item {
            background: rgba(168, 213, 168, 0.3);
            padding: 15px 25px;
            border-radius: 15px;
            border-left: 4px solid #4a7c59;
        }
        
        .info-label {
            font-weight: 600;
            color: #4a7c59;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        
        .info-value {
            font-size: 1.1rem;
            color: #2d4a2d;
            margin-top: 5px;
        }
        
        .section {
            margin-bottom: 50px;
        }
        
        .section-title {
            font-family: 'Dancing Script', cursive;
            font-size: 2.5rem;
            color: #4a7c59;
            text-align: center;
            margin-bottom: 30px;
            position: relative;
        }
        
        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 3px;
            background: linear-gradient(90deg, #6b8e23, #90ee90);
            margin: 10px auto;
            border-radius: 2px;
        }
        
        .stack-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .stack-category {
            background: linear-gradient(135deg, rgba(232, 245, 232, 0.8), rgba(240, 248, 240, 0.8));
            padding: 25px;
            border-radius: 20px;
            border: 1px solid rgba(168, 213, 168, 0.5);
        }
        
        .stack-title {
            font-weight: 600;
            color: #2d4a2d;
            margin-bottom: 20px;
            font-size: 1.3rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .tech-badges {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .tech-badge {
            padding: 6px 12px;
            background: linear-gradient(45deg, #a8d5a8, #90ee90);
            color: #2d4a2d;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 500;
            border: 1px solid rgba(74, 124, 89, 0.3);
            transition: all 0.3s ease;
        }
        
        .tech-badge:hover {
            transform: scale(1.05);
            box-shadow: 0 5px 15px rgba(144, 238, 144, 0.4);
        }
        
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 25px;
        }
        
        .project-card {
            background: linear-gradient(135deg, #ffffff 0%, #f8fbf8 100%);
            border: 2px solid #d4e4c8;
            border-radius: 20px;
            padding: 30px;
            transition: all 0.4s ease;
            position: relative;
            overflow: hidden;
        }
        
        .project-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #4a7c59, #6b8e23);
        }
        
        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 25px 50px rgba(45, 74, 45, 0.2);
            border-color: #6b8e23;
        }
        
        .project-emoji {
            font-size: 2rem;
            margin-bottom: 15px;
            display: block;
        }
        
        .project-title {
            font-size: 1.4rem;
            font-weight: 600;
            color: #2d4a2d;
            margin-bottom: 15px;
        }
        
        .project-desc {
            color: #4a7c59;
            margin-bottom: 20px;
            line-height: 1.7;
        }
        
        .project-impact {
            background: #e8f5e8;
            padding: 12px 18px;
            border-radius: 12px;
            border-left: 4px solid #6b8e23;
            margin-bottom: 20px;
            font-weight: 500;
        }
        
        .project-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 20px;
        }
        
        .repo-link {
            display: inline-block;
            padding: 10px 20px;
            background: linear-gradient(45deg, #4a7c59, #6b8e23);
            color: white;
            text-decoration: none;
            border-radius: 25px;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        
        .repo-link:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 25px rgba(74, 124, 89, 0.4);
        }
        
        .learning-list, .talk-list, .open-collabs {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
        }
        
        .list-item {
            background: linear-gradient(135deg, rgba(168, 213, 168, 0.4), rgba(144, 238, 144, 0.2));
            padding: 20px;
            border-radius: 15px;
            border-right: 4px solid #90ee90;
            position: relative;
        }
        
        .list-item::before {
            content: attr(data-emoji);
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 1.5rem;
            opacity: 0.6;
        }
        
        .internship, .certifications {
            background: linear-gradient(135deg, #f5f1df, #e9c785);
            border: 2px solid #e6aa15;
            border-radius: 20px;
            padding: 30px;
            margin-bottom: 40px;
        }
        
        .contact-cta {
            text-align: center;
            padding: 40px;
            background: linear-gradient(135deg, #4a7c59, #6b8e23);
            color: white;
            border-radius: 25px;
            margin-top: 40px;
        }
        
        @media (max-width: 768px) {
            .container {
                padding: 20px;
                margin: 10px;
            }
            
            .whoami-title {
                font-size: 2rem;
            }
            
            .info-grid {
                grid-template-columns: 1fr;
            }
        }
        
        .responsive-img {
            max-width: 100%;
            height: auto;
            border-radius: 15px;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header Badges -->
        <div class="header-badges">
            <a href="mailto:nidhijagadish2002@gmail.com" class="badge" title="Email Sunidhi">
                📧 Gmail
            </a>
            <a href="https://www.linkedin.com/in/sunidhi-jagadish-chandra/" class="badge" title="LinkedIn Profile">
                💼 LinkedIn
            </a>
            <a href="https://github.com/Sunidhi7602" class="badge" title="GitHub Repositories">
                🐙 GitHub
            </a>
            <a href="#" class="badge" title="Download Resume">
                📄 Resume
            </a>
            <span class="badge" title="Profile Views">
                👁️ 1.2k+
            </span>
        </div>

        <!-- Whoami Box -->
        <div class="whoami-box">
            <h1 class="whoami-title">whoami</h1>
            <div class="info-grid">
                <div class="info-item">
                    <div class="info-label">name</div>
                    <div class="info-value">✦ Sunidhi J</div>
                </div>
                <div class="info-item">
                    <div class="info-label">degree</div>
                    <div class="info-value">✦ MCA @ PES University, Bengaluru (July 2026)</div>
                </div>
                <div class="info-item">
                    <div class="info-label">internship</div>
                    <div class="info-value">✦ Full Stack Developer @ Yokogawa Tech Solutions</div>
                </div>
                <div class="info-item">
                    <div class="info-label">domain</div>
                    <div class="info-value">✦ Cybersecurity · Agentic AI · Full Stack Dev</div>
                </div>
                <div class="info-item">
                    <div class="info-label">building</div>
                    <div class="info-value">✦ Agentic AI Security Scanner (capstone, 2026)</div>
                </div>
                <div class="info-item">
                    <div class="info-label">interests</div>
                    <div class="info-value">✦ Mindful Living · Spirituality · Art & Craft</div>
                </div>
            </div>
        </div>

        <!-- Stack Section -->
        <div class="section">
            <h2 class="section-title">🌿 Stack</h2>
            <div class="stack-grid">
                <div class="stack-category">
                    <div class="stack-title">✦ Frontend ✦ 🌱</div>
                    <div class="tech-badges">
                        <span class="tech-badge">React</span>
                        <span class="tech-badge">Angular</span>
                        <span class="tech-badge">TypeScript</span>
                        <span class="tech-badge">Flutter</span>
                        <span class="tech-badge">HTML5</span>
                        <span class="tech-badge">CSS3</span>
                        <span class="tech-badge">SCSS</span>
                    </div>
                </div>
                <div class="stack-category">
                    <div class="stack-title">✦ Backend ✦ ⚙️</div>
                    <div class="tech-badges">
                        <span class="tech-badge">FastAPI</span>
                        <span class="tech-badge">NodeJS</span>
                        <span class="tech-badge">Express</span>
                        <span class="tech-badge">Flask</span>
                        <span class="tech-badge">Python</span>
                        <span class="tech-badge">Java</span>
                    </div>
                </div>
                <div class="stack-category">
                    <div class="stack-title">✦ Databases & Cloud ✦ ☁️</div>
                    <div class="tech-badges">
                        <span class="tech-badge">PostgreSQL</span>
                        <span class="tech-badge">MongoDB</span>
                        <span class="tech-badge">MySQL</span>
                        <span class="tech-badge">MongoAtlas</span>
                        <span class="tech-badge">Docker</span>
                        <span class="tech-badge">Firebase</span>
                        <span class="tech-badge">Redis</span>
                        <span class="tech-badge">Celery</span>
                    </div>
                </div>
                <div class="stack-category">
                    <div class="stack-title">✦ Cybersecurity ✦ 🛡️</div>
                    <div class="tech-badges">
                        <span class="tech-badge">OWASP ZAP</span>
                        <span class="tech-badge">BurpSuite</span>
                        <span class="tech-badge">Wireshark</span>
                        <span class="tech-badge">Nmap</span>
                        <span class="tech-badge">Linux</span>
                        <span class="tech-badge">Git</span>
                    </div>
                </div>
                <div class="stack-category">
                    <div class="stack-title">✦ Tools & Design ✦ 🛠️</div>
                    <div class="tech-badges">
                        <span class="tech-badge">VSCode</span>
                        <span class="tech-badge">IntelliJ</span>
                        <span class="tech-badge">Figma</span>
                        <span class="tech-badge">Postman</span>
                        <span class="tech-badge">Swagger</span>
                        <span class="tech-badge">Notion</span>
                        <span class="tech-badge">AndroidStudio</span>
                        <span class="tech-badge">Canva</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- Projects Section -->
        <div class="section">
            <h2 class="section-title">🌿 Projects</h2>
            <div class="projects-grid">
                <div class="project-card">
                    <span class="project-emoji">🔐</span>
                    <h3 class="project-title">Agentic AI Security Scanner</h3>
                    <p class="project-desc">Autonomous multi-agent security platform. Scans web apps with OWASP ZAP, maps vulnerabilities to CVE/OWASP Top 10, generates AI-powered patches via Gemini, and outputs consolidated security reports.</p>
                    <div class="project-impact">**Impact:** Detects & remediates vulnerabilities in minutes. Capstone project integrating cutting-edge AI security research.</div>
                    <div class="project-tech">
                        <span class="tech-badge">FastAPI</span>
                        <span class="tech-badge">OWASP ZAP</span>
                        <span class="tech-badge">Gemini AI</span>
                        <span class="tech-badge">MongoDB</span>
                        <span class="tech-badge">React</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/agentic-ai-security-scanner" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">🍯</span>
                    <h3 class="project-title">Honeypot Framework</h3>
                    <p class="project-desc">Deception-based intrusion detection system that monitors, logs, and visualizes attacker behavior in real time with centralized threat dashboards.</p>
                    <div class="project-impact">**Impact:** Published IEEE research. Successfully tracked 15+ attack patterns in testing phase.</div>
                    <div class="project-tech">
                        <span class="tech-badge">MongoDB</span>
                        <span class="tech-badge">React</span>
                        <span class="tech-badge">NodeJS</span>
                        <span class="tech-badge">SCSS</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/honeypot-framework" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">🏠</span>
                    <h3 class="project-title">Apartment Management App</h3>
                    <p class="project-desc">Full-stack tenant management with Aadhaar-based records, rent tracking, payment history, and analytics dashboards.</p>
                    <div class="project-impact">**Features:** Role-based access, automated rent reminders, financial analytics.</div>
                    <div class="project-tech">
                        <span class="tech-badge">React</span>
                        <span class="tech-badge">NodeJS</span>
                        <span class="tech-badge">TypeScript</span>
                        <span class="tech-badge">PostgreSQL</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/apartment-management-app" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">🧠</span>
                    <h3 class="project-title">Sudoku AI Web App</h3>
                    <p class="project-desc">AI-powered Sudoku solver with interactive gameplay, multiple difficulty levels, and algorithmic solving visualization.</p>
                    <div class="project-impact">**Features:** Backtracking algorithm visualization, hint system, progress tracking.</div>
                    <div class="project-tech">
                        <span class="tech-badge">Python</span>
                        <span class="tech-badge">Flask</span>
                        <span class="tech-badge">React</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/sudoku-ai-solver" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">🎟️</span>
                    <h3 class="project-title">Event Booking System</h3>
                    <p class="project-desc">End-to-end event and ticket management platform with authentication, scheduling, and booking workflows.</p>
                    <div class="project-impact">**Features:** JWT auth, real-time seat availability, invoice generation.</div>
                    <div class="project-tech">
                        <span class="tech-badge">Angular</span>
                        <span class="tech-badge">NodeJS</span>
                        <span class="tech-badge">TypeScript</span>
                        <span class="tech-badge">PostgreSQL</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/event-booking-system" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">📱</span>
                    <h3 class="project-title">Mental Health Support App</h3>
                    <p class="project-desc">Android wellness app for mood tracking, emotional support, and community-based mental health assistance.</p>
                    <div class="project-impact">**Features:** Daily mood logging, AI-driven recommendations, crisis resources.</div>
                    <div class="project-tech">
                        <span class="tech-badge">Android Studio</span>
                        <span class="tech-badge">Firebase</span>
                        <span class="tech-badge">Figma</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/mental-health-support-app" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">🌐</span>
                    <h3 class="project-title">Community Connect App</h3>
                    <p class="project-desc">Social-community Android app enabling local interaction, announcements, and neighborhood engagement features.</p>
                    <div class="project-impact">**Features:** Real-time notifications, community forums, event calendar.</div>
                    <div class="project-tech">
                        <span class="tech-badge">Android Studio</span>
                        <span class="tech-badge">Firebase</span>
                        <span class="tech-badge">Figma</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/community-connect-app" class="repo-link">🌿 view repo</a>
                </div>

                <div class="project-card">
                    <span class="project-emoji">⚡</span>
                    <h3 class="project-title">VitalCheck</h3>
                    <p class="project-desc">All-in-one health website with BMI calculator, personalized diet suggestions, and daily fitness activity tracker with progress visualization.</p>
                    <div class="project-impact">**Features:** Nutrition database integration, workout plans, progress analytics.</div>
                    <div class="project-tech">
                        <span class="tech-badge">HTML5</span>
                        <span class="tech-badge">CSS3</span>
                        <span class="tech-badge">JavaScript</span>
                        <span class="tech-badge">Java</span>
                    </div>
                    <a href="https://github.com/Sunidhi7602/vitalcheck" class="repo-link">🌿 view repo</a>
                </div>
            </div>
        </div>

        <!-- Currently Learning -->
        <div class="section">
            <h2 class="section-title">🌿 Currently Learning</h2>
            <div class="learning-list">
                <div class="list-item" data-emoji="🤖">
                    Advanced LLM Agents & Multi-Agent Orchestration — Pushing boundaries of autonomous security systems
                </div>
                <div class="list-item" data-emoji="☁️">
                    Cloud Security — AWS & GCP security certifications in progress
                </div>
                <div class="list-item" data-emoji="🔐">
                    Zero-Trust Architecture — Modern security paradigms for distributed systems
                </div>
                <div class="list-item" data-emoji="🛠️">
                    LangChain & Vector Databases — Enhancing AI agent capabilities
                </div>
            </div>
        </div>

        <!-- Talk to Me About -->
        <div class="section">
            <h2 class="section-title">🌿 Talk to Me About</h2>
            <div class="talk-list">
                <div class="list-item" data-emoji="🤖">Agentic AI Security — Building intelligent systems for vulnerability detection & remediation</div>
                <div class="list-item" data-emoji="🔒">OWASP & Threat Modeling — Web application security best practices</div>
                <div class="list-item" data-emoji="🌐">Full Stack Development — End-to-end system design and implementation</div>
                <div class="list-item" data-emoji="🔬">Cybersecurity Research — Emerging threats, intrusion detection, threat intelligence</div>
                <div class="list-item" data-emoji="🧘">Mindfulness & Digital Wellness — Balance in tech careers</div>
            </div>
        </div>

        <!-- Internship Experience -->
        <div class="internship">
            <h2 class="section-title" style="color: #5d4037;">🌿 Internship Experience</h2>
            <div style="font-size: 1.2rem; line-height: 1.8; color: #5d4037;">
                <strong>Full Stack Developer @ Yokogawa Tech Solutions (Current)</strong><br><br>
                Developing full-stack solutions for industrial IoT platforms<br>
                Building secure, scalable backend systems with FastAPI & Node.js<br>
                Implementing responsive frontends with React<br>
                Collaborating with cross-functional teams on production deployments
            </div>
        </div>

        <!-- Certifications -->
        <div class="certifications">
            <h2 class="section-title" style="color: #5d4037;">🌿 Certifications & Research</h2>
            <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px;">
                <div style="background: rgba(255,255,255,0.8); padding: 20px; border-radius: 15px; text-align: center;">
                    <span style="font-size: 2rem; display: block; margin-bottom: 10px;">🛡️</span>
                    ISC² Certified in Cybersecurity (CC)
                </div>
                <div style="background: rgba(255,255,255,0.8); padding: 20px; border-radius: 15px; text-align: center;">
                    <span style="font-size: 2rem; display: block; margin-bottom: 10px;">📘</span>
                    NPTEL — Cybersecurity and Privacy
                </div>
                <div style="background: rgba(255,255,255,0.8); padding: 20px; border-radius: 15px; text-align: center;">
                    <span style="font-size: 2rem; display: block; margin-bottom: 10px;">🔬</span>
                    IEEE Research — Honeypot Intrusion Detection
                </div>
            </div>
        </div>

        <!-- Open to Collaboration -->
        <div class="contact-cta">
            <h2 style="font-family: 'Dancing Script', cursive; font-size: 3rem; margin-bottom: 20px;">🌿 Open to Collaboration</h2>
            <p style="font-size: 1.3rem; margin-bottom: 30px; opacity: 0.95;">
                I'm actively looking for opportunities in:<br>
                🤖 Agentic AI Security · 🔒 Application Security · 🌐 Full Stack Development · 📚 Open Source Security Projects
            </p>
            <p style="font-size: 1.2rem;">
                Let's build something secure and intelligent together!<br>
                Feel free to reach out via 
                <a href="mailto:nidhijagadish2002@gmail.com" style="color: #f5f1df; text-decoration: underline;">email</a> 
                or 
                <a href="https://www.linkedin.com/in/sunidhi-jagadish-chandra/" style="color: #f5f1df; text-decoration: underline;">LinkedIn</a>.
            </p>
        </div>
    </div>
</body>
</html>
