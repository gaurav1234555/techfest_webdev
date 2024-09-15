<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Website</title>
    <style>
        /* General Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #333;
            color: white;
            padding: 15px;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
        }

        /* Section Styles */
        .section {
            display: none;
            padding: 20px;
        }

        .active {
            display: block;
        }

        h1 {
            font-size: 2em;
            margin-bottom: 10px;
        }

        ul {
            padding-left: 20px;
        }

        ul li {
            margin-bottom: 10px;
        }

        a {
            color: #3498db;
            text-decoration: none;
        }

        a:hover {
            text-decoration: underline;
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            nav ul li {
                display: block;
                margin-bottom: 10px;
            }

            h1 {
                font-size: 1.5em;
            }
        }
    </style>
</head>
<body>

    <!-- Header and Navigation -->
    <header>
        <nav>
            <ul>
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('achievements')">Achievements</a></li>
                <li><a href="#" onclick="showSection('projects')">Projects</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="section active">
        <h1>Hello! I'm [Your Name]</h1>
        <p>Welcome to my personal website. Explore my achievements, current work, and past projects.</p>
    </section>

    <!-- Achievements Section -->
    <section id="achievements" class="section">
        <h1>Achievements</h1>
        <ul>
            <li><strong>XYZ Hackathon Winner:</strong> Won the XYZ Hackathon in [Year].</li>
            <li><strong>Published Research Paper:</strong> Published a research paper on ABC in [Year].</li>
            <li><strong>Dean's List:</strong> Achieved top academic performance in [Year].</li>
        </ul>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="section">
        <h1>Projects</h1>
        <ul>
            <li><strong>Room Allocation Web App:</strong> A tool to efficiently allocate rooms in hostels based on group ID, gender, and capacity. <a href="#">View Demo</a></li>
            <li><strong>E-commerce Website:</strong> An online platform for selling products with integrated payment gateway. <a href="#">View Demo</a></li>
            <li><strong>Personal Portfolio:</strong> A responsive portfolio website showcasing my work. <a href="#">View Demo</a></li>
        </ul>
    </section>

    <!-- JavaScript for Navigation -->
    <script>
        function showSection(sectionId) {
            var sections = document.querySelectorAll('.section');
            sections.forEach(function(section) {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
        }
    </script>

</body>
</html>
