<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Student Study Hub | Notes, PDFs, Tools & Learning</title>

    <meta name="description"
          content="Student Study Hub provides useful study notes, PDFs, educational videos, calculators and study tools for students.">

    <meta name="keywords"
          content="Student Study Hub, study notes, PDF notes, diploma notes, electrical engineering, mathematics, physics, computer">

    <meta name="author" content="Student Study Hub">

    <link rel="stylesheet" href="style.css">
</head>

<body>

<header class="header">

    <div class="container nav">

        <a href="index.html" class="logo">
            📚 Student Study Hub
        </a>

        <button class="menu-btn" onclick="toggleMenu()">☰</button>

        <nav id="navMenu">
            <a href="index.html">Home</a>
            <a href="#subjects">Subjects</a>
            <a href="#tools">Tools</a>
            <a href="#videos">Videos</a>
            <a href="about.html">About</a>
            <a href="contact.html">Contact</a>
            <button onclick="toggleDarkMode()" class="dark-btn">🌙</button>
        </nav>

    </div>

</header>


<!-- HERO -->

<section class="hero">

    <div class="container">

        <span class="hero-badge">🎓 Learn • Practice • Improve</span>

        <h1>Student Study Hub</h1>

        <p>
            Notes, PDFs, educational videos and useful study tools
            — all in one place.
        </p>

        <div class="search-box">

            <input
                type="text"
                id="searchInput"
                placeholder="🔍 Search subjects, notes or tools..."
                onkeyup="searchContent()">

        </div>

    </div>

</section>


<!-- QUICK FEATURES -->

<section class="container quick-section">

    <div class="quick-card">
        <span>📚</span>
        <div>
            <strong>Study Notes</strong>
            <small>Easy-to-understand material</small>
        </div>
    </div>

    <div class="quick-card">
        <span>📄</span>
        <div>
            <strong>PDF Resources</strong>
            <small>Download useful PDFs</small>
        </div>
    </div>

    <div class="quick-card">
        <span>🎥</span>
        <div>
            <strong>Learning Videos</strong>
            <small>Learn visually</small>
        </div>
    </div>

    <div class="quick-card">
        <span>🛠️</span>
        <div>
            <strong>Study Tools</strong>
            <small>Useful student utilities</small>
        </div>
    </div>

</section>


<!-- SUBJECTS -->

<section id="subjects" class="section container">

    <div class="section-title">
        <span>📚</span>
        <div>
            <h2>Study Subjects</h2>
            <p>Choose a subject and start learning.</p>
        </div>
    </div>


    <div class="grid" id="subjectGrid">

        <article class="card searchable">

            <div class="card-icon">⚡</div>

            <h3>Electrical Engineering</h3>

            <p>
                Basic electrical engineering notes,
                formulas and study materials.
            </p>

            <div class="card-buttons">
                <a href="pdfs/electrical-engineering.pdf"
                   target="_blank"
                   class="btn purple">
                    👁 View PDF
                </a>

                <a href="pdfs/electrical-engineering.pdf"
                   download
                   class="btn green">
                    📥 Download
                </a>
            </div>

        </article>


        <article class="card searchable">

            <div class="card-icon">📐</div>

            <h3>Mathematics</h3>

            <p>
                Engineering mathematics formulas,
                examples and notes.
            </p>

            <div class="card-buttons">

                <a href="pdfs/mathematics.pdf"
                   target="_blank"
                   class="btn purple">
                    👁 View PDF
                </a>

                <a href="pdfs/mathematics.pdf"
                   download
                   class="btn green">
                    📥 Download
                </a>

            </div>

        </article>


        <article class="card searchable">

            <div class="card-icon">🔬</div>

            <h3>Physics</h3>

            <p>
                Applied Physics concepts,
                formulas and numerical practice.
            </p>

            <div class="card-buttons">

                <a href="pdfs/physics.pdf"
                   target="_blank"
                   class="btn purple">
                    👁 View PDF
                </a>

                <a href="pdfs/physics.pdf"
                   download
                   class="btn green">
                    📥 Download
                </a>

            </div>

        </article>


        <article class="card searchable">

            <div class="card-icon">💻</div>

            <h3>Computer</h3>

            <p>
                Computer fundamentals,
                digital technology and programming.
            </p>

            <div class="card-buttons">

                <a href="pdfs/computer.pdf"
                   target="_blank"
                   class="btn purple">
                    👁 View PDF
                </a>

                <a href="pdfs/computer.pdf"
                   download
                   class="btn green">
                    📥 Download
                </a>

            </div>

        </article>

    </div>

</section>


<!-- TOOLS -->

