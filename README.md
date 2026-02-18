<!DOCTYPE html>
<html lang="en" class="scroll-smooth dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arcson — Building What's Next</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
        body { font-family: 'Inter', system_ui, sans-serif; }
        .hero-bg { background: linear-gradient(135deg, #0f172a 0%, #1e2937 100%); }
    </style>
</head>
<body class="bg-zinc-950 text-zinc-200">
    <!-- Navbar -->
    <nav class="fixed top-0 w-full border-b border-zinc-800 bg-zinc-950/80 backdrop-blur-lg z-50">
        <div class="max-w-6xl mx-auto px-6 py-5 flex items-center justify-between">
            <div class="flex items-center gap-3">
                <div class="w-9 h-9 bg-gradient-to-br from-blue-600 to-indigo-600 rounded-2xl flex items-center justify-center text-white font-bold text-2xl">A</div>
                <span class="text-2xl font-semibold tracking-tighter">Arcson</span>
            </div>
            <div class="hidden md:flex gap-8 text-sm font-medium">
                <a href="#about" class="hover:text-white transition">About</a>
                <a href="#services" class="hover:text-white transition">Services</a>
                <a href="#projects" class="hover:text-white transition">Projects</a>
                <a href="#contact" class="hover:text-white transition">Contact</a>
            </div>
            <button onclick="toggleTheme()" class="p-3 rounded-xl hover:bg-zinc-800 transition">
                <i class="fas fa-moon text-xl" id="theme-icon"></i>
            </button>
        </div>
    </nav>

    <!-- Hero -->
    <section class="hero-bg min-h-screen flex items-center pt-20">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <h1 class="text-6xl md:text-7xl font-bold tracking-tighter mb-6">We build the future.</h1>
            <p class="text-2xl text-zinc-400 max-w-2xl mx-auto mb-12">Clean code. Reliable systems. Canadian-made.</p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#contact" class="px-10 py-4 bg-white text-zinc-950 font-semibold rounded-2xl hover:bg-zinc-100 transition text-lg">Let's talk</a>
                <a href="https://github.com/arcson-ca" target="_blank" class="px-10 py-4 border border-white/30 font-semibold rounded-2xl hover:bg-white/10 transition text-lg flex items-center justify-center gap-3">
                    <i class="fab fa-github"></i> GitHub
                </a>
            </div>
        </div>
    </section>

    <!-- About -->
    <section id="about" class="py-24 bg-zinc-900">
        <div class="max-w-6xl mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div>
                    <h2 class="text-5xl font-bold tracking-tight mb-8">Arcson is a Canadian technology studio.</h2>
                    <p class="text-lg text-zinc-400 leading-relaxed">We create simple, powerful digital products and infrastructure that just work. From private photo libraries to custom web tools — everything we build is secure, fast, and built to last.</p>
                </div>
                <div class="bg-zinc-800/50 border border-zinc-700 rounded-3xl p-10 text-sm space-y-6">
                    <div class="flex gap-4">
                        <div class="text-blue-400"><i class="fas fa-shield-alt text-2xl"></i></div>
                        <div>Privacy-first by default</div>
                    </div>
                    <div class="flex gap-4">
                        <div class="text-blue-400"><i class="fas fa-bolt text-2xl"></i></div>
                        <div>Lightning-fast Canadian hosting</div>
                    </div>
                    <div class="flex gap-4">
                        <div class="text-blue-400"><i class="fas fa-code text-2xl"></i></div>
                        <div>Open-source where it matters</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services / Projects -->
    <section id="services" class="py-24">
        <div class="max-w-6xl mx-auto px-6">
            <h2 class="text-4xl font-bold text-center mb-16">What we're building</h2>
            <div class="grid md:grid-cols-3 gap-8">
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 hover:border-blue-500 transition group">
                    <div class="text-blue-500 mb-6"><i class="fas fa-camera text-5xl"></i></div>
                    <h3 class="text-2xl font-semibold mb-3">Private Photo Hosting</h3>
                    <p class="text-zinc-400">Self-hosted Immich instances with Cloudflare Access protection.</p>
                </div>
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 hover:border-blue-500 transition group">
                    <div class="text-blue-500 mb-6"><i class="fas fa-images text-5xl"></i></div>
                    <h3 class="text-2xl font-semibold mb-3">Easy Albums</h3>
                    <p class="text-zinc-400">Beautiful shared photo albums for friends & family.</p>
                </div>
                <div class="bg-zinc-900 border border-zinc-800 rounded-3xl p-8 hover:border-blue-500 transition group">
                    <div class="text-blue-500 mb-6"><i class="fas fa-code text-5xl"></i></div>
                    <h3 class="text-2xl font-semibold mb-3">Custom Tools</h3>
                    <p class="text-zinc-400">Web apps, automation, and internal tools.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="py-24 bg-zinc-900">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <h2 class="text-5xl font-bold tracking-tight mb-6">Ready to build something?</h2>
            <p class="text-xl text-zinc-400 mb-12">Drop us a line — we reply fast.</p>
            <a href="mailto:hello@arcson.ca" class="inline-flex items-center gap-3 px-10 py-5 bg-blue-600 hover:bg-blue-500 rounded-3xl text-xl font-semibold transition">
                hello@arcson.ca <i class="fas fa-arrow-right"></i>
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer class="border-t border-zinc-800 py-12 bg-black">
        <div class="max-w-6xl mx-auto px-6 text-center text-zinc-500 text-sm">
            © 2026 Arcson • Made in Canada • <a href="https://github.com/arcson-ca" class="hover:text-white">GitHub</a>
        </div>
    </footer>

    <script>
        function toggleTheme() {
            document.documentElement.classList.toggle('dark');
            const icon = document.getElementById('theme-icon');
            icon.classList.toggle('fa-moon');
            icon.classList.toggle('fa-sun');
        }
        // Set initial icon
        document.getElementById('theme-icon').classList.add('fa-sun');
    </script>
</body>
</html>
