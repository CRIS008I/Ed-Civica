<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Oltre le Etichette - Genere e Identità</title>
    <!-- Tailwind CSS per lo stile -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome per le icone -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;800&display=swap" rel="stylesheet">
    
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f8fafc;
            overflow-x: hidden;
        }
        
        /* Classi per l'animazione allo scorrimento */
        .reveal {
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.8s ease-out;
        }
        
        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }

        /* Gradiente di sfondo per l'intestazione */
        .bg-hero {
            background: linear-gradient(135deg, #4f46e5 0%, #db2777 100%);
        }
        
        /* Stile per le card */
        .glass-card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 1rem;
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1), 0 8px 10px -6px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        /* Decorazioni laterali per le card */
        .glass-card::before {
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            width: 8px;
        }
        .card-pink::before { left: 0; background-color: #db2777; }
        .card-indigo::before { right: 0; background-color: #4f46e5; }
        .card-teal::before { left: 0; background-color: #0d9488; }
    </style>
</head>
<body class="text-slate-800">

    <!-- HERO SECTION -->
    <header class="bg-hero min-h-screen flex flex-col justify-center items-center text-white p-6 text-center relative">
        <div class="reveal active max-w-4xl">
            <i class="fa-solid fa-masks-theater text-5xl md:text-7xl mb-6 opacity-80 drop-shadow-md"></i>
            <h1 class="text-5xl md:text-7xl font-extrabold mb-4 tracking-tight drop-shadow-lg">Oltre le Etichette</h1>
            <p class="text-xl md:text-2xl font-light mb-8 max-w-2xl mx-auto opacity-90 drop-shadow">
                Il viaggio del "Gender" tra biologia, cultura e la ricerca della nostra identità.
            </p>
            <div class="mt-12 animate-bounce">
                <p class="text-sm uppercase tracking-widest mb-2 opacity-80 font-semibold">Scorri per esplorare</p>
                <i class="fa-solid fa-chevron-down text-2xl"></i>
            </div>
        </div>
        <!-- Onda decorativa -->
        <svg class="absolute bottom-0 w-full text-slate-50" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
            <path fill="currentColor" fill-opacity="1" d="M0,160L48,176C96,192,192,224,288,218.7C384,213,480,171,576,149.3C672,128,768,128,864,149.3C960,171,1056,213,1152,224C1248,235,1344,213,1392,202.7L1440,192L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
        </svg>
    </header>

    <!-- MAIN CONTENT -->
    <main class="container mx-auto px-4 py-16 max-w-5xl">

        <!-- Punto 1 -->
        <section class="reveal mb-16 md:mb-24 flex flex-col md:flex-row items-center gap-8">
            <div class="md:w-1/3 flex justify-center text-pink-600">
                <i class="fa-solid fa-dna text-8xl md:text-9xl drop-shadow-lg transform hover:scale-110 transition-transform duration-300"></i>
            </div>
            <div class="glass-card card-pink p-8 md:p-10 md:w-2/3 pl-10">
                <h2 class="text-3xl font-bold mb-4 text-slate-800">1. Sesso $\neq$ Genere</h2>
                <p class="text-lg leading-relaxed text-slate-600">
                    Il <strong>Sesso</strong> definisce la nostra biologia. Il <strong>Genere</strong> è pura cultura: sono i ruoli e i significati che la società ci attribuisce. Questa distinzione, nata negli anni '70, è rivoluzionaria: ha <span class="bg-pink-100 text-pink-800 font-semibold px-2 py-1 rounded">smascherato la falsa idea che le gerarchie sociali siano "naturali"</span>, offrendo nuove strategie politiche di liberazione.
                </p>
            </div>
        </section>

        <!-- Punto 2 -->
        <section class="reveal mb-16 md:mb-24 flex flex-col md:flex-row-reverse items-center gap-8">
            <div class="md:w-1/3 flex justify-center text-indigo-600">
                <i class="fa-solid fa-puzzle-piece text-8xl md:text-9xl drop-shadow-lg transform hover:scale-110 transition-transform duration-300"></i>
            </div>
            <div class="glass-card card-indigo p-8 md:p-10 md:w-2/3 pr-10">
                <h2 class="text-3xl font-bold mb-4 text-slate-800">2. L'Identità è un Mosaico</h2>
                <p class="text-lg leading-relaxed text-slate-600">
                    Con il tempo, la riflessione si amplia. Capiamo che l'identità non è determinata <em>solo</em> dal genere, ma si gioca su più piani simultanei. Si apre a una <strong>molteplicità di fattori concorrenti</strong>, come la <em>razza</em>, la <em>classe sociale</em> e l'<em>orientamento sessuale</em>, delineando la differenza fondamentale tra biologia e identità percepita.
                </p>
            </div>
        </section>

        <!-- Punto 3 -->
        <section class="reveal mb-16 md:mb-24 flex flex-col md:flex-row items-center gap-8">
            <div class="md:w-1/3 flex justify-center text-teal-600">
                <i class="fa-solid fa-scale-balanced text-8xl md:text-9xl drop-shadow-lg transform hover:scale-110 transition-transform duration-300"></i>
            </div>
            <div class="glass-card card-teal p-8 md:p-10 md:w-2/3 pl-10">
                <h2 class="text-3xl font-bold mb-4 text-slate-800">3. Il Paradosso e i Simboli per Definirsi</h2>
                <p class="text-lg leading-relaxed text-slate-600">
                    Ignorare del tutto i corpi crea un rischioso "soggetto indistinto". Come osserva R. Braidotti, la dissoluzione del soggetto avvantaggia solo <strong>chi ha già potere e autorità</strong> (il maschio dominante). 
                </p>
                <div class="mt-4 p-4 bg-teal-50 rounded-lg border border-teal-100">
                    <p class="text-md text-teal-900">
                        <strong>La vera sfida:</strong> Usare la categoria di genere con consapevolezza. Serve a decostruire le gerarchie culturali e a <em>fornire alle donne e ai soggetti marginalizzati i simboli per definirsi partendo da sé</em>, in un mondo in cui il modello "normativo" è ancora maschile.
                    </p>
                </div>
            </div>
        </section>

    </main>

    <!-- FOOTER -->
    <footer class="bg-slate-900 text-slate-400 py-8 text-center border-t-4 border-pink-600">
        <p class="text-sm">
            Riflessione basata sul testo <em>"Gender e femminismo"</em> di Simona Segoloni Ruta (2021).
        </p>
    </footer>

    <!-- Script per le animazioni -->
    <script>
        function revealOnScroll() {
            var reveals = document.querySelectorAll('.reveal');
            var windowHeight = window.innerHeight;
            
            reveals.forEach(function(reveal) {
                var elementTop = reveal.getBoundingClientRect().top;
                var elementVisible = 100; // Quando attivare l'animazione
                
                if (elementTop < windowHeight - elementVisible) {
                    reveal.classList.add("active");
                }
            });
        }

        window.addEventListener("scroll", revealOnScroll);
        // Trigger iniziale al caricamento
        setTimeout(revealOnScroll, 100); 
    </script>
</body>
</html>