<section id="tools" class="section container">

    <div class="section-title">
        <span>🛠️</span>
        <div>
            <h2>Student Tools</h2>
            <p>Useful tools for everyday study.</p>
        </div>
    </div>


    <div class="grid tools-grid">


        <!-- CALCULATOR -->

        <div class="card tool-card">

            <h3>🧮 Calculator</h3>

            <input
                type="text"
                id="calcInput"
                placeholder="Example: 25+10*2">

            <div class="tool-buttons">

                <button onclick="calculate()" class="btn blue">
                    Calculate
                </button>

                <button onclick="clearCalculator()" class="btn gray">
                    Clear
                </button>

            </div>

            <div id="calcResult" class="result">
                Result will appear here
            </div>

        </div>


        <!-- TIMER -->

        <div class="card tool-card">

            <h3>⏱️ Study Timer</h3>

            <div id="timer" class="timer">
                25:00
            </div>

            <div class="tool-buttons">

                <button onclick="startTimer()" class="btn blue">
                    ▶ Start
                </button>

                <button onclick="pauseTimer()" class="btn orange">
                    ⏸ Pause
                </button>

                <button onclick="resetTimer()" class="btn gray">
                    ↻ Reset
                </button>

            </div>

        </div>


        <!-- DARK MODE -->

        <div class="card tool-card">

            <h3>🌙 Dark Mode</h3>

            <p>
                Change the website appearance
                for comfortable studying.
            </p>

            <button onclick="toggleDarkMode()" class="btn blue">
                🌙 Toggle Theme
            </button>

        </div>

    </div>

</section>


<!-- VIDEOS -->

<section id="videos" class="section container">

    <div class="section-title">
        <span>🎥</span>
        <div>
            <h2>Learning Videos</h2>
            <p>Educational videos for students.</p>
        </div>
    </div>


    <div class="video-grid">

        <div class="video-card">

            <div class="video-wrapper">

                <iframe
                    src="https://www.youtube.com/embed/VIDEO_ID_1"
                    title="Educational Video"
                    allowfullscreen>
                </iframe>

            </div>

            <h3>Electrical Engineering Basics</h3>

            <p>
                Learn basic electrical engineering concepts.
            </p>

        </div>


        <div class="video-card">

            <div class="video-wrapper">

                <iframe
                    src="https://www.youtube.com/embed/VIDEO_ID_2"
                    title="Mathematics Video"
                    allowfullscreen>
                </iframe>

            </div>

            <h3>Engineering Mathematics</h3>

            <p>
                Important formulas and concepts.
            </p>

        </div>


        <div class="video-card">

            <div class="video-wrapper">

                <iframe
                    src="https://www.youtube.com/embed/VIDEO_ID_3"
                    title="Physics Video"
                    allowfullscreen>
                </iframe>

            </div>

            <h3>Applied Physics</h3>

            <p>
                Understand physics with examples.
            </p>

        </div>

    </div>

</section>


<!-- WHY US -->

<section class="why-section">

    <div class="container">

        <div class="section-title">
            <span>⭐</span>
            <div>
                <h2>Why Student Study Hub?</h2>
                <p>Designed to make learning easier.</p>
            </div>
        </div>


        <div class="features">

            <div>
                <span>📱</span>
                <h3>Mobile Friendly</h3>
                <p>Study comfortably from your phone.</p>
            </div>

            <div>
                <span>🎯</span>
                <h3>Simple Learning</h3>
                <p>Easy and student-friendly resources.</p>
            </div>

            <div>
                <span>⚡</span>
                <h3>Useful Tools</h3>
                <p>Calculator, timer and other study utilities.</p>
            </div>

        </div>

    </div>

</section>


<!-- ABOUT PREVIEW -->

<section class="container about-preview">

    <h2>ℹ️ About Student Study Hub</h2>

    <p>
        Student Study Hub is an educational platform created
        to provide students with useful study resources,
        notes, PDFs, educational videos and study tools
        in one convenient place.
    </p>

    <a href="about.html" class="btn blue">
        Learn More →
    </a>

</section>


<!-- FOOTER -->

<footer>

    <div class="container footer-grid">

        <div>
            <h3>📚 Student Study Hub</h3>

            <p>
                Learn • Practice • Improve
            </p>
        </div>


        <div>

            <h4>Quick Links</h4>

            <a href="index.html">Home</a>
            <a href="about.html">About</a>
            <a href="contact.html">Contact</a>

        </div>


        <div>

            <h4>Legal</h4>

            <a href="privacy.html">Privacy Policy</a>
            <a href="terms.html">Terms & Conditions</a>

        </div>

    </div>


    <div class="copyright">

        © 2026 Student Study Hub.
        All rights reserved.

    </div>

</footer>


<script src="script.js"></script>

</body>
</html>
