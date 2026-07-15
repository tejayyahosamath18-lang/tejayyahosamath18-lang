<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>tejayye · GitHub Profile</title>
    <!-- Font Awesome 6 (free) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" />
    <style>
        /* ── reset & base ── */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: radial-gradient(ellipse at 20% 50%, #1a1a2e, #0f0f1a 70%);
            padding: 2rem 1rem;
        }

        /* ── main glass container ── */
        .glass-wrapper {
            max-width: 1100px;
            width: 100%;
            background: rgba(255, 255, 255, 0.06);
            backdrop-filter: blur(18px) saturate(180%);
            -webkit-backdrop-filter: blur(18px) saturate(180%);
            border-radius: 3rem;
            padding: 2.5rem 2.8rem;
            border: 1px solid rgba(255, 255, 255, 0.10);
            box-shadow: 0 30px 80px rgba(0, 0, 0, 0.7), inset 0 1px 0 rgba(255, 255, 255, 0.06);
            transition: all 0.25s ease;
        }

        /* ── scrollable inner (if needed) ── */
        .glass-inner {
            display: flex;
            flex-direction: column;
            gap: 2.2rem;
        }

        /* ── typography ── */
        h1,
        h2,
        h3,
        p,
        a,
        li,
        span {
            color: #f0f2fa;
            letter-spacing: 0.01em;
        }

        h1 {
            font-size: 2.6rem;
            font-weight: 700;
            background: linear-gradient(135deg, #f0f2fa 30%, #a0b4ff 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            letter-spacing: -0.02em;
        }

        h2 {
            font-size: 1.3rem;
            font-weight: 600;
            color: #c8d0f0;
            margin-bottom: 0.4rem;
            letter-spacing: -0.01em;
        }

        h3 {
            font-size: 1.05rem;
            font-weight: 500;
            color: #d0d8f5;
            margin-bottom: 0.6rem;
        }

        .subhead {
            font-size: 1rem;
            color: #a8b2dd;
            font-weight: 400;
            margin-top: -0.2rem;
        }

        /* ── glass card ── */
        .glass-card {
            background: rgba(255, 255, 255, 0.04);
            backdrop-filter: blur(10px) saturate(160%);
            -webkit-backdrop-filter: blur(10px) saturate(160%);
            border-radius: 2rem;
            padding: 1.6rem 2rem;
            border: 1px solid rgba(255, 255, 255, 0.07);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3), inset 0 1px 0 rgba(255, 255, 255, 0.04);
            transition: transform 0.2s ease, box-shadow 0.25s ease;
        }

        .glass-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 14px 44px rgba(0, 0, 0, 0.45), inset 0 1px 0 rgba(255, 255, 255, 0.06);
        }

        /* ── header row ── */
        .profile-header {
            display: flex;
            align-items: center;
            gap: 1.8rem;
            flex-wrap: wrap;
        }

        .avatar {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            background: linear-gradient(135deg, #6c7cff, #a78bfa);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.4rem;
            font-weight: 700;
            color: #fff;
            box-shadow: 0 8px 28px rgba(108, 124, 255, 0.35);
            border: 2px solid rgba(255, 255, 255, 0.15);
            flex-shrink: 0;
        }

        .header-text {
            flex: 1;
        }

        .header-text .handle {
            font-size: 1.1rem;
            font-weight: 400;
            color: #a8b2dd;
            background: rgba(255, 255, 255, 0.06);
            padding: 0.2rem 1rem;
            border-radius: 40px;
            display: inline-block;
            border: 1px solid rgba(255, 255, 255, 0.05);
        }

        .header-text .handle i {
            margin-right: 0.4rem;
            color: #7c8cff;
        }

        /* ── about grid ── */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.8rem;
        }

        .about-grid .glass-card {
            padding: 1.4rem 1.8rem;
        }

        .about-grid ul {
            list-style: none;
            margin-top: 0.3rem;
        }

        .about-grid ul li {
            font-size: 0.95rem;
            padding: 0.3rem 0;
            color: #d0d8f5;
            display: flex;
            align-items: flex-start;
            gap: 0.6rem;
            line-height: 1.5;
        }

        .about-grid ul li i {
            color: #7c8cff;
            width: 1.1rem;
            margin-top: 0.2rem;
            font-size: 0.85rem;
        }

        .tag-group {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-top: 0.3rem;
        }

        .tag {
            background: rgba(108, 124, 255, 0.15);
            border: 1px solid rgba(108, 124, 255, 0.15);
            padding: 0.25rem 1rem;
            border-radius: 40px;
            font-size: 0.8rem;
            font-weight: 500;
            color: #c8d0f5;
            transition: all 0.2s;
            backdrop-filter: blur(4px);
        }

        .tag:hover {
            background: rgba(108, 124, 255, 0.25);
            border-color: rgba(108, 124, 255, 0.3);
            transform: scale(1.04);
        }

        /* ── socials ── */
        .social-row {
            display: flex;
            gap: 1.4rem;
            flex-wrap: wrap;
            align-items: center;
        }

        .social-row a {
            color: #b0bce8;
            font-size: 1.3rem;
            transition: all 0.2s;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.4rem;
            background: rgba(255, 255, 255, 0.04);
            padding: 0.4rem 1.2rem 0.4rem 1rem;
            border-radius: 40px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 0.9rem;
            font-weight: 500;
        }

        .social-row a i {
            font-size: 1.2rem;
        }

        .social-row a:hover {
            color: #ffffff;
            background: rgba(108, 124, 255, 0.18);
            border-color: rgba(108, 124, 255, 0.25);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(108, 124, 255, 0.15);
        }

        /* ── tech stack ── */
        .tech-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 0.6rem 1rem;
            margin-top: 0.2rem;
        }

        .tech-item {
            font-size: 0.85rem;
            font-weight: 500;
            color: #c8d0f5;
            background: rgba(255, 255, 255, 0.04);
            padding: 0.3rem 1.2rem;
            border-radius: 40px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(4px);
            transition: all 0.2s;
        }

        .tech-item:hover {
            background: rgba(108, 124, 255, 0.12);
            border-color: rgba(108, 124, 255, 0.15);
        }

        .tech-item i {
            margin-right: 0.4rem;
            color: #7c8cff;
            font-size: 0.8rem;
        }

        /* ── stats row ── */
        .stats-row {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 1.2rem;
        }

        .stat-card {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 1.4rem;
            padding: 1.2rem 0.8rem;
            text-align: center;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: all 0.2s;
        }

        .stat-card:hover {
            background: rgba(255, 255, 255, 0.06);
            transform: translateY(-3px);
        }

        .stat-number {
            font-size: 2.2rem;
            font-weight: 700;
            background: linear-gradient(135deg, #f0f2fa, #a0b4ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            line-height: 1.2;
        }

        .stat-label {
            font-size: 0.75rem;
            text-transform: uppercase;
            letter-spacing: 0.06em;
            color: #8892b8;
            font-weight: 500;
            margin-top: 0.2rem;
        }

        .stat-sub {
            font-size: 0.7rem;
            color: #6a74a0;
            margin-top: 0.1rem;
        }

        /* ── languages & repos ── */
        .two-col {
            display: grid;
            grid-template-columns: 1fr 1.6fr;
            gap: 1.8rem;
        }

        .lang-bar {
            display: flex;
            flex-direction: column;
            gap: 0.5rem;
            margin-top: 0.4rem;
        }

        .lang-row {
            display: flex;
            align-items: center;
            gap: 0.8rem;
        }

        .lang-row .name {
            width: 90px;
            font-size: 0.85rem;
            font-weight: 500;
            color: #d0d8f5;
            flex-shrink: 0;
        }

        .lang-track {
            flex: 1;
            height: 6px;
            background: rgba(255, 255, 255, 0.06);
            border-radius: 20px;
            overflow: hidden;
        }

        .lang-track .fill {
            height: 100%;
            border-radius: 20px;
            background: linear-gradient(90deg, #6c7cff, #a78bfa);
            width: 0%;
        }

        .lang-row .pct {
            font-size: 0.8rem;
            font-weight: 500;
            color: #8892b8;
            width: 44px;
            text-align: right;
        }

        .repo-list {
            display: flex;
            flex-direction: column;
            gap: 0.8rem;
        }

        .repo-item {
            background: rgba(255, 255, 255, 0.03);
            border-radius: 1.2rem;
            padding: 0.8rem 1.2rem;
            border: 1px solid rgba(255, 255, 255, 0.04);
            transition: all 0.2s;
        }

        .repo-item:hover {
            background: rgba(255, 255, 255, 0.06);
            border-color: rgba(108, 124, 255, 0.12);
        }

        .repo-item .repo-name {
            font-weight: 600;
            font-size: 0.95rem;
            color: #e0e6ff;
            display: flex;
            align-items: center;
            gap: 0.6rem;
        }

        .repo-item .repo-name i {
            color: #7c8cff;
            font-size: 0.8rem;
        }

        .repo-item .repo-desc {
            font-size: 0.82rem;
            color: #a8b2dd;
            margin-top: 0.2rem;
            line-height: 1.5;
        }

        .repo-item .repo-meta {
            display: flex;
            gap: 1rem;
            margin-top: 0.3rem;
            font-size: 0.7rem;
            color: #6a74a0;
        }

        .repo-item .repo-meta i {
            margin-right: 0.2rem;
        }

        /* ── contributor badge ── */
        .contrib-badge {
            display: inline-flex;
            align-items: center;
            gap: 0.4rem;
            background: rgba(108, 124, 255, 0.10);
            padding: 0.2rem 1rem 0.2rem 0.8rem;
            border-radius: 40px;
            font-size: 0.75rem;
            color: #b0bce8;
            border: 1px solid rgba(108, 124, 255, 0.08);
            margin-top: 0.5rem;
        }

        .contrib-badge i {
            color: #7c8cff;
        }

        /* ── responsive ── */
        @media (max-width: 860px) {
            .glass-wrapper {
                padding: 1.8rem 1.4rem;
                border-radius: 2rem;
            }
            .about-grid {
                grid-template-columns: 1fr;
            }
            .stats-row {
                grid-template-columns: repeat(2, 1fr);
            }
            .two-col {
                grid-template-columns: 1fr;
            }
            .profile-header {
                flex-direction: column;
                align-items: flex-start;
            }
            h1 {
                font-size: 2rem;
            }
            .social-row a {
                padding: 0.3rem 0.9rem 0.3rem 0.8rem;
                font-size: 0.8rem;
            }
        }

        @media (max-width: 480px) {
            .glass-wrapper {
                padding: 1.2rem 0.8rem;
                border-radius: 1.4rem;
            }
            .glass-card {
                padding: 1rem 1rem;
                border-radius: 1.4rem;
            }
            .stats-row {
                grid-template-columns: 1fr 1fr;
                gap: 0.6rem;
            }
            .stat-number {
                font-size: 1.6rem;
            }
            .tech-item {
                font-size: 0.75rem;
                padding: 0.2rem 0.8rem;
            }
            .repo-item .repo-desc {
                font-size: 0.75rem;
            }
        }

        /* ── scrollbar polish ── */
        ::-webkit-scrollbar {
            width: 5px;
        }
        ::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.02);
            border-radius: 20px;
        }
        ::-webkit-scrollbar-thumb {
            background: rgba(108, 124, 255, 0.3);
            border-radius: 20px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: rgba(108, 124, 255, 0.5);
        }

        /* small extra */
        .mt-1 {
            margin-top: 0.6rem;
        }
        .flex-wrap {
            display: flex;
            flex-wrap: wrap;
            gap: 0.6rem 1.2rem;
        }
        .text-glow {
            text-shadow: 0 0 30px rgba(108, 124, 255, 0.15);
        }
        .divider-light {
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.04), transparent);
            margin: 0.2rem 0 1rem 0;
        }
    </style>
