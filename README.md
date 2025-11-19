<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ishanka Chathuranga Botheju - GitHub Profile</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            background: #0d1117;
            color: #c9d1d9;
            min-height: 100vh;
        }

        .github-container {
            display: grid;
            grid-template-columns: 320px 1fr;
            gap: 24px;
            max-width: 1400px;
            margin: 0 auto;
            padding: 32px 24px;
        }

        /* Left Sidebar */
        .sidebar {
            position: sticky;
            top: 32px;
            height: fit-content;
        }

        .profile-image {
            width: 100%;
            aspect-ratio: 1;
            border-radius: 50%;
            border: 1px solid #30363d;
            margin-bottom: 16px;
            object-fit: cover;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 120px;
        }

        .profile-name {
            font-size: 26px;
            font-weight: 600;
            line-height: 1.25;
            color: #c9d1d9;
            margin-bottom: 4px;
        }

        .profile-username {
            font-size: 20px;
            font-weight: 300;
            color: #8b949e;
            margin-bottom: 16px;
        }

        .follow-btn {
            width: 100%;
            padding: 8px 16px;
            background: #21262d;
            color: #c9d1d9;
            border: 1px solid #30363d;
            border-radius: 6px;
            font-size: 14px;
            font-weight: 500;
            cursor: pointer;
            transition: background 0.2s;
        }

        .follow-btn:hover {
            background: #30363d;
        }

        .profile-bio {
            margin-top: 16px;
            font-size: 14px;
            line-height: 1.5;
            color: #c9d1d9;
        }

        .profile-stats {
            display: flex;
            gap: 8px;
            margin-top: 16px;
            font-size: 14px;
            color: #8b949e;
        }

        .profile-stats a {
            color: #8b949e;
            text-decoration: none;
        }

        .profile-stats a:hover {
            color: #58a6ff;
        }

        .profile-info {
            margin-top: 16px;
        }

        .info-item {
            display: flex;
            align-items: center;
            gap: 8px;
            margin-bottom: 8px;
            font-size: 14px;
            color: #8b949e;
        }

        .info-item svg {
            width: 16px;
            height: 16px;
            fill: #8b949e;
        }

        .info-item a {
            color: #58a6ff;
            text-decoration: none;
        }

        .info-item a:hover {
            text-decoration: underline;
        }

        .achievements {
            margin-top: 24px;
        }

        .section-title {
            font-size: 16px;
            font-weight: 600;
            margin-bottom: 12px;
        }

        .achievement-badge {
            width: 64px;
            height: 64px;
            border-radius: 50%;
            border: 1px solid #30363d;
            background: #161b22;
        }

        /* Main Content */
        .main-content {
            min-width: 0;
        }

        .tabs {
            display: flex;
            gap: 16px;
            border-bottom: 1px solid #21262d;
            margin-bottom: 24px;
        }

        .tab {
            padding: 16px 8px;
            color: #8b949e;
            text-decoration: none;
            border-bottom: 2px solid transparent;
            font-size: 14px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .tab.active {
            color: #c9d1d9;
            border-bottom-color: #f78166;
        }

        .readme-header {
            display: flex;
            align-items: center;
            gap: 8px;
            padding: 12px 16px;
            background: #161b22;
            border: 1px solid #30363d;
            border-bottom: none;
            border-radius: 6px 6px 0 0;
            font-size: 14px;
            color: #8b949e;
        }

        .readme-content {
            background: #0d1117;
            border: 1px solid #30363d;
            border-radius: 0 0 6px 6px;
            padding: 32px;
        }

        .readme-title {
            font-size: 32px;
            font-weight: 600;
            margin-bottom: 16px;
            text-align: center;
        }

        .readme-subtitle {
            font-size: 20px;
            text-align: center;
            margin-bottom: 24px;
            color: #8b949e;
        }

        .profile-views {
            display: inline-block;
            padding: 4px 8px;
            background: #1f6feb;
            border-radius: 4px;
            font-size: 12px;
            margin-left: 8px;
        }

        .role-badges {
            text-align: center;
            font-size: 18px;
            color: #f0883e;
            margin-bottom: 32px;
            padding: 16px;
            border-top: 1px solid #21262d;
            border-bottom: 1px solid #21262d;
        }

        .info-section {
            margin: 24px 0;
        }

        .info-section ul {
            list-style: none;
        }

        .info-section li {
            padding: 8px 0;
            line-height: 1.6;
        }

        .info-section li::before {
            content: "•";
            color: #f0883e;
            font-weight: bold;
            display: inline-block;
            width: 1em;
            margin-left: -1em;
        }

        .info-section a {
            color: #58a6ff;
            text-decoration: none;
        }

        .info-section a:hover {
            text-decoration: underline;
        }

        .connect-section {
            text-align: center;
            margin: 32px 0;
            padding: 24px;
            background: #161b22;
            border-radius: 6px;
        }

        .social-icon {
            display: inline-flex;
            width: 64px;
            height: 64px;
            background: #0a66c2;
            border-radius: 8px;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            color: white;
            text-decoration: none;
            transition: transform 0.2s;
        }

        .social-icon:hover {
            transform: scale(1.1);
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            justify-content: center;
            padding: 24px;
            background: #161b22;
            border-radius: 6px;
            margin: 24px 0;
        }

        .tech-icon {
            width: 48px;
            height: 48px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #21262d;
            border-radius: 8px;
            font-size: 32px;
            transition: transform 0.2s;
        }

        .tech-icon:hover {
            transform: scale(1.1);
        }

        .trophies-section {
            margin-top: 32px;
        }

        .trophies-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
            gap: 16px;
            margin-top: 16px;
        }

        .trophy-card {
            background: #161b22;
            border: 1px solid #30363d;
            border-radius: 6px;
            padding: 16px;
            text-align: center;
        }

        .trophy-icon {
            font-size: 48px;
            margin-bottom: 8px;
        }

        .trophy-title {
            font-size: 12px;
            color: #8b949e;
            margin-bottom: 4px;
        }

        .trophy-rank {
            font-size: 14px;
            font-weight: 600;
            color: #f0883e;
        }

        @media (max-width: 768px) {
            .github-container {
                grid-template-columns: 1fr;
            }
            
            .sidebar {
                position: relative;
                top: 0;
            }
        }
    </style>
