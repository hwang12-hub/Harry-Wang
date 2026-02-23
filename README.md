<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Harry Wang</title>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

<style>
body {
    margin: 0;
    font-family: 'Inter', sans-serif;
    background: #f8f9fb;
    color: #111;
    line-height: 1.6;
}

.container {
    max-width: 900px;
    margin: auto;
    padding: 80px 20px;
}

.hero {
    text-align: center;
    padding: 120px 20px 80px 20px;
    background: linear-gradient(135deg, #1f2937, #111827);
    color: white;
}

.hero h1 {
    font-size: 56px;
    margin: 0;
    font-weight: 700;
    letter-spacing: -1px;
}

.hero p {
    margin-top: 15px;
    font-size: 18px;
    opacity: 0.85;
}

.section {
    margin-bottom: 80px;
}

.section h2 {
    font-size: 28px;
    margin-bottom: 20px;
    font-weight: 600;
}

.card {
    background: white;
    padding: 40px;
    border-radius: 16px;
    box-shadow: 0 20px 40px rgba(0,0,0,0.05);
}

ul {
    padding-left: 20px;
}

li {
    margin-bottom: 15px;
}

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
    max-height: 500px;
    margin-top: 20px;
}

footer {
    text-align: center;
    padding: 40px;
    font-size: 14px;
    color: #666;
}
</style>
</head>

<body>

<div class="hero">
    <h1>Harry Wang</h1>
    <p>Entrepreneur | Founder | Community Builder</p>
</div>

<div class="container">

    <!-- About Section -->
    <div class="section">
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

    <!-- Projects Section -->
    <div class="section">
        <h2>Projects</h2>
        <div class="card">
            <ul>
                <li>Founder, Music School (150+ students in drums & guitar)</li>
                <li>Founder, Equestrian Club</li>
                <li>Entrepreneurship & Community Development</li>
            </ul>
        </div>
    </div>

    <!-- Proof Section -->
    <div class="section">
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

    <!-- Interactive Section -->
    <div class="section">
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

</div>

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
