```html
<!DOCTYPE html>
<html lang="es" class="h-full bg-slate-950 text-slate-100">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pa cuando live? | lunayahaslive.com</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Space Grotesk & Inter -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&family=Space+Grotesk:wght@500;700;800&display=swap" rel="stylesheet">
    <!-- FontAwesome icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        display: ['Space Grotesk', 'sans-serif'],
                    },
                    animation: {
                        'pulse-slow': 'pulse 3s cubic-bezier(0.4, 0, 0.6, 1) infinite',
                        'neon-float': 'neonFloat 6s ease-in-out infinite alternate',
                        'spin-slow': 'spin 12s linear infinite',
                    },
                    keyframes: {
                        neonFloat: {
                            '0%': { transform: 'translateY(0px) rotate(0deg)', opacity: '0.6' },
                            '100%': { transform: 'translateY(-20px) rotate(3deg)', opacity: '0.9' },
                        }
                    }
                }
            }
        }
    </script>
    <style>
        /* Neon streamer gradient text */
        .neon-streamer-text {
            background: linear-gradient(135deg, #ffffff 0%, #a855f7 35%, #9333ea 65%, #00f59b 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            filter: drop-shadow(0 0 35px rgba(168, 85, 247, 0.45));
        }

        /* Ambient Neon Glow Backdrops */
        .neon-glow-purple {
            position: absolute;
            width: 450px;
            height: 450px;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(147, 51, 234, 0.3) 0%, rgba(168, 85, 247, 0.1) 50%, rgba(0, 0, 0, 0) 70%);
            filter: blur(80px);
            pointer-events: none;
        }

        .neon-glow-green {
            position: absolute;
            width: 350px;
            height: 350px;
            border-radius: 50%;
            background: radial-gradient(circle, rgba(0, 245, 155, 0.2) 0%, rgba(16, 185, 129, 0.05) 50%, rgba(0, 0, 0, 0) 70%);
            filter: blur(80px);
            pointer-events: none;
        }

        /* Glassmorphism Twitch-style card */
        .twitch-glass {
            background: rgba(13, 11, 24, 0.75);
            backdrop-filter: blur(20px);
            -webkit-backdrop-filter: blur(20px);
            border: 1px solid rgba(168, 85, 247, 0.2);
            box-shadow: 0 20px 50px rgba(0, 0, 0, 0.6), 0 0 30px rgba(147, 51, 234, 0.15);
        }

        /* Soft neon button glow */
        .neon-btn-glow {
            box-shadow: 0 0 20px rgba(168, 85, 247, 0.4), inset 0 0 10px rgba(255, 255, 255, 0.2);
        }
        .neon-btn-glow:hover {
            box-shadow: 0 0 30px rgba(168, 85, 247, 0.7), inset 0 0 15px rgba(255, 255, 255, 0.3);
        }
    </style>
</head>
<body class="h-full flex flex-col justify-between items-center overflow-x-hidden bg-[#090810] text-slate-100 selection:bg-purple-600 selection:text-white relative">

    <!-- Background Grid Effect -->
    <div class="fixed inset-0 bg-[linear-gradient(to_right,#a855f70a_1px,transparent_1px),linear-gradient(to_bottom,#a855f70a_1px,transparent_1px)] bg-[size:3.5rem_3.5rem] pointer-events-none"></div>

    <!-- Neon Glow Background Elements -->
    <div class="neon-glow-purple -top-10 -left-10 animate-neon-float"></div>
    <div class="neon-glow-green bottom-10 right-10 animate-neon-float" style="animation-delay: -3s;"></div>

    <!-- Streamer Top Navigation Bar -->
    <header class="w-full max-w-6xl px-6 py-6 flex justify-between items-center z-10">
        <div class="flex items-center gap-3">
            <div class="relative flex h-3 w-3">
              <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-purple-400 opacity-75"></span>
              <span class="relative inline-flex rounded-full h-3 w-3 bg-purple-500"></span>
            </div>
            <span class="text-xs font-mono font-bold tracking-widest text-purple-300 uppercase">lunayahaslive.com</span>
        </div>
        <div class="twitch-glass px-4 py-1.5 rounded-full flex items-center gap-2.5 text-xs text-slate-300">
            <i class="fa-brands fa-twitch text-purple-400 text-sm"></i>
            <span>Canal: <strong class="text-white font-semibold">OFFLINE</strong></span>
        </div>
    </header>

    <!-- Hero / Main Section -->
    <main class="w-full max-w-4xl px-4 my-auto flex flex-col items-center text-center z-10">
        
        <!-- Animated Badge -->
        <div class="mb-8 inline-flex items-center gap-2.5 px-4 py-2 rounded-full bg-purple-950/60 border border-purple-500/30 text-purple-300 text-xs sm:text-sm font-medium shadow-lg backdrop-blur-md">
            <i class="fa-solid fa-headset text-purple-400 animate-pulse"></i>
            <span class="tracking-wider uppercase font-semibold text-[11px] sm:text-xs">Esperando la transmisión</span>
        </div>

        <!-- Main Neon Heading -->
        <h1 class="font-display font-extrabold text-5xl sm:text-7xl md:text-8xl tracking-tight mb-6 neon-streamer-text leading-tight drop-shadow-2xl">
            Pa cuando live?
        </h1>

        <!-- Subtitle -->
        <p class="text-slate-400 text-base sm:text-lg max-w-md mx-auto mb-10 font-light leading-relaxed">
            El chat está esperando. Activa las notificaciones para enterarte apenas inicie el directo.
        </p>

        <!-- Streamer Interactive Card -->
        <div class="twitch-glass p-6 sm:p-8 rounded-3xl w-full max-w-md relative overflow-hidden">
            <!-- Top Light Accent Line -->
            <div class="absolute top-0 left-0 right-0 h-[2px] bg-gradient-to-r from-transparent via-purple-500 to-transparent"></div>

            <!-- Wait Timer -->
            <div class="mb-6">
                <span class="text-[11px] font-mono uppercase tracking-widest text-slate-400 block mb-3">Tiempo esperando directo</span>
                <div class="flex justify-center items-center gap-4 text-center bg-black/40 py-3 rounded-2xl border border-white/5">
                    <div class="flex flex-col">
                        <span id="hours" class="font-display text-3xl font-bold text-white">00</span>
                        <span class="text-[9px] text-slate-500 uppercase tracking-widest font-mono">Horas</span>
                    </div>
                    <span class="text-xl text-purple-500 font-bold mb-3">:</span>
                    <div class="flex flex-col">
                        <span id="minutes" class="font-display text-3xl font-bold text-white">00</span>
                        <span class="text-[9px] text-slate-500 uppercase tracking-widest font-mono">Min</span>
                    </div>
                    <span class="text-xl text-purple-500 font-bold mb-3">:</span>
                    <div class="flex flex-col">
                        <span id="seconds" class="font-display text-3xl font-bold text-emerald-400">00</span>
                        <span class="text-[9px] text-slate-500 uppercase tracking-widest font-mono">Seg</span>
                    </div>
                </div>
            </div>

            <!-- Notification Action Button -->
            <button id="notifyBtn" onclick="toggleNotify()" class="w-full py-4 px-6 rounded-2xl bg-gradient-to-r from-purple-600 via-indigo-600 to-purple-700 hover:from-purple-500 hover:to-indigo-500 text-white font-bold text-sm transition-all duration-300 transform active:scale-95 neon-btn-glow flex items-center justify-center gap-2.5 group">
                <i id="bellIcon" class="fa-solid fa-bell group-hover:rotate-12 transition-transform text-purple-200"></i>
                <span id="btnText">¡Avisarme cuando prenda!</span>
            </button>

            <!-- Social Media Icons -->
            <div class="mt-6 pt-4 border-t border-white/5 flex justify-center items-center gap-6 text-slate-400 text-xl">
                <a href="#" class="hover:text-purple-400 transition-all hover:scale-110" title="Twitch"><i class="fa-brands fa-twitch"></i></a>
                <a href="#" class="hover:text-red-500 transition-all hover:scale-110" title="YouTube"><i class="fa-brands fa-youtube"></i></a>
                <a href="#" class="hover:text-emerald-400 transition-all hover:scale-110" title="Kick"><i class="fa-solid fa-bolt"></i></a>
                <a href="#" class="hover:text-sky-400 transition-all hover:scale-110" title="Twitter / X"><i class="fa-brands fa-x-twitter"></i></a>
                <a href="#" class="hover:text-pink-500 transition-all hover:scale-110" title="Instagram"><i class="fa-brands fa-instagram"></i></a>
            </div>
        </div>

    </main>

    <!-- Footer -->
    <footer class="w-full py-6 text-center text-xs text-slate-500 z-10">
        <p>© <span id="year"></span> lunayahaslive.com — Todos los derechos reservados.</p>
    </footer>

    <!-- Notification Toast -->
    <div id="toast" class="fixed bottom-6 right-6 twitch-glass px-5 py-3.5 rounded-2xl shadow-2xl flex items-center gap-3 text-sm text-slate-200 transform translate-y-24 opacity-0 transition-all duration-300 z-50">
        <i class="fa-solid fa-circle-check text-emerald-400 text-lg"></i>
        <span>¡Te avisaremos en cuanto empiece el live!</span>
    </div>

    <!-- Script para lógica dinámica -->
    <script>
        document.getElementById('year').textContent = new Date().getFullYear();

        // Contador de tiempo de espera
        let totalSeconds = 3600 * 2 + 1800 + 45;
        
        function updateCounter() {
            totalSeconds++;
            const hrs = Math.floor(totalSeconds / 3600);
            const mins = Math.floor((totalSeconds % 3600) / 60);
            const secs = totalSeconds % 60;

            document.getElementById('hours').textContent = String(hrs).padStart(2, '0');
            document.getElementById('minutes').textContent = String(mins).padStart(2, '0');
            document.getElementById('seconds').textContent = String(secs).padStart(2, '0');
        }

        setInterval(updateCounter, 1000);

        // Activación de notificaciones
        let notified = false;
        function toggleNotify() {
            const btnText = document.getElementById('btnText');
            const bellIcon = document.getElementById('bellIcon');
            const toast = document.getElementById('toast');

            notified = !notified;

            if (notified) {
                btnText.textContent = '¡Notificación Activada!';
                bellIcon.className = 'fa-solid fa-bell text-emerald-300 animate-bounce';
                
                toast.classList.remove('translate-y-24', 'opacity-0');
                setTimeout(() => {
                    toast.classList.add('translate-y-24', 'opacity-0');
                }, 3500);
            } else {
                btnText.textContent = '¡Avisarme cuando prenda!';
                bellIcon.className = 'fa-solid fa-bell text-purple-200';
            }
        }
    </script>
</body>
</html>
```
