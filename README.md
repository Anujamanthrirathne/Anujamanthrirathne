<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Interactive Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.0.3/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/aos@2.3.1/dist/aos.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/gsap@3.8.0/dist/gsap.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/lottie-web@5.7.6/build/player/lottie.min.js"></script>
</head>
<body class="bg-gray-900 text-white">
    <!-- Hero Section with Lottie Animation -->
    <section class="h-screen flex justify-center items-center bg-cover bg-center relative">
        <div class="absolute inset-0 bg-black opacity-50"></div>
        <div class="z-10 text-center">
            <h1 class="text-5xl font-bold mb-4">Hi, I'm Anuja Manthrirathna</h1>
            <p class="text-xl">Passionate Full-Stack Developer</p>
            <button class="mt-6 px-6 py-3 bg-blue-500 hover:bg-blue-700 rounded-full" data-aos="zoom-in">View My Work</button>
        </div>
        <div id="lottie" class="absolute bottom-0 left-0 right-0"></div>
    </section>

    <!-- Projects Section with Scroll-trigger Animations -->
    <section id="projects" class="py-20">
        <div class="container mx-auto text-center">
            <h2 class="text-3xl font-bold mb-6" data-aos="fade-up">My Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div class="project-card" data-aos="flip-left">
                    <img src="project-image.jpg" alt="Project 1" class="w-full h-40 object-cover rounded-lg">
                    <h3 class="mt-4 text-xl">Project 1</h3>
                    <p class="text-gray-400">Description of the project.</p>
                </div>
                <!-- Repeat for more projects -->
            </div>
        </div>
    </section>

    <!-- Contact Form -->
    <section id="contact" class="py-20 bg-gray-800">
        <div class="container mx-auto text-center">
            <h2 class="text-3xl font-bold mb-6" data-aos="fade-up">Contact Me</h2>
            <form action="#" method="post">
                <input type="text" name="name" placeholder="Your Name" class="input-field" required>
                <input type="email" name="email" placeholder="Your Email" class="input-field" required>
                <textarea name="message" placeholder="Your Message" class="input-field" required></textarea>
                <button type="submit" class="mt-4 px-6 py-3 bg-green-500 hover:bg-green-700 rounded-full">Send Message</button>
            </form>
        </div>
    </section>

    <script>
        AOS.init(); // Initialize AOS library for scroll animations
        var animation = lottie.loadAnimation({
            container: document.getElementById('lottie'),
            path: 'https://assets7.lottiefiles.com/packages/lf20_5zw88c3b.json', // Example Lottie JSON file
            renderer: 'svg',
            loop: true,
            autoplay: true
        });
    </script>
</body>
</html>
