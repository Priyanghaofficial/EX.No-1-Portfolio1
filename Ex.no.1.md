# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PRIYANGHA G Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700;800&display=swap');
        body {
            font-family: 'Inter', sans-serif;
        }
        .active-link {
            position: relative;
            color: #38bdf8;  
        }
        .active-link::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 3px;
            background-color: #38bdf8; 
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .animate-fade-in-up {
            animation: fadeIn 0.8s ease-out forwards;
        }
    </style>
</head>
<body class="bg-slate-950 text-slate-200">


    <header class="sticky top-0 z-50 bg-slate-900 shadow-xl">
        <nav class="container mx-auto px-6 py-5 flex justify-center space-x-10">
            <a href="#about" class="text-slate-300 hover:text-sky-400 font-semibold transition-colors duration-300">About</a>
            <a href="#skills" class="text-slate-300 hover:text-sky-400 font-semibold transition-colors duration-300">Skills</a>
            <a href="#projects" class="text-slate-300 hover:text-sky-400 font-semibold transition-colors duration-300">Projects</a>
            <a href="#contact" class="text-slate-300 hover:text-sky-400 font-semibold transition-colors duration-300">Contact</a>
        </nav>
    </header>

    <section id="hero" class="bg-sky-950 text-white py-32 md:py-48 flex flex-col items-center justify-center text-center px-4">
        <h1 class="text-5xl md:text-7xl font-extrabold mb-4 animate-fade-in-up">Hi, I'm Priyangha </h1>
        <p class="text-xl md:text-3xl max-w-3xl leading-relaxed text-sky-100 opacity-0 animate-fade-in-up" style="animation-delay: 0.3s;">A dedicated developer with a passion for building beautiful and functional web experiences.</p>
    </section>

    <main class="container mx-auto px-6 py-20 md:py-28">

        <section id="about" class="mb-20 md:mb-32">
            <h2 class="text-3xl md:text-4xl font-extrabold text-sky-400 border-b-4 border-sky-400 pb-2 mb-8 inline-block">About Me</h2>
            <p class="text-lg md:text-xl leading-relaxed text-slate-300">
                I'm Priyangha G , a frontend enthusiast with a strong foundation in core web technologies. My skills in HTML, CSS, and JavaScript allow me to create interactive and visually appealing websites, and my passion for UI/UX design ensures a focus on intuitive user experiences.
            </p>
        </section>

        <section id="skills" class="mb-20 md:mb-32">
            <h2 class="text-3xl md:text-4xl font-extrabold text-sky-400 border-b-4 border-sky-400 pb-2 mb-8 inline-block">Skills</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                <div class="bg-slate-800 p-8 rounded-xl shadow-lg hover:bg-slate-700 transition-colors duration-300">
                    <h3 class="text-xl font-bold text-sky-300 mb-2">Frontend</h3>
                    <p class="text-slate-400">HTML, CSS, JavaScript</p>
                </div>
                <div class="bg-slate-800 p-8 rounded-xl shadow-lg hover:bg-slate-700 transition-colors duration-300">
                    <h3 class="text-xl font-bold text-sky-300 mb-2">Design</h3>
                    <p class="text-slate-400">UI/UX Design</p>
                </div>
                <div class="bg-slate-800 p-8 rounded-xl shadow-lg hover:bg-slate-700 transition-colors duration-300">
                    <h3 class="text-xl font-bold text-sky-300 mb-2">Tools</h3>
                    <p class="text-slate-400">Git</p>
                </div>
                <div class="bg-slate-800 p-8 rounded-xl shadow-lg hover:bg-slate-700 transition-colors duration-300">
                    <h3 class="text-xl font-bold text-sky-300 mb-2">Concepts</h3>
                    <p class="text-slate-400">Responsive Design, Accessibility</p>
                </div>
            </div>
        </section>

        <section id="projects" class="mb-20 md:mb-32">
            <h2 class="text-3xl md:text-4xl font-extrabold text-sky-400 border-b-4 border-sky-400 pb-2 mb-8 inline-block">Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-10">
                <div class="bg-slate-800 p-10 rounded-xl shadow-lg hover:shadow-xl transition-shadow duration-300">
                    <h3 class="text-2xl font-bold text-sky-300 mb-2">Simple To-Do List App</h3>
                    <p class="text-slate-400">A basic web application created with vanilla JavaScript, HTML, and CSS for managing daily tasks and practicing DOM manipulation.</p>
                </div>
                <div class="bg-slate-800 p-10 rounded-xl shadow-lg hover:shadow-xl transition-shadow duration-300">
                    <h3 class="text-2xl font-bold text-sky-300 mb-2">Figma-Styled Hair Care Brand Website</h3>
                    <p class="text-slate-400">A modern, responsive website prototype for a hair care brand, designed in Figma and implemented with HTML, CSS, and Tailwind. The design emphasizes clean layouts, pastel color palettes, and user-friendly product browsing.</p>
                </div>
            </div>
        </section>

        <section id="contact" class="bg-sky-950 text-white p-12 rounded-xl shadow-2xl text-center">
            <h2 class="text-3xl md:text-4xl font-extrabold pb-2 mb-6 inline-block border-b-4 border-sky-400">Get In Touch</h2>
            <p class="text-lg md:text-xl leading-relaxed mb-4">I'm always open to new opportunities and interesting projects. Let's connect!</p>
            <p class="text-lg md:text-xl">Email: <a href="mailto:priyanghaofficial@gmail.com" class="text-sky-300 hover:text-sky-200 transition-colors duration-300 font-medium">priyanghaofficial@gmail.com</a></p>
        </section>

    </main>

    <footer class="bg-slate-900 text-slate-400 text-center py-6 mt-20">
        <p>&copy; 2025 Hemapriya K. All rights reserved.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('nav a');

            const options = {
                root: null, 
                threshold: 0.5 
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        navLinks.forEach(link => link.classList.remove('active-link'));
                        const currentSectionId = entry.target.id;
                        const activeLink = document.querySelector(`nav a[href="#${currentSectionId}"]`);
                        if (activeLink) {
                            activeLink.classList.add('active-link');
                        }
                    }
                });
            }, options);

            sections.forEach(section => {
                observer.observe(section);
            });
        });
    </script>
</body>
</html>

```


## OUTPUT

<img width="1920" height="1080" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/536aa0c2-ac67-4ee4-9e13-026ee2c3878d" />

<img width="1920" height="1080" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/d013ec55-1380-455e-811a-ee38e741bc53" />

<img width="1920" height="1080" alt="Screenshot (52)" src="https://github.com/user-attachments/assets/7ac13d7d-acaf-4888-b864-1e325cb7a3a2" />

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
