<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Harry Wang</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>

/* =========================
   DESIGN SYSTEM
========================= */

:root {
    --bg: #f9fafb;
    --surface: #ffffff;
    --text-primary: #0f172a;
    --text-secondary: #64748b;
    --accent: #1e293b;
    --radius: 16px;
}

/* Typography Scale */
h1 { font-size: 64px; font-weight: 700; letter-spacing: -1px; }
h2 { font-size: 32px; font-weight: 600; }
p  { font-size: 18px; }
small { font-size: 14px; color: var(--text-secondary); }

/* Layout System */
body {
    margin: 0;
    font-family: 'Inter', sans-serif;
    background: var(--bg);
    color: var(--text-primary);
    line-height: 1.7;
}

.section {
    padding: 120px 24px;
}

.container {
    max-width: 900px;
    margin: 0 auto;
}

/* Hero */
.hero {
    background: var(--accent);
    color: white;
    text-align: center;
    padding: 160px 24px 120px 24px;
}

.hero p {
    margin-top: 16px;
    font-size: 20px;
    opacity: 0.85;
}

/* Card */
.card {
    background: var(--surface);
    padding: 48px;
    border-radius: var(--radius);
    box-shadow: 0 30px 60px rgba(0,0,0,0.06);
    transition: transform 0.3s ease;
}

.card:hover {
    transform: translateY(-6px);
}

/* Lists */
ul {
    padding-left: 20px;
}

li {
    margin-bottom: 16px;
    font-size: 18px;
}

/* Interactive */
.interactive-heading {
    cursor: pointer;
    transition: opacity 0.3s ease;
}

.interactive-heading:hover {
    opacity: 0.6;
}

.hidden-content {
    max-height: 0;
    overflow: hidden;
    transition: max-height 0.5s ease;
}

.hidden-content.open {
    max-height: 700px;
    margin-top: 32px;
}

/* Footer */
footer {
    text-align: center;
    padding: 80px 24px;
    color: var(--text-secondary);
    font-size: 14px;
}

/* Button System (future ready) */
.button {
    display: inline-block;
    padding: 14px 28px;
    background: var(--accent);
    color: white;
    border-radius: 12px;
    text-decoration: none;
    font-weight: 500;
    transition: all 0.3s ease;
}

.button:hover {
    opacity: 0.85;
    transform: translateY(-2px);
}

</style>
</head>

<body>

<!-- HERO -->
<section class="hero">
    <div class="container">
        <h1>Harry Wang</h1>
        <p>Entrepreneur | Founder | Community Builder</p>
    </div>
</section>

<!-- ABOUT -->
<section class="section">
    <div class="container">
        <h2>About Me</h2>
        <div class="card">
            <p>
                I am an entrepreneur who started my first company as a freshman in college.
                What began as a small idea has grown into a music school with over 150 students
                learning drums and guitar.
            </p>
            <p>
                Growing up, I faced difficulty communicating with my father. That experience
                shaped how I think about leadership and community. I believe structured shared
                experiences can help families connect in deeper ways.
            </p>
            <p>
                Last year, I founded an Equestrian Club focused not only on riding skills,
                but also on resilience education and strengthening the parent-child relationship.
            </p>
        </div>
    </div>
</section>

<!-- PROJECTS -->
<section class="section">
    <div class="container">
        <h2>Projects</h2>
        <div class="card">
            <ul>
                <li>Founder, Music School (150+ students in drums & guitar)</li>
                <li>Founder, Equestrian Club</li>
                <li>Entrepreneurship & Community Development</li>
            </ul>
        </div>
    </div>
</section>

<!-- PROOF -->
<section class="section">
    <div class="container">
        <h2>Why Trust This?</h2>
        <div class="card">
            <ul>
                <li>
                    <strong>Proven Community Builder:</strong> I founded a music school that has grown to over 150 students. 
                    Sustained growth at that scale shows families trust the environment and the results.
                </li>
                <li>
                    <strong>Real Parent–Child Impact:</strong> Through both my music school and equestrian club, 
                    I have seen parents better understand their children — not only their talents, 
                    but also their struggles. Being a kid is not always sunshine and rainbows.
                </li>
                <li>
                    <strong>Intentional Growth Design:</strong> My programs combine equestrian training, 
                    resilience education, and structured shared experiences that create space for 
                    conversation, reflection, and long-term character development.
                </li>
            </ul>
        </div>
    </div>
</section>

<!-- INTERACTIVE -->
<section class="section">
    <div class="container">
        <h2 class="interactive-heading" onclick="toggleContent()">
            What I Care About Right Now
        </h2>

        <div id="careContent" class="hidden-content">
            <div class="card">
                <p>
                    Right now, I am exploring how structured activities like music and horseback riding
                    can improve communication between kids and parents.
                </p>
                <p>
                    I am especially interested in how resilience education and shared challenges
                    can strengthen family relationships while building real skill.
                </p>
                <p>
                    I believe there is an edge in designing community spaces that feel like home,
                    while still building discipline and long-term growth. If you care about youth
                    development, family connection, and meaningful offline experiences,
                    my work may be worth following.
                </p>
            </div>
        </div>
    </div>
</section>

<footer>
    © 2026 Harry Wang
</footer>

<script>
function toggleContent() {
    const content = document.getElementById("careContent");
    content.classList.toggle("open");
}
</script>

</body>
</html>