</head>
<body>
    <div class="github-container">
        <!-- Left Sidebar -->
        <div class="sidebar">
            <div class="profile-image">👨‍💻</div>
            
            <h1 class="profile-name">Ishanka Chathuranga</h1>
            <div class="profile-username">Ishanka-git</div>
            
            <button class="follow-btn">Follow</button>
            
            <div class="profile-bio">
                Data Science Student passionate about tech, ML, and automation. Skilled in web development, problem solving, and teamwork, always eager to learn and innovate.
            </div>
            
            <div class="profile-stats">
                <a href="#"><strong>0</strong> followers</a>
                •
                <a href="#"><strong>0</strong> following</a>
            </div>
            
            <div class="profile-info">
                <div class="info-item">
                    <svg viewBox="0 0 16 16"><path d="M11.536 3.464a5 5 0 010 7.072L8 14.07l-3.536-3.535a5 5 0 117.072-7.072v.001zm1.06 8.132a6.5 6.5 0 10-9.192 0l3.535 3.536a1.5 1.5 0 002.122 0l3.535-3.536zM8 9a2 2 0 100-4 2 2 0 000 4z"></path></svg>
                    Sri Lanka 🇱🇰
                </div>
                <div class="info-item">
                    <svg viewBox="0 0 16 16"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path></svg>
                    <a href="#">ishanka.vercel.app</a>
                </div>
                <div class="info-item">
                    <svg viewBox="0 0 16 16"><path d="M13.545 2.907a13.227 13.227 0 0 0-3.257-1.011.05.05 0 0 0-.052.025c-.141.25-.297.577-.406.833a12.19 12.19 0 0 0-3.658 0 8.258 8.258 0 0 0-.412-.833.051.051 0 0 0-.052-.025c-1.125.194-2.22.534-3.257 1.011a.041.041 0 0 0-.021.018C.356 6.024-.213 9.047.066 12.032c.001.014.01.028.021.037a13.276 13.276 0 0 0 3.995 2.02.05.05 0 0 0 .056-.019c.308-.42.582-.863.818-1.329a.05.05 0 0 0-.01-.059.051.051 0 0 0-.018-.011 8.875 8.875 0 0 1-1.248-.595.05.05 0 0 1-.02-.066.051.051 0 0 1 .015-.019c.084-.063.168-.129.248-.195a.05.05 0 0 1 .051-.007c2.619 1.196 5.454 1.196 8.041 0a.052.052 0 0 1 .053.007c.08.066.164.132.248.195a.051.051 0 0 1-.004.085 8.254 8.254 0 0 1-1.249.594.05.05 0 0 0-.03.03.052.052 0 0 0 .003.041c.24.465.515.909.817 1.329a.05.05 0 0 0 .056.019 13.235 13.235 0 0 0 4.001-2.02.049.049 0 0 0 .021-.037c.334-3.451-.559-6.449-2.366-9.106a.034.034 0 0 0-.02-.019Zm-8.198 7.307c-.789 0-1.438-.724-1.438-1.612 0-.889.637-1.613 1.438-1.613.807 0 1.45.73 1.438 1.613 0 .888-.637 1.612-1.438 1.612Zm5.316 0c-.788 0-1.438-.724-1.438-1.612 0-.889.637-1.613 1.438-1.613.807 0 1.451.73 1.438 1.613 0 .888-.631 1.612-1.438 1.612Z"></path></svg>
                    in/ishanka-botheju
                </div>
                <div class="info-item">
                    <svg viewBox="0 0 16 16"><path d="M1.5 8a6.5 6.5 0 1113 0 6.5 6.5 0 01-13 0zM8 0a8 8 0 100 16A8 8 0 008 0zm.5 4.75a.75.75 0 00-1.5 0v3.5a.75.75 0 00.471.696l2.5 1a.75.75 0 00.557-1.392L8.5 7.742V4.75z"></path></svg>
                    ishanka.fb
                </div>
            </div>
            
            <div class="achievements">
                <div class="section-title">Achievements</div>
                <div class="achievement-badge">🎖️</div>
            </div>
        </div>

        <!-- Main Content -->
        <div class="main-content">
            <div class="tabs">
                <a href="#" class="tab active">📖 Overview</a>
                <a href="#" class="tab">📁 Repositories <span style="background:#30363d;padding:2px 6px;border-radius:12px;font-size:12px;">0</span></a>
                <a href="#" class="tab">📦 Projects</a>
                <a href="#" class="tab">📦 Packages</a>
                <a href="#" class="tab">⭐ Stars</a>
            </div>

            <div class="readme-header">
                🔗 Ishanka-git / README.md
            </div>

            <div class="readme-content">
                <h1 class="readme-title">Hi, I'm Ishanka Chathuranga Botheju</h1>
                
                <div class="readme-subtitle">
                    Always excited to learn, build, and collaborate!
                    <span class="profile-views">Profile views 345</span>
                </div>

                <div class="role-badges">
                    Data Science Student | Machine Learning Enthusiast | AI & Deep Learning
                </div>

                <div class="info-section">
                    <ul>
                        <li>I'm currently learning <strong>Python, R, TensorFlow, and React</strong></li>
                        <li>All of my projects are available on <a href="#">LinkedIn</a></li>
                        <li>Reach me via: <a href="#">ishanka@example.com</a></li>
                        <li>More about me on <a href="#">LinkedIn</a></li>
                        <li><strong>Fun fact:</strong> I can debug code faster than I can decide what to eat! 😋💻</li>
                    </ul>
                </div>

                <div class="connect-section">
                    <h3 style="margin-bottom: 16px;">🔗 Connect with me:</h3>
                    <a href="#" class="social-icon">in</a>
                </div>

                <div class="info-section">
                    <h3 style="margin-bottom: 16px;">🛠️ Languages & Tools</h3>
                </div>

                <div class="tech-stack">
                    <div class="tech-icon" title="React">⚛️</div>
                    <div class="tech-icon" title="Angular">🅰️</div>
                    <div class="tech-icon" title="Flutter">🦋</div>
                    <div class="tech-icon" title="GraphQL">◼️</div>
                    <div class="tech-icon" title="Node.js">🟢</div>
                    <div class="tech-icon" title="Tailwind">🌊</div>
                    <div class="tech-icon" title="HTML5">🌐</div>
                    <div class="tech-icon" title="CSS3">🎨</div>
                    <div class="tech-icon" title="JavaScript">JS</div>
                    <div class="tech-icon" title="TypeScript">TS</div>
                    <div class="tech-icon" title="Java">☕</div>
                    <div class="tech-icon" title="C">C</div>
                    <div class="tech-icon" title="C++">C++</div>
                    <div class="tech-icon" title="Python">🐍</div>
                    <div class="tech-icon" title="MongoDB">🍃</div>
                    <div class="tech-icon" title="Firebase">🔥</div>
                    <div class="tech-icon" title="AWS">☁️</div>
                    <div class="tech-icon" title="Azure">🔷</div>
                    <div class="tech-icon" title="TensorFlow">🧠</div>
                    <div class="tech-icon" title="PyTorch">🔦</div>
                    <div class="tech-icon" title="Git">📊</div>
                    <div class="tech-icon" title="GitHub">🐙</div>
                    <div class="tech-icon" title="VS Code">💻</div>
                </div>

                <div class="trophies-section">
                    <h3 style="margin-bottom: 16px;">🏆 GitHub Trophies</h3>
                    
                    <div class="trophies-grid">
                        <div class="trophy-card">
                            <div class="trophy-icon">🔤</div>
                            <div class="trophy-title">MultiLanguage</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">💬</div>
                            <div class="trophy-title">Commits</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">📚</div>
                            <div class="trophy-title">Repositories</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">⭐</div>
                            <div class="trophy-title">Experience</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">👥</div>
                            <div class="trophy-title">Followers</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">🎯</div>
                            <div class="trophy-title">Issues</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">🔀</div>
                            <div class="trophy-title">Pull Requests</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                        <div class="trophy-card">
                            <div class="trophy-icon">⚡</div>
                            <div class="trophy-title">Stars</div>
                            <div class="trophy-rank">GOLD</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</body>
</html>
