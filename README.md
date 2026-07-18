# 💫 About Me:
🔭 I'm currently working on<br>Data Analytics projects using Python, SQL, Excel, Power BI, and Tableau.<br><br>👯 I'm looking to collaborate on<br>Open Source, Data Analytics, AI Automation, and Business Intelligence projects.<br><br>🤝 I'm looking for help with<br>Real-world Data Analytics projects, Machine Learning, and career opportunities.<br><br>🌱 I'm currently learning<br>RStudio, Big Data, Machine Learning, AI Automation, n8n, Git, GitHub, Pandas, NumPy, and Jupyter Notebook/Lab.<br><br>💬 Ask me about<br>Python, SQL, Excel, Power BI, Tableau, Tally Prime, Data Analytics, Data Visualization, and Automation.<br><br>⚡ Fun fact<br>I enjoy transforming raw data into meaningful insights and continuously learning new technologies to solve real-world business problems.


## 🌐 Socials:
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/https://www.instagram.com/greentree_333?igsh=MWszcWQwaDg1c2Myeg==) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/https://www.linkedin.com/in/tejayya-hosamath?utm_source=share_via&utm_content=profile&utm_medium=member_android)  [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:tejayyahosamath18@gmail.com)    [![](https://komarev.com/ghpvc/?username=tejayyahosamath18-lang&icon=My&color=yellow)](https://tejayya-m-hosamath-portfolio-1004083300830.asia-southeast1.run.app)

