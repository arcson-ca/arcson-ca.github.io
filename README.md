<!DOCTYPE html>
<html lang="en" class="scroll-smooth dark">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arcson Canadat</title>
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
                <a href="#contact" class="hover:text-white transition">Contact</a>
            </div>
            <button onclick="toggleTheme()" class="p-3 rounded-xl hover:bg-zinc-800 transition">
                <i class="fas fa-moon text-xl" id="theme-icon"></i>
            </button>
        </div>
    </nav>

    <!-- About -->
    <section id="about" class="py-24 bg-zinc-900">
        <div class="max-w-6xl mx-auto px-6">
            <div class="grid md:grid-cols-2 gap-16 items-center">
                <div>
                    <h2 class="text-5xl font-bold tracking-tight mb-8">Arcson Canada is a work from Peter Watkins a sole proprietor in Victoria BC.</h2>
                    <p class="text-lg text-zinc-400 leading-relaxed">Sharing solutions I've built that may have value for others.</p>
                </div>
            </div>
        </div>
    </section>


    <!-- Contact -->
    <section id="contact" class="py-24 bg-zinc-900">
        <div class="max-w-6xl mx-auto px-6 text-center">
            <a href="mailto:peter@arcson.ca" class="inline-flex items-center gap-3 px-10 py-5 bg-blue-600 hover:bg-blue-500 rounded-3xl text-xl font-semibold transition">
                peter@arcson.ca <i class="fas fa-arrow-right"></i>
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
