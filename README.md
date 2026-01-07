<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adab Student's Union | SFADC</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

    <style>
        body {
            font-family: 'Plus Jakarta Sans', sans-serif;
        }
        
        .hero-pattern {
            background-color: #1e293b;
            background-image: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23334155' fill-opacity='0.4'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .text-gradient {
            background: linear-gradient(135deg, #1e40af 0%, #3b82f6 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .animate-fade-in {
            animation: fadeIn 0.8s ease-out forwards;
            opacity: 0;
            transform: translateY(20px);
        }

        @keyframes fadeIn {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 antialiased">

    <!-- Navigation -->
    <nav class="fixed w-full z-50 transition-all duration-300 bg-white/90 backdrop-blur-md shadow-sm" id="navbar">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20 items-center">
                <!-- Logo -->
                <div class="flex-shrink-0 flex items-center gap-2 cursor-pointer" onclick="window.scrollTo(0,0)">
                    <div class="w-10 h-10 bg-blue-900 rounded-lg flex items-center justify-center text-white font-bold text-xl">A</div>
                    <div>
                        <span class="font-bold text-xl tracking-tight text-slate-900 block leading-none">ADAB</span>
                        <span class="text-xs text-blue-600 font-semibold tracking-wide">STUDENT'S UNION</span>
                    </div>
                </div>

                <!-- Desktop Menu -->
                <div class="hidden md:flex space-x-8 items-center">
                    <a href="#home" class="text-slate-600 hover:text-blue-700 font-medium transition-colors">Home</a>
                    <a href="#about" class="text-slate-600 hover:text-blue-700 font-medium transition-colors">About</a>
                    <a href="#leadership" class="text-slate-600 hover:text-blue-700 font-medium transition-colors">Committee</a>
                    <a href="#events" class="text-slate-600 hover:text-blue-700 font-medium transition-colors">Events</a>
                    <a href="#contact" class="bg-blue-900 text-white px-5 py-2.5 rounded-full font-medium hover:bg-blue-800 transition-all shadow-lg shadow-blue-900/20 transform hover:-translate-y-0.5">Contact Us</a>
                </div>

                <!-- Mobile Menu Button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-slate-600 hover:text-blue-900 focus:outline-none">
                        <i data-lucide="menu" class="w-8 h-8"></i>
                    </button>
                </div>
            </div>
        </div>

        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-slate-100">
            <div class="px-4 pt-2 pb-6 space-y-1">
                <a href="#home" class="block px-3 py-3 rounded-md text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-700">Home</a>
                <a href="#about" class="block px-3 py-3 rounded-md text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-700">About</a>
                <a href="#leadership" class="block px-3 py-3 rounded-md text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-700">Committee</a>
                <a href="#events" class="block px-3 py-3 rounded-md text-base font-medium text-slate-700 hover:bg-blue-50 hover:text-blue-700">Events</a>
                <a href="#contact" class="block px-3 py-3 mt-4 text-center rounded-md text-base font-bold bg-blue-900 text-white">Contact Us</a>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="relative pt-32 pb-20 lg:pt-48 lg:pb-32 overflow-hidden hero-pattern">
        <div class="absolute inset-0 bg-gradient-to-b from-transparent to-slate-900/90"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10 text-center">
            <div class="inline-flex items-center gap-2 px-4 py-2 rounded-full bg-blue-500/10 border border-blue-400/20 text-blue-100 text-sm font-medium mb-8 animate-fade-in" style="animation-delay: 0.1s;">
                <span class="w-2 h-2 rounded-full bg-blue-400 animate-pulse"></span>
                Welcome to the Official Union Portal
            </div>
            
            <h1 class="text-4xl md:text-6xl lg:text-7xl font-extrabold text-white tracking-tight mb-6 animate-fade-in leading-tight" style="animation-delay: 0.2s;">
                Empowering Minds, <br />
                <span class="text-transparent bg-clip-text bg-gradient-to-r from-blue-400 to-indigo-400">Shaping the Future.</span>
            </h1>
            
            <p class="mt-4 max-w-2xl mx-auto text-xl text-slate-300 animate-fade-in" style="animation-delay: 0.3s;">
                The Adab Student's Union at SFADC stands for integrity, innovation, and unity. We are the voice of the students, dedicated to academic excellence and cultural growth.
            </p>
            
            <div class="mt-10 flex flex-col sm:flex-row justify-center gap-4 animate-fade-in" style="animation-delay: 0.4s;">
                <a href="#join" class="px-8 py-4 rounded-full bg-blue-600 text-white font-bold text-lg hover:bg-blue-500 transition-all shadow-lg shadow-blue-600/30 flex items-center justify-center gap-2">
                    Join Our Community
                    <i data-lucide="arrow-right" class="w-5 h-5"></i>
                </a>
                <a href="#events" class="px-8 py-4 rounded-full bg-white/10 backdrop-blur-sm border border-white/20 text-white font-bold text-lg hover:bg-white/20 transition-all flex items-center justify-center gap-2">
                    <i data-lucide="calendar" class="w-5 h-5"></i>
                    Upcoming Events
                </a>
            </div>
        </div>
    </section>

    <!-- Stats Section -->
    <section class="py-10 bg-white shadow-sm relative z-20 -mt-8 mx-4 md:mx-auto max-w-6xl rounded-2xl glass-card">
        <div class="grid grid-cols-2 md:grid-cols-4 gap-8 text-center divide-x divide-slate-100">
            <div class="p-4">
                <div class="text-3xl font-bold text-blue-900">500+</div>
                <div class="text-sm text-slate-500 font-medium mt-1">Active Members</div>
            </div>
            <div class="p-4">
                <div class="text-3xl font-bold text-blue-900">50+</div>
                <div class="text-sm text-slate-500 font-medium mt-1">Yearly Events</div>
            </div>
            <div class="p-4">
                <div class="text-3xl font-bold text-blue-900">12</div>
                <div class="text-sm text-slate-500 font-medium mt-1">Committee Members</div>
            </div>
            <div class="p-4">
                <div class="text-3xl font-bold text-blue-900">24/7</div>
                <div class="text-sm text-slate-500 font-medium mt-1">Student Support</div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-24 bg-slate-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid lg:grid-cols-2 gap-16 items-center">
                <div class="order-2 lg:order-1 relative">
                    <div class="absolute -top-4 -left-4 w-72 h-72 bg-blue-200 rounded-full mix-blend-multiply filter blur-3xl opacity-30"></div>
                    <div class="relative rounded-2xl overflow-hidden shadow-2xl">
                        <!-- Placeholder for a group photo or campus shot -->
                        <img src="https://images.unsplash.com/photo-1523580494863-6f3031224c94?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Students Gathering" class="w-full h-full object-cover">
                        <div class="absolute inset-0 bg-gradient-to-t from-blue-900/60 to-transparent"></div>
                        <div class="absolute bottom-6 left-6 text-white">
                            <p class="font-bold text-lg">Founded in Tradition</p>
                            <p class="text-sm opacity-80">Leading with Innovation</p>
                        </div>
                    </div>
                </div>
                
                <div class="order-1 lg:order-2">
                    <div class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-blue-100 text-blue-700 text-xs font-bold uppercase tracking-wider mb-6">
                        About Us
                    </div>
                    <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mb-6">Fostering Academic & Creative Excellence</h2>
                    <p class="text-lg text-slate-600 mb-6 leading-relaxed">
                        The Adab Student's Union is the representative body of students at SFADC. We are committed to creating an environment where every student can thrive academically, socially, and creatively.
                    </p>
                    <ul class="space-y-4 mb-8">
                        <li class="flex items-start gap-3">
                            <div class="flex-shrink-0 w-6 h-6 rounded-full bg-green-100 flex items-center justify-center text-green-600 mt-1">
                                <i data-lucide="check" class="w-4 h-4"></i>
                            </div>
                            <span class="text-slate-700">Organizing educational workshops and seminars.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <div class="flex-shrink-0 w-6 h-6 rounded-full bg-green-100 flex items-center justify-center text-green-600 mt-1">
                                <i data-lucide="check" class="w-4 h-4"></i>
                            </div>
                            <span class="text-slate-700">Promoting arts, literature, and cultural activities.</span>
                        </li>
                        <li class="flex items-start gap-3">
                            <div class="flex-shrink-0 w-6 h-6 rounded-full bg-green-100 flex items-center justify-center text-green-600 mt-1">
                                <i data-lucide="check" class="w-4 h-4"></i>
                            </div>
                            <span class="text-slate-700">Providing a platform for student grievances and welfare.</span>
                        </li>
                    </ul>
                    <a href="#committee" class="text-blue-600 font-bold hover:text-blue-800 inline-flex items-center gap-2 group transition-colors">
                        Meet the Leaders
                        <i data-lucide="arrow-right" class="w-4 h-4 transform group-hover:translate-x-1 transition-transform"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Leadership Committee Section -->
    <section id="leadership" class="py-24 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mb-4">Our Committee</h2>
                <p class="text-slate-600 max-w-2xl mx-auto">Meet the dedicated individuals working tirelessly to serve the student community.</p>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- Member 1 -->
                <div class="group relative">
                    <div class="aspect-[4/5] rounded-2xl overflow-hidden bg-slate-200">
                        <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" alt="President" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="mt-4">
                        <h3 class="text-xl font-bold text-slate-900">Mohammed Zayan</h3>
                        <p class="text-blue-600 font-medium">President</p>
                    </div>
                </div>

                <!-- Member 2 -->
                <div class="group relative">
                    <div class="aspect-[4/5] rounded-2xl overflow-hidden bg-slate-200">
                        <img src="https://images.unsplash.com/photo-1519085360753-af0119f7cbe7?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" alt="Secretary" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="mt-4">
                        <h3 class="text-xl font-bold text-slate-900">Abdullah Razi</h3>
                        <p class="text-blue-600 font-medium">General Secretary</p>
                    </div>
                </div>

                <!-- Member 3 (Personalized Context) -->
                <div class="group relative">
                    <div class="aspect-[4/5] rounded-2xl overflow-hidden bg-slate-200 relative">
                        <!-- Custom badge for the personalized profile -->
                        <div class="absolute top-3 right-3 bg-blue-600 text-white text-xs px-2 py-1 rounded font-bold z-10 shadow-sm">MEDIA</div>
                        <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" alt="Baheej" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="mt-4">
                        <h3 class="text-xl font-bold text-slate-900">Baheej</h3>
                        <p class="text-blue-600 font-medium">Head of Journalism & Media</p>
                        <p class="text-xs text-slate-500 mt-1 line-clamp-2">Specializing in politics and current affairs.</p>
                    </div>
                </div>

                <!-- Member 4 -->
                <div class="group relative">
                    <div class="aspect-[4/5] rounded-2xl overflow-hidden bg-slate-200">
                        <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-4.0.3&auto=format&fit=crop&w=400&q=80" alt="Arts Secretary" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">
                    </div>
                    <div class="mt-4">
                        <h3 class="text-xl font-bold text-slate-900">Ibrahim K.</h3>
                        <p class="text-blue-600 font-medium">Arts Secretary</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Events Section -->
    <section id="events" class="py-24 bg-slate-50 relative overflow-hidden">
        <!-- Background decorative elements -->
        <div class="absolute top-0 right-0 w-1/3 h-full bg-slate-100 skew-x-12 transform origin-top-right z-0"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="flex flex-col md:flex-row justify-between items-end mb-12 gap-4">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mb-2">Upcoming Events</h2>
                    <p class="text-slate-600">Don't miss out on what's happening at Adab Union.</p>
                </div>
                <a href="#" class="text-blue-600 font-bold hover:underline flex items-center gap-1">View Calendar <i data-lucide="arrow-up-right" class="w-4 h-4"></i></a>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <!-- Event Card 1 -->
                <div class="bg-white rounded-2xl p-6 shadow-lg shadow-slate-200/50 hover:shadow-xl transition-shadow border border-slate-100">
                    <div class="flex items-center justify-between mb-4">
                        <span class="bg-blue-100 text-blue-700 text-xs font-bold px-3 py-1 rounded-full">ACADEMIC</span>
                        <span class="text-slate-400 text-sm font-medium flex items-center gap-1"><i data-lucide="clock" class="w-3 h-3"></i> 2 Days left</span>
                    </div>
                    <div class="mb-4">
                        <div class="text-4xl font-bold text-slate-900 mb-1">15</div>
                        <div class="text-sm font-bold text-slate-500 uppercase tracking-wide">Oct, 2025</div>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-2">Media & Politics Workshop</h3>
                    <p class="text-slate-600 text-sm mb-4">An interactive session led by the Media Wing focusing on modern journalism trends.</p>
                    <button class="w-full py-2 rounded-lg border border-slate-200 text-slate-700 font-medium hover:bg-slate-50 transition-colors text-sm">Register Now</button>
                </div>

                <!-- Event Card 2 -->
                <div class="bg-white rounded-2xl p-6 shadow-lg shadow-slate-200/50 hover:shadow-xl transition-shadow border border-slate-100">
                    <div class="flex items-center justify-between mb-4">
                        <span class="bg-purple-100 text-purple-700 text-xs font-bold px-3 py-1 rounded-full">CULTURAL</span>
                        <span class="text-slate-400 text-sm font-medium flex items-center gap-1"><i data-lucide="clock" class="w-3 h-3"></i> 10 Days left</span>
                    </div>
                    <div class="mb-4">
                        <div class="text-4xl font-bold text-slate-900 mb-1">25</div>
                        <div class="text-sm font-bold text-slate-500 uppercase tracking-wide">Oct, 2025</div>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-2">Adab Arts Fest '25</h3>
                    <p class="text-slate-600 text-sm mb-4">The biggest cultural gathering of the year featuring debates, poetry, and art.</p>
                    <button class="w-full py-2 rounded-lg border border-slate-200 text-slate-700 font-medium hover:bg-slate-50 transition-colors text-sm">View Details</button>
                </div>

                <!-- Event Card 3 -->
                <div class="bg-white rounded-2xl p-6 shadow-lg shadow-slate-200/50 hover:shadow-xl transition-shadow border border-slate-100">
                    <div class="flex items-center justify-between mb-4">
                        <span class="bg-orange-100 text-orange-700 text-xs font-bold px-3 py-1 rounded-full">SPORTS</span>
                        <span class="text-slate-400 text-sm font-medium flex items-center gap-1"><i data-lucide="clock" class="w-3 h-3"></i> TBD</span>
                    </div>
                    <div class="mb-4">
                        <div class="text-4xl font-bold text-slate-900 mb-1">05</div>
                        <div class="text-sm font-bold text-slate-500 uppercase tracking-wide">Nov, 2025</div>
                    </div>
                    <h3 class="text-xl font-bold text-slate-900 mb-2">Inter-Class Football</h3>
                    <p class="text-slate-600 text-sm mb-4">League matches starting soon at the main ground. Register your teams.</p>
                    <button class="w-full py-2 rounded-lg border border-slate-200 text-slate-700 font-medium hover:bg-slate-50 transition-colors text-sm">Register Team</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-24 bg-blue-900 text-white relative overflow-hidden">
        <div class="absolute inset-0 opacity-10" style="background-image: radial-gradient(#ffffff 1px, transparent 1px); background-size: 30px 30px;"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-2 gap-16">
                <div>
                    <h2 class="text-3xl md:text-4xl font-bold mb-6">Get in Touch</h2>
                    <p class="text-blue-200 mb-8 text-lg">Have suggestions, complaints, or just want to connect? We are here to listen.</p>
                    
                    <div class="space-y-6">
                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 rounded-full bg-blue-800 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="map-pin" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Visit Us</h4>
                                <p class="text-blue-200">SFADC Campus, Darul Huda Islamic University Affiliated Center.</p>
                            </div>
                        </div>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 rounded-full bg-blue-800 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="mail" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Email Us</h4>
                                <p class="text-blue-200">union@adab-sfadc.edu</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 rounded-full bg-blue-800 flex items-center justify-center flex-shrink-0">
                                <i data-lucide="phone" class="w-5 h-5"></i>
                            </div>
                            <div>
                                <h4 class="font-bold text-lg">Call Us</h4>
                                <p class="text-blue-200">+91 98765 43210</p>
                            </div>
                        </div>
                    </div>

                    <div class="mt-10 flex gap-4">
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                            <i data-lucide="instagram" class="w-5 h-5"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                            <i data-lucide="facebook" class="w-5 h-5"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-white/10 hover:bg-white/20 flex items-center justify-center transition-colors">
                            <i data-lucide="twitter" class="w-5 h-5"></i>
                        </a>
                    </div>
                </div>

                <div class="bg-white rounded-2xl p-8 text-slate-900 shadow-2xl">
                    <form onsubmit="event.preventDefault(); alert('Thank you for your message! The union secretary will contact you shortly.');">
                        <div class="grid md:grid-cols-2 gap-4 mb-4">
                            <div>
                                <label class="block text-sm font-bold text-slate-700 mb-2">Name</label>
                                <input type="text" class="w-full px-4 py-3 rounded-lg bg-slate-50 border border-slate-200 focus:outline-none focus:border-blue-500 transition-colors" placeholder="Your Name" required>
                            </div>
                            <div>
                                <label class="block text-sm font-bold text-slate-700 mb-2">Class/Batch</label>
                                <input type="text" class="w-full px-4 py-3 rounded-lg bg-slate-50 border border-slate-200 focus:outline-none focus:border-blue-500 transition-colors" placeholder="e.g. 2nd Year" required>
                            </div>
                        </div>
                        <div class="mb-4">
                            <label class="block text-sm font-bold text-slate-700 mb-2">Email</label>
                            <input type="email" class="w-full px-4 py-3 rounded-lg bg-slate-50 border border-slate-200 focus:outline-none focus:border-blue-500 transition-colors" placeholder="you@example.com" required>
                        </div>
                        <div class="mb-6">
                            <label class="block text-sm font-bold text-slate-700 mb-2">Message</label>
                            <textarea class="w-full px-4 py-3 rounded-lg bg-slate-50 border border-slate-200 focus:outline-none focus:border-blue-500 transition-colors h-32 resize-none" placeholder="How can we help you?" required></textarea>
                        </div>
                        <button type="submit" class="w-full py-3 rounded-lg bg-blue-900 text-white font-bold hover:bg-blue-800 transition-colors shadow-lg shadow-blue-900/20">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-900 text-slate-400 py-8 border-t border-slate-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center gap-4">
            <div class="text-sm">
                &copy; 2025 Adab Student's Union. All rights reserved.
            </div>
            <div class="flex gap-6 text-sm font-medium">
                <a href="#" class="hover:text-white transition-colors">Constitution</a>
                <a href="#" class="hover:text-white transition-colors">Privacy</a>
                <a href="#" class="hover:text-white transition-colors">Support</a>
            </div>
        </div>
    </footer>

    <!-- Scripts -->
    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Mobile Menu Toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            const icon = mobileMenu.classList.contains('hidden') ? 'menu' : 'x';
            // Re-render icon logic if using react, but here simple toggle is fine.
            // For simplicity in vanilla JS with Lucide re-render:
            mobileMenuBtn.innerHTML = `<i data-lucide="${icon}" class="w-8 h-8"></i>`;
            lucide.createIcons();
        });

        // Sticky Navbar Effect
        window.addEventListener('scroll', () => {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 10) {
                navbar.classList.add('shadow-md');
                navbar.classList.replace('bg-white/90', 'bg-white/95');
            } else {
                navbar.classList.remove('shadow-md');
                navbar.classList.replace('bg-white/95', 'bg-white/90');
            }
        });
    </script>
</body>
</html>
