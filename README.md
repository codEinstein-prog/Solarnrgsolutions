<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Solar Company | Renewable Energy Solutions</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/@phosphor-icons/web"></script>
    <style>
        .animate-bg {
            background: linear-gradient(45deg, #ffbb00, #ff7700, #ffbb00);
            background-size: 200% 200%;
            animation: gradientBG 5s infinite alternate;
        }
        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            100% { background-position: 100% 50%; }
        }
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeIn 1s forwards;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>

    <!-- CSS Animations -->
    <style>
        .workflow-step {
            opacity: 0;
            transform: translateY(30px);
            animation: fadeInUp 1s forwards;
            transition: transform 0.3s ease-in-out;
        }

        .workflow-step:hover {
            transform: scale(1.05);
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body class="bg-gray-100 text-gray-900 dark:bg-gray-900 dark:text-white">
    
    <!-- Navbar -->
    <nav class="bg-white dark:bg-gray-800 shadow-md p-4 flex justify-between items-center fixed w-full top-0 z-50">
        <h1 class="text-2xl font-bold text-yellow-500 flex items-center">
            <i class="ph ph-sun text-yellow-500 mr-2"></i> SolarNRG Solutions
        </h1>
        <ul class="hidden md:flex space-x-6 text-gray-800 dark:text-white">
            <li><a href="#home" class="nav-link hover:text-yellow-500 transition-colors">Home</a></li>
            <li><a href="#about" class="nav-link hover:text-yellow-500 transition-colors">About</a></li>
            <li><a href="#projects" class="nav-link hover:text-yellow-500 transition-colors">Projects</a></li>
            <li><a href="#services" class="nav-link hover:text-yellow-500 transition-colors">Services</a></li>
            <li><a href="#contact" class="nav-link hover:text-yellow-500 transition-colors">Contact</a></li>
        </ul>
        <button id="darkModeToggle" class="bg-gray-200 dark:bg-gray-600 px-3 py-1 rounded">🌙</button>
    </nav>

    
    <!-- Hero Section -->
    <section id="home" class="animate-bg text-white py-20 text-center fade-in">
        <h2 class="text-5xl font-bold">Power Your Home with Clean Energy</h2>
        <p class="mt-4 text-lg">Join the solar revolution today and save on electricity bills.</p>
        <a href="upload-utility-bill.html" class="mt-6 bg-white text-yellow-500 px-6 py-2 rounded-lg text-lg font-semibold shadow-lg inline-block hover:scale-105 transition-transform">Get a Free Quote</a>
    </section>
    
    <!-- Slideshow of Previous Projects -->
    <section id="projects" class="py-16 text-center fade-in">
        <h3 class="text-3xl font-bold mb-8">Our Previous Projects</h3>
        <div class="relative w-full max-w-4xl mx-auto">
            <div id="slideshow" class="relative w-full overflow-hidden rounded-lg shadow-lg">
                <img id="slideImage" class="w-full h-96 object-cover" src="" alt="Solar Project">
            </div>
        </div>
    </section>
    
    <!-- Services with Images from Instagram -->
    <section id="services" class="py-16 px-6 text-center fade-in">
        <h3 class="text-3xl font-bold mb-8">Our Services</h3>
        <div class="grid md:grid-cols-3 gap-8">
            <div class="p-6 bg-white dark:bg-gray-800 shadow-md rounded-lg">
                <img class="w-full h-48 object-cover rounded-lg" id="service1" src="" alt="Solar Panel Installation">
                <h4 class="text-xl font-semibold mt-4 flex items-center justify-center"><i class="ph ph-solar-panel text-yellow-500 mr-2"></i> Solar Panel Installation</h4>
                <p class="mt-2">Efficient and affordable solar panel setup for homes and businesses.</p>
            </div>
            <div class="p-6 bg-white dark:bg-gray-800 shadow-md rounded-lg">
                <img class="w-full h-48 object-cover rounded-lg" id="service2" src="" alt="Battery Storage Solutions">
                <h4 class="text-xl font-semibold mt-4 flex items-center justify-center"><i class="ph ph-battery-full text-yellow-500 mr-2"></i> Battery Storage Solutions</h4>
                <p class="mt-2">Store excess energy and use it when needed.</p>
            </div>
            <div class="p-6 bg-white dark:bg-gray-800 shadow-md rounded-lg">
                <img class="w-full h-48 object-cover rounded-lg" id="service3" src="" alt="Maintenance & Support">
                <h4 class="text-xl font-semibold mt-4 flex items-center justify-center"><i class="ph ph-tools text-yellow-500 mr-2"></i><i class="ph ph-user text-yellow-500 mr-2"></i> Maintenance & Support</h4>
                <p class="mt-2">We provide long-term maintenance for solar systems.</p>
            </div>
        </div>
    </section>

    <!-- Project Workflow Section -->
    <section id="workflow" class="py-20 px-6 bg-gray-100 dark:bg-gray-900 fade-in">
        <h2 class="text-4xl font-bold text-center text-yellow-500 mb-12">Our Project Workflow</h2>

        <div class="space-y-16">
            <!-- Step 1: Consultation (Left) -->
            <div class="flex flex-col md:flex-row items-center md:items-start">
                <img src="https://i.pinimg.com/736x/03/c6/23/03c62358cdef785b96094bfd4ee1c9e0.jpg" alt="Consultation"
                    class="w-full md:w-1/3 rounded-lg shadow-lg">
                <div class="md:w-2/3 md:pl-8 text-center md:text-left">
                    <h3 class="text-2xl font-semibold text-yellow-500">Consultation</h3>
                    <p class="mt-2 text-gray-700 dark:text-gray-300">We analyze your energy needs and provide customized solar solutions.</p>
            </div>
        </div>

        <!-- Step 2: Design & Planning (Right) -->
        <div class="flex flex-col md:flex-row-reverse items-center md:items-start">
            <img src="https://i.pinimg.com/736x/03/c6/23/03c62358cdef785b96094bfd4ee1c9e0.jpg" alt="Design & Planning"
                class="w-full md:w-1/3 rounded-lg shadow-lg">
            <div class="md:w-2/3 md:pr-8 text-center md:text-left">
                <h3 class="text-2xl font-semibold text-yellow-500">Design & Planning</h3>
                <p class="mt-2 text-gray-700 dark:text-gray-300">Our team creates a tailored system layout for optimal efficiency.</p>
            </div>
        </div>

        <!-- Step 3: Installation (Center) -->
        <div class="flex flex-col items-center text-center">
            <img src="https://i.pinimg.com/736x/03/c6/23/03c62358cdef785b96094bfd4ee1c9e0.jpg" alt="Installation"
                class="w-full md:w-1/2 rounded-lg shadow-lg">
            <h3 class="text-2xl font-semibold text-yellow-500 mt-4">Installation</h3>
            <p class="mt-2 text-gray-700 dark:text-gray-300">Certified experts install your solar panels quickly and efficiently.</p>
        </div>

        <!-- Step 4: Inspection & Testing (Left) -->
        <div class="flex flex-col md:flex-row items-center md:items-start">
            <img src="https://i.pinimg.com/736x/03/c6/23/03c62358cdef785b96094bfd4ee1c9e0.jpg" alt="Inspection & Testing"
                class="w-full md:w-1/3 rounded-lg shadow-lg">
            <div class="md:w-2/3 md:pl-8 text-center md:text-left">
                <h3 class="text-2xl font-semibold text-yellow-500">Inspection & Testing</h3>
                <p class="mt-2 text-gray-700 dark:text-gray-300">We ensure the system is working optimally before handover.</p>
            </div>
        </div>

        <!-- Step 5: Activation (Right) -->
        <div class="flex flex-col md:flex-row-reverse items-center md:items-start">
            <img src="https://i.pinimg.com/736x/03/c6/23/03c62358cdef785b96094bfd4ee1c9e0.jpg" alt="Activation"
                class="w-full md:w-1/3 rounded-lg shadow-lg">
            <div class="md:w-2/3 md:pr-8 text-center md:text-left">
                <h3 class="text-2xl font-semibold text-yellow-500">Activation</h3>
                <p class="mt-2 text-gray-700 dark:text-gray-300">Your solar system goes live, reducing your energy costs immediately.</p>
            </div>
        </div>

        <!-- Step 6: Maintenance & Support (Center) -->
        <div class="flex flex-col items-center text-center">
            <img src="https://i.pinimg.com/736x/03/c6/23/03c62358cdef785b96094bfd4ee1c9e0.jpg" alt="Maintenance & Support"
                class="w-full md:w-1/2 rounded-lg shadow-lg">
            <h3 class="text-2xl font-semibold text-yellow-500 mt-4">Maintenance & Support</h3>
            <p class="mt-2 text-gray-700 dark:text-gray-300">We provide long-term support to ensure your system runs smoothly.</p>
        </div>
    </div>
    </section>



    <!-- About Us Section -->
    <section id="about" class="py-20 px-6 text-center bg-gray-100 dark:bg-gray-900 fade-in">
        <div class="max-w-4xl mx-auto">
            <h2 class="text-4xl font-bold text-yellow-500 mb-6">About Us</h2>
            <p class="text-lg text-gray-700 dark:text-gray-300">
                SolarNRG Solutions is dedicated to providing clean, renewable energy solutions for homes and businesses.
                Our mission is to reduce carbon footprints while helping customers save on electricity costs.
            </p>
            <div class="mt-6 flex justify-center">
                <a href="#contact" class="bg-yellow-500 text-white px-6 py-3 rounded-lg shadow-lg text-lg font-semibold hover:bg-yellow-600 transition">Get in Touch</a>
            </div>
        </div>
    </section>

    
    <!-- Footer Section -->
    <footer class="bg-gray-800 text-gray-300 py-12 mt-16">
        <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 md:grid-cols-3 gap-12">
            
            <!-- Contact Section -->
            <div>
                <h3 class="text-xl font-semibold text-white mb-4">Contact Us</h3>
                <p class="flex items-center gap-2"><i class="ph ph-envelope text-yellow-500"></i> info@dacrew.com</p>
                <p class="flex items-center gap-2"><i class="ph ph-phone text-yellow-500"></i> +123 456 7890</p>
                <p class="flex items-center gap-2"><i class="ph ph-map-pin text-yellow-500"></i> 123 Street, City, Country</p>
            </div>
    
            <!-- Latest Post Section -->
            <div class="text-center">
                <h3 class="text-xl font-semibold text-white mb-4">Latest Post</h3>
                <div class="relative w-full h-40 bg-gray-700 rounded-lg overflow-hidden shadow-lg">
                    <a href="https://www.instagram.com/p/YOUR_POST_LINK" target="_blank">
                        <img src="https://www.instagram.com/p/YOUR_POST_IMAGE.jpg" 
                            alt="Latest Instagram Post" 
                            class="w-full h-full object-cover hover:opacity-80 transition-opacity">
                    </a>
                </div>
            </div>
    
            <!-- Quick Links -->
            <div class="text-right">
                <h3 class="text-xl font-semibold text-white mb-4">Quick Links</h3>
                <ul class="space-y-2">
                    <li><a href="/faq" class="hover:text-yellow-500 transition-colors">FAQ</a></li>
                    
                    <li><a href="/terms" class="hover:text-yellow-500 transition-colors">Terms & Conditions</a></li>
                    <li><a href="/privacy-policy" class="hover:text-yellow-500 transition-colors">Privacy Policy</a></li>
                    <li><a href="/refunds" class="hover:text-yellow-500 transition-colors">Refunds & Returns</a></li>
                </ul>
            </div>
    
        </div>
    
        <!-- Footer Bottom Bar -->
        <div class="border-t border-gray-700 mt-8 pt-6 text-center text-sm">
            <p>&copy; 2025 SolarNRG Solutions. All rights reserved.</p>
        </div>
    </footer>
    
    
    <!-- JavaScript to Fetch Images from Instagram and Handle Slideshow -->
        <script>
            const animatebg = document.querySelector('.animate-bg');

            animatebg.addEventListener('mouseover', () => {
                // Transition to an image on hover
                animatebg.style.background = 'url("https://via.placeholder.com/800x600?text=Solar+Energy") center/cover no-repeat';
                animatebg.style.backgroundSize = 'cover'; // Ensures the image covers the element
                animatebg.style.animation = ''; // Remove gradient animation on hover
                animatebg.style.transition = 'background 0.5s ease-in-out'; // Smooth transition
            });

            animatebg.addEventListener('mouseout', () => {
                // Reset back to gradient when mouse leaves
                animatebg.style.background = 'linear-gradient(45deg, #ffbb00, #ff7700, #ffbb00)';
                animatebg.style.animation = 'gradientBG 5s infinite alternate'; // Restore gradient animation
            });
        </script>

    <script>
        const instagramImages = [
            'https://via.placeholder.com/800x600?text=Solar+Project+1',
            'https://via.placeholder.com/800x600?text=Solar+Project+2',
            'https://via.placeholder.com/800x600?text=Solar+Project+3'
        ];
        
        let slideIndex = 0;
        function changeSlide() {
            document.getElementById('slideImage').src = instagramImages[slideIndex];
            slideIndex = (slideIndex + 1) % instagramImages.length;
        }
        setInterval(changeSlide, 3000);
        changeSlide();

        document.getElementById('service1').src = instagramImages[0];
        document.getElementById('service2').src = instagramImages[1];
        document.getElementById('service3').src = instagramImages[2];
    </script>

    <!-- JavaScript to Trigger Animation on Scroll -->
    <script>
        document.addEventListener("DOMContentLoaded", function() {
            const steps = document.querySelectorAll(".workflow-step");

            function revealOnScroll() {
                const triggerBottom = window.innerHeight * 0.85;

                steps.forEach((step) => {
                    const stepTop = step.getBoundingClientRect().top;
                    if (stepTop < triggerBottom) {
                        step.style.animationPlayState = "running";
                    }
                });
            }

            window.addEventListener("scroll", revealOnScroll);
            revealOnScroll(); // Trigger on page load
        });
    </script>

    <script>
        document.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                const target = document.querySelector(link.getAttribute('href'));
                target.scrollIntoView({ behavior: 'smooth' });
            });
        });
    </script>
    
    <script>
        const INSTAGRAM_ACCESS_TOKEN = 'YOUR_ACCESS_TOKEN_HERE';
        const INSTAGRAM_API_URL = `https://graph.instagram.com/me/media?fields=id,media_type,media_url,permalink&access_token=${INSTAGRAM_ACCESS_TOKEN}`;
        
        async function fetchInstagramImages() {
            try {
                const response = await fetch(INSTAGRAM_API_URL);
                const data = await response.json();
                
                // Filter only images
                const images = data.data.filter(item => item.media_type === 'IMAGE').map(item => item.media_url);
                
                if (images.length > 0) {
                    updateHeroBackground(images[0]);  // Hero section background
                    updateSlideshow(images);
                    updateServices(images);
                    updateProjectWorkflow(images);
                }
            } catch (error) {
                console.error('Error fetching Instagram images:', error);
            }
        }
        
        // 🔹 Hero Section Background
        function updateHeroBackground(imageUrl) {
            const heroSection = document.querySelector('.animate-bg');
            heroSection.style.background = `url("${imageUrl}") center/cover no-repeat`;
        }
        
        // 🔹 Slideshow
        function updateSlideshow(images) {
            let slideIndex = 0;
            const slideImage = document.getElementById('slideImage');
        
            function changeSlide() {
                if (images.length > 0) {
                    slideImage.src = images[slideIndex];
                    slideIndex = (slideIndex + 1) % images.length;
                }
            }
        
            setInterval(changeSlide, 3000);
            changeSlide();
        }
        
        // 🔹 Services Section
        function updateServices(images) {
            if (images.length >= 3) {
                document.getElementById('service1').src = images[0];
                document.getElementById('service2').src = images[1];
                document.getElementById('service3').src = images[2];
            }
        }
        
        // 🔹 Project Workflow Section (Randomized)
        function updateProjectWorkflow(images) {
            const projectCards = document.querySelectorAll('.project-card');
        
            projectCards.forEach((card, index) => {
                if (images[index]) {
                    const img = card.querySelector('img');
                    img.src = images[index];
        
                    // Randomly position: left, right, or center
                    const positions = ['text-left', 'text-right', 'text-center'];
                    card.classList.add(positions[Math.floor(Math.random() * positions.length)]);
                }
            });
        }
        
        // 🔹 Call API on page load
        fetchInstagramImages();
    </script>
</body>
</html>