# 💻 Tech Stack:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white) ![SQLite](https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white) ![MicrosoftSQLServer](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white) ![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Google Cloud](https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white) ![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white) ![Teradata](https://img.shields.io/badge/Teradata-F37440?style=for-the-badge&logo=teradata&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Meta](https://img.shields.io/badge/Meta-%230467DF.svg?style=for-the-badge&logo=Meta&logoColor=white)
# 📊 GitHub Stats :
![](https://github-readme-stats.shion.dev/api?username=tejayyahosamath18-lang&theme=dark&hide_border=false&include_all_commits=false&count_private=false)<br/>
![](https://streak-stats.demolab.com/?user=tejayyahosamath18-lang&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.shion.dev/api/top-langs/?username=tejayyahosamath18-lang&theme=dark&hide_border=false&include_all_commits=false&count_private=false&layout=compact)

---
[![](https://komarev.com/ghpvc/?username=tejayyahosamath18-lang&icon=0&color=0)](https://tejayya-m-hosamath-portfolio-1004083300830.asia-southeast1.run.app)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Cinematic Animated Text Intro</title>
    <style>
        /* ── Reset & Base ── */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #0a0a0f;
            overflow: hidden;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
            height: 100vh;
            width: 100vw;
        }

        /* ── Canvas (background) ── */
        #bgCanvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: 0;
        }

        /* ── Scene Container ── */
        #sceneContainer {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: 1;
            display: flex;
            align-items: center;
            justify-content: center;
            pointer-events: none;
        }

        /* ── Scene base ── */
        .scene {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            transition: opacity 1.2s ease-in-out;
            flex-direction: column;
            padding: 2rem;
        }
        .scene.active {
            opacity: 1;
        }
        .scene.exit {
            opacity: 0;
        }

        /* ── Text styling ── */
        .main-text {
            font-size: clamp(2.4rem, 8vw, 6rem);
            font-weight: 700;
            letter-spacing: 0.04em;
            text-align: center;
            color: #fff;
            position: relative;
            line-height: 1.2;
            max-width: 90vw;
            text-shadow:
                0 0 10px rgba(0, 180, 255, 0.3),
                0 0 30px rgba(0, 180, 255, 0.15);
        }

        .sub-text {
            font-size: clamp(1rem, 2.5vw, 2.2rem);
            font-weight: 400;
            letter-spacing: 0.15em;
            text-align: center;
            color: rgba(180, 220, 255, 0.7);
            margin-top: 1.2rem;
            text-shadow: 0 0 20px rgba(0, 150, 255, 0.2);
            opacity: 0.85;
        }

        /* ── Cursor ── */
        .cursor {
            display: inline-block;
            width: 0.08em;
            height: 1.1em;
            background: #00ccff;
            margin-left: 0.04em;
            vertical-align: text-bottom;
            animation: cursorBlink 0.9s step-end infinite;
            box-shadow: 0 0 12px #00ccff, 0 0 24px #00ccff66;
            border-radius: 1px;
        }
        @keyframes cursorBlink {
            0%,
            100% {
                opacity: 1;
            }
            50% {
                opacity: 0;
            }
        }

        /* ── Scene 1 specific ── */
        #scene1 .main-text {
            font-weight: 800;
            background: linear-gradient(135deg, #ffffff 0%, #80d4ff 40%, #a855f7 70%, #f472b6 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            filter: drop-shadow(0 0 40px rgba(0, 180, 255, 0.25));
        }

        /* ── Scene 2 specific ── */
        #scene2 .main-text {
            font-weight: 800;
            background: linear-gradient(135deg, #ffffff 0%, #60a5fa 30%, #8b5cf6 60%, #a78bfa 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            filter: drop-shadow(0 0 50px rgba(96, 165, 250, 0.3));
            text-shadow: none;
        }

        /* ── Glitch overlay (Scene 1) ── */
        .glitch-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 10;
            mix-blend-mode: screen;
            opacity: 0;
            transition: opacity 0.1s;
        }
        .glitch-overlay.active {
            opacity: 0.6;
        }
        .glitch-overlay .glitch-slice {
            position: absolute;
            background: rgba(0, 200, 255, 0.08);
            width: 100%;
            height: 4px;
            left: 0;
            animation: glitchSlice 0.08s infinite alternate;
        }
        @keyframes glitchSlice {
            0% {
                transform: translateX(-2%) skewX(2deg);
                opacity: 0.2;
            }
            100% {
                transform: translateX(2%) skewX(-2deg);
                opacity: 0.8;
            }
        }

        /* ── Scan lines ── */
        .scanlines {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 2;
            background: repeating-linear-gradient(0deg,
                    transparent 0px,
                    transparent 3px,
                    rgba(0, 180, 255, 0.015) 3px,
                    rgba(0, 180, 255, 0.015) 4px);
            animation: scanMove 10s linear infinite;
        }
        @keyframes scanMove {
            0% {
                transform: translateY(0);
            }
            100% {
                transform: translateY(100%);
            }
        }

        /* ── Vignette ── */
        .vignette {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
            background: radial-gradient(ellipse at center, transparent 50%, rgba(0, 0, 0, 0.6) 100%);
        }

        /* ── Scene 1: Typing container ── */
        .typing-container {
            display: flex;
            align-items: center;
            justify-content: center;
            flex-wrap: wrap;
            gap: 0.04em;
        }
        .typing-container .char {
            display: inline-block;
            opacity: 0;
            transform: scale(0.6) rotateX(30deg);
            animation: charReveal 0.35s cubic-bezier(0.34, 1.56, 0.64, 1) forwards;
        }
        @keyframes charReveal {
            0% {
                opacity: 0;
                transform: scale(0.6) rotateX(30deg) translateY(20px);
                filter: blur(4px);
            }
            100% {
                opacity: 1;
                transform: scale(1) rotateX(0) translateY(0);
                filter: blur(0);
            }
        }
        .typing-container .char.glitch-char {
            animation: charGlitch 0.15s ease-in-out 3;
        }
        @keyframes charGlitch {
            0% {
                transform: translate(0, 0) skewX(0);
                opacity: 1;
                filter: blur(0);
            }
            20% {
                transform: translate(-4px, 2px) skewX(6deg);
                opacity: 0.7;
                filter: blur(1px);
                color: #ff00cc;
            }
            40% {
                transform: translate(4px, -2px) skewX(-6deg);
                opacity: 0.7;
                filter: blur(1px);
                color: #00ffcc;
            }
            60% {
                transform: translate(-2px, 4px) skewX(3deg);
                opacity: 0.8;
                filter: blur(0.5px);
                color: #ffcc00;
            }
            80% {
                transform: translate(2px, -4px) skewX(-3deg);
                opacity: 0.8;
                filter: blur(0.5px);
                color: #00ccff;
            }
            100% {
                transform: translate(0, 0) skewX(0);
                opacity: 1;
                filter: blur(0);
            }
        }

        /* ── Energy wave ring ── */
        .energy-ring {
            position: absolute;
            border: 2px solid rgba(0, 200, 255, 0.3);
            border-radius: 50%;
            width: 0;
            height: 0;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            opacity: 0;
            pointer-events: none;
            z-index: 5;
        }
        .energy-ring.active {
            animation: energyRingExpand 1.8s ease-out forwards;
        }
        @keyframes energyRingExpand {
            0% {
                width: 0;
                height: 0;
                opacity: 0.8;
                border-width: 4px;
            }
            100% {
                width: 200vmax;
                height: 200vmax;
                opacity: 0;
                border-width: 1px;
            }
        }

        /* ── Holographic flicker ── */
        .holo-flicker {
            animation: holoFlicker 0.12s ease-in-out 6;
        }
        @keyframes holoFlicker {
            0%,
            100% {
                opacity: 1;
                filter: brightness(1) contrast(1);
            }
            25% {
                opacity: 0.85;
                filter: brightness(1.3) contrast(1.2) hue-rotate(5deg);
            }
            50% {
                opacity: 0.95;
                filter: brightness(0.9) contrast(1.1) hue-rotate(-5deg);
            }
            75% {
                opacity: 0.7;
                filter: brightness(1.5) contrast(1.3) hue-rotate(8deg);
            }
        }

        /* ── Pulse animation ── */
        .pulse-glow {
            animation: pulseGlow 2s ease-in-out infinite;
        }
        @keyframes pulseGlow {
            0%,
            100% {
                filter: drop-shadow(0 0 20px rgba(0, 180, 255, 0.2));
            }
            50% {
                filter: drop-shadow(0 0 60px rgba(0, 180, 255, 0.5)) drop-shadow(0 0 120px rgba(100, 0, 255, 0.2));
            }
        }

        /* ── Metallic shine ── */
        .metallic-shine {
            position: relative;
            overflow: hidden;
        }
        .metallic-shine::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: linear-gradient(135deg,
                    transparent 30%,
                    rgba(255, 255, 255, 0.15) 45%,
                    rgba(255, 255, 255, 0.4) 50%,
                    rgba(255, 255, 255, 0.15) 55%,
                    transparent 70%);
            transform: rotate(25deg) translateX(-100%);
            animation: metallicSweep 3.5s ease-in-out infinite;
            pointer-events: none;
            mix-blend-mode: overlay;
        }
        @keyframes metallicSweep {
            0% {
                transform: rotate(25deg) translateX(-100%);
            }
            100% {
                transform: rotate(25deg) translateX(100%);
            }
        }

        /* ── Scene 2: HUD elements ── */
        .hud-grid {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            opacity: 0.15;
            background-image:
                linear-gradient(rgba(0, 180, 255, 0.05) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 180, 255, 0.05) 1px, transparent 1px);
            background-size: 40px 40px;
            animation: hudGridPulse 4s ease-in-out infinite;
        }
        @keyframes hudGridPulse {
            0%,
            100% {
                opacity: 0.1;
            }
            50% {
                opacity: 0.25;
            }
        }

        .hud-corner {
            position: absolute;
            width: 40px;
            height: 40px;
            border-color: rgba(0, 200, 255, 0.3);
            border-style: solid;
            border-width: 0;
            z-index: 1;
            opacity: 0.5;
        }
        .hud-corner.tl {
            top: 20px;
            left: 20px;
            border-top-width: 2px;
            border-left-width: 2px;
        }
        .hud-corner.tr {
            top: 20px;
            right: 20px;
            border-top-width: 2px;
            border-right-width: 2px;
        }
        .hud-corner.bl {
            bottom: 20px;
            left: 20px;
            border-bottom-width: 2px;
            border-left-width: 2px;
        }
        .hud-corner.br {
            bottom: 20px;
            right: 20px;
            border-bottom-width: 2px;
            border-right-width: 2px;
        }

        /* ── Scene 2: Data tags ── */
        .data-tags {
            position: absolute;
            bottom: 10%;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            gap: clamp(0.6rem, 2vw, 1.8rem);
            flex-wrap: wrap;
            justify-content: center;
            z-index: 2;
            opacity: 0;
            transition: opacity 1.5s ease 2s;
        }
        .data-tags.visible {
            opacity: 1;
        }
        .data-tags span {
            font-size: clamp(0.5rem, 1vw, 0.9rem);
            font-weight: 500;
            letter-spacing: 0.1em;
            color: rgba(150, 210, 255, 0.6);
            background: rgba(0, 40, 80, 0.3);
            padding: 0.3em 1em;
            border-radius: 20px;
            border: 1px solid rgba(0, 180, 255, 0.15);
            backdrop-filter: blur(6px);
            text-transform: uppercase;
            box-shadow: 0 0 20px rgba(0, 100, 255, 0.05);
        }

        /* ── Scene 2: Code rain (Canvas overlay) ── */
        #codeRainCanvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: 0;
            pointer-events: none;
            opacity: 0.08;
        }

        /* ── Responsive ── */
        @media (max-width: 768px) {
            .main-text {
                font-size: clamp(1.6rem, 10vw, 3rem);
            }
            .sub-text {
                font-size: clamp(0.7rem, 3vw, 1.2rem);
            }
            .hud-corner {
                width: 20px;
                height: 20px;
            }
            .data-tags span {
                font-size: 0.5rem;
                padding: 0.2em 0.6em;
            }
        }

        @media (max-width: 480px) {
            .main-text {
                font-size: clamp(1.2rem, 8vw, 2rem);
            }
            .sub-text {
                font-size: clamp(0.6rem, 2.5vw, 0.9rem);
                margin-top: 0.6rem;
            }
        }

        /* ── Utility ── */
        .hidden {
            display: none !important;
        }
        .relative {
            position: relative;
        }
        .flex-center {
            display: flex;
            align-items: center;
            justify-content: center;
        }

        /* ── Scene 2 glass morphism overlay ── */
        .glass-overlay {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 70%;
            max-width: 900px;
            padding: 3rem 4rem;
            background: rgba(10, 20, 40, 0.25);
            backdrop-filter: blur(12px);
            -webkit-backdrop-filter: blur(12px);
            border: 1px solid rgba(0, 180, 255, 0.12);
            border-radius: 32px;
            box-shadow:
                0 0 60px rgba(0, 100, 255, 0.05),
                inset 0 0 60px rgba(0, 180, 255, 0.03);
            z-index: 1;
            opacity: 0;
            transition: opacity 1.8s ease 0.5s;
            pointer-events: none;
        }
        .glass-overlay.visible {
            opacity: 1;
        }

        @media (max-width: 768px) {
            .glass-overlay {
                width: 88%;
                padding: 2rem 1.5rem;
                border-radius: 20px;
            }
        }

        /* ── Floating geometric shapes (CSS) ── */
        .geo-shape {
            position: fixed;
            border-radius: 50%;
            pointer-events: none;
            z-index: 0;
            opacity: 0.06;
            background: radial-gradient(circle, rgba(0, 200, 255, 0.1), transparent 70%);
            animation: geoFloat 20s ease-in-out infinite alternate;
        }
        .geo-shape:nth-child(1) {
            width: 300px;
            height: 300px;
            top: 10%;
            left: -5%;
            animation-delay: 0s;
        }
        .geo-shape:nth-child(2) {
            width: 200px;
            height: 200px;
            bottom: 15%;
            right: -3%;
            animation-delay: -7s;
            background: radial-gradient(circle, rgba(168, 85, 247, 0.08), transparent 70%);
        }
        .geo-shape:nth-child(3) {
            width: 150px;
            height: 150px;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation-delay: -14s;
            background: radial-gradient(circle, rgba(244, 114, 182, 0.06), transparent 70%);
        }
        @keyframes geoFloat {
            0% {
                transform: translate(0, 0) scale(1) rotate(0deg);
            }
            33% {
                transform: translate(30px, -40px) scale(1.1) rotate(120deg);
            }
            66% {
                transform: translate(-20px, 20px) scale(0.9) rotate(240deg);
            }
            100% {
                transform: translate(10px, -10px) scale(1.05) rotate(360deg);
            }
        }

        /* ── Lens flare (CSS) ── */
        .lens-flare {
            position: fixed;
            top: 20%;
            right: 10%;
            width: 200px;
            height: 200px;
            pointer-events: none;
            z-index: 0;
            background: radial-gradient(circle,
                    rgba(0, 200, 255, 0.08) 0%,
                    rgba(100, 0, 255, 0.04) 30%,
                    transparent 70%);
            border-radius: 50%;
            filter: blur(20px);
            animation: lensPulse 8s ease-in-out infinite alternate;
        }
        .lens-flare:nth-child(2) {
            top: 60%;
            left: 5%;
            width: 120px;
            height: 120px;
            animation-delay: -4s;
            background: radial-gradient(circle, rgba(244, 114, 182, 0.06) 0%, transparent 70%);
        }
        @keyframes lensPulse {
            0% {
                transform: scale(1) translate(0, 0);
                opacity: 0.5;
            }
            100% {
                transform: scale(1.5) translate(30px, -20px);
                opacity: 1;
            }
        }

        /* ── Scene transition flash ── */
        .transition-flash {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(ellipse at center, rgba(0, 180, 255, 0.3), rgba(100, 0, 255, 0.1));
            pointer-events: none;
            z-index: 20;
            opacity: 0;
            transition: opacity 0.2s;
        }
        .transition-flash.active {
            opacity: 1;
            transition: opacity 0.05s;
        }

        /* ── Scene 2: Electric outline glow ── */
        .electric-outline {
            position: relative;
        }
        .electric-outline::before {
            content: '';
            position: absolute;
            inset: -6px;
            border: 2px solid rgba(0, 200, 255, 0.2);
            border-radius: 12px;
            filter: blur(4px);
            animation: electricPulse 1.8s ease-in-out infinite;
            pointer-events: none;
        }
        @keyframes electricPulse {
            0%,
            100% {
                opacity: 0.3;
                border-color: rgba(0, 200, 255, 0.2);
                box-shadow: 0 0 20px rgba(0, 200, 255, 0.05);
         
