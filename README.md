<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Evans Kipsang | Portfolio</title>
    <style>
        /* ========== GLOBAL STYLES ========== */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: "Poppins", sans-serif;
        }

        body {
            background: linear-gradient(120deg, #1a1a2e, #16213e);
            color: #fff;
            min-height: 100vh;
            line-height: 1.6;
        }

        header {
            background: rgba(0, 0, 0, 0.3);
            padding: 1.5rem 0;
            text-align: center;
        }

        header h1 {
            font-size: 2rem;
            letter-spacing: 1px;
            color: #00adb5;
        }

        header p {
            color: #aaa;
            font-size: 1rem;
        }

        nav {
            margin-top: 1rem;
        }

        nav a {
            color: #eee;
            text-decoration: none;
            margin: 0 10px;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #00adb5;
        }

        /* ========== MAIN SECTIONS ========== */
        section {
            max-width: 900px;
            margin: 3rem auto;
            background: rgba(255, 255, 255, 0.05);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 0 10px rgba(0,0,0,0.3);
        }

        h2 {
            color: #00adb5;
            margin-bottom: 1rem;
            border-bottom: 2px solid #00adb5;
            display: inline-block;
            padding-bottom: 5px;
        }

        .about p {
            margin-top: 1rem;
            color: #ddd;
        }

        .skills ul {
            list-style: none;
            margin-top: 1rem;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            gap: 0.8rem;
        }

        .skills li {
            background: #0f3460;
            padding: 0.8rem;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s;
        }

        .skills li:hover {
            transform: scale(1.05);
        }

        .projects .project {
            background: #0f3460;
            padding: 1rem;
            margin: 1rem 0;
            border-radius: 10px;
        }

        .projects .project h3 {
            color: #00adb5;
        }

        .projects .project p {
            color: #ccc;
            margin-top: 0.5rem;
        }

        .contact {
            text-align: center;
        }

        .contact a {
            display: inline-block;
            background: #00adb5;
            color: #fff;
            padding: 0.7rem 1.5rem;
            border-radius: 25px;
            margin-top: 1rem;
            text-decoration: none;
            transition: background 0.3s;
        }

        .contact a:hover {
            background: #08d9d6;
        }

        footer {
            text-align: center;
            padding: 1.5rem 0;
            color: #aaa;
            background: rgba(0,0,0,0.3);
            margin-top: 3rem;
        }

        footer a {
            color: #00adb5;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>Evans Kipsang</h1>
        <p>Mathematics & Computer Science Graduate | Web Developer | ICT Trainer</p>
        <nav>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="about" class="about">
        <h2>About Me</h2>
        <p>
            I am a dedicated and detail-oriented Mathematics and Computer Science graduate from Kirinyaga University. 
            Currently attached at Chepsirei Technical College, I have developed a strong foundation in web development, programming, 
            and ICT training. I am passionate about using technology to solve real-world problems and empower others through digital learning.
        </p>
    </section>

    <section id="skills" class="skills">
        <h2>Skills</h2>
        <ul>
            <li>HTML & CSS</li>
            <li>PHP & MySQL</li>
            <li>JavaScript</li>
            <li>Python (Basics)</li>
            <li>Database Design</li>
            <li>ICT Training</li>
            <li>Networking Fundamentals</li>
            <li>Microsoft Office Suite</li>
        </ul>
    </section>

    <section id="projects" class="projects">
        <h2>Projects</h2>

        <div class="project">
            <h3>Online Learning Platform</h3>
            <p>Developed a PHP-based online learning system that allows students to register, log in, access study materials, and track learning progress.</p>
        </div>

        <div class="project">
            <h3>Resource Management System</h3>
            <p>Created an administrative system for uploading, managing, and downloading educational materials efficiently through a database-driven interface.</p>
        </div>

        <div class="project">
            <h3>Personal Portfolio Website</h3>
            <p>This portfolio website, hosted on GitHub Pages, showcases my technical and teaching skills, demonstrating my capability in both design and web development.</p>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact</h2>
        <p>Feel free to reach out for collaborations, job opportunities, or inquiries.</p>
        <a href="mailto:evansrotich269@gmail.com">Contact Me</a>
    </section>

    <footer>
        <p>&copy; 2025 Evans Kipsang | <a href="https://github.com/evanskipsang" target="_blank">GitHub</a> | Designed with ❤️ in Kenya</p>
    </footer>
</body>
</html>