</head>
<body>

    <div class="glass-wrapper">
        <div class="glass-inner">

            <!-- ─── HEADER ─── -->
            <div class="profile-header">
                <div class="avatar">T</div>
                <div class="header-text">
                    <h1>tejayye</h1>
                    <div class="handle">
                        <i class="fab fa-github"></i> GitHub.com/tejayye
                    </div>
                    <p class="subhead" style="margin-top:0.3rem;">
                        <i class="fas fa-code" style="color:#7c8cff;margin-right:0.4rem;"></i>
                        Data Analytics · AI Automation · Business Intelligence
                    </p>
                </div>
            </div>

            <!-- ─── ABOUT ─── -->
            <div class="about-grid">
                <!-- left -->
                <div class="glass-card">
                    <h2><i class="fas fa-user-astronaut" style="color:#7c8cff;margin-right:0.6rem;"></i> About Me</h2>
                    <ul>
                        <li><i class="fas fa-briefcase"></i> Data Analytics · Python · SQL · Excel · Power BI · Tableau</li>
                        <li><i class="fas fa-handshake"></i> Open Source · AI Automation · BI projects</li>
                        <li><i class="fas fa-graduation-cap"></i> Learning: RStudio · Big Data · ML · n8n · Git · Pandas · NumPy · Jupyter</li>
                        <li><i class="fas fa-lightbulb"></i> Ask me about Python, SQL, Power BI, Tableau, Tally Prime, Automation</li>
                        <li><i class="fas fa-heart" style="color:#f472b6;"></i> Transforming raw data into meaningful insights</li>
                    </ul>
                </div>

                <!-- right -->
                <div class="glass-card">
                    <h2><i class="fas fa-rocket" style="color:#7c8cff;margin-right:0.6rem;"></i> Current Focus</h2>
                    <ul>
                        <li><i class="fas fa-database"></i> Data Analytics projects (Python, SQL, Power BI, Tableau)</li>
                        <li><i class="fas fa-robot"></i> AI Automation &amp; Machine Learning</li>
                        <li><i class="fas fa-code-branch"></i> Open Source collaboration</li>
                        <li><i class="fas fa-chart-line"></i> Real-world business intelligence</li>
                        <li><i class="fas fa-tools"></i> RStudio · Big Data · n8n · Jupyter Lab</li>
                    </ul>
                    <div class="contrib-badge">
                        <i class="fas fa-users"></i> Looking to collaborate &amp; grow
                    </div>
                </div>
            </div>

            <!-- ─── SOCIALS ─── -->
            <div class="glass-card" style="padding:1rem 1.8rem;">
                <div class="social-row">
                    <a href="https://www.instagram.com/" target="_blank"><i class="fab fa-instagram"></i> Instagram</a>
                    <a href="https://www.linkedin.com/" target="_blank"><i class="fab fa-linkedin-in"></i> LinkedIn</a>
                    <a href="https://www.mastodon.social/" target="_blank"><i class="fab fa-mastodon"></i> Mastodon</a>
                    <a href="https://twitter.com/" target="_blank"><i class="fab fa-twitter"></i> Twitter</a>
                    <span style="color:#6a74a0;font-size:0.75rem;margin-left:auto;"><i class="fas fa-globe"></i> @tejayye</span>
                </div>
            </div>

            <!-- ─── TECH STACK ─── -->
            <div class="glass-card">
                <h2><i class="fas fa-microchip" style="color:#7c8cff;margin-right:0.6rem;"></i> Tech Stack</h2>
                <div class="tech-grid">
                    <span class="tech-item"><i class="fab fa-python"></i> Python</span>
                    <span class="tech-item"><i class="fas fa-database"></i> MySQL</span>
                    <span class="tech-item"><i class="fas fa-database"></i> SQLite</span>
                    <span class="tech-item"><i class="fas fa-server"></i> MS SQL Server</span>
                    <span class="tech-item"><i class="fas fa-chart-pie"></i> Power BI</span>
                    <span class="tech-item"><i class="fab fa-aws"></i> AWS</span>
                    <span class="tech-item"><i class="fab fa-google"></i> Google Cloud</span>
                    <span class="tech-item"><i class="fab fa-github"></i> GitHub</span>
                    <span class="tech-item"><i class="fas fa-cogs"></i> GitHub Actions</span>
                    <span class="tech-item"><i class="fas fa-database"></i> Teradata</span>
                    <span class="tech-item"><i class="fas fa-table"></i> Pandas</span>
                    <span class="tech-item"><i class="fas fa-calculator"></i> NumPy</span>
                    <span class="tech-item"><i class="fas fa-chart-bar"></i> Tableau</span>
                    <span class="tech-item"><i class="fas fa-cube"></i> Tally Prime</span>
                    <span class="tech-item"><i class="fas fa-code"></i> RStudio</span>
                    <span class="tech-item"><i class="fas fa-robot"></i> n8n</span>
                    <span class="tech-item"><i class="fas fa-book"></i> Jupyter</span>
                </div>
            </div>

            <!-- ─── STATS ─── -->
            <div class="glass-card">
                <h2><i class="fas fa-chart-simple" style="color:#7c8cff;margin-right:0.6rem;"></i> GitHub Stats</h2>
                <div class="stats-row">
                    <div class="stat-card">
                        <div class="stat-number">25</div>
                        <div class=
