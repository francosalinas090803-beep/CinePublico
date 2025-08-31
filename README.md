<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CinePúblico - Películas de Dominio Público en Español</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #1a202c 0%, #2d3748 100%);
            min-height: 100vh;
            color: #e2e8f0;
        }
        
        .movie-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            background: linear-gradient(145deg, #2d3748 0%, #4a5568 100%);
            border: 1px solid #4a5568;
        }
        
        .movie-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }
        
        .hero-gradient {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        }
        
        .ad-container {
            background: linear-gradient(145deg, #2d3748 0%, #4a5568 100%);
            border: 2px dashed #667eea;
            min-height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 12px;
        }
        
        .play-button {
            transition: all 0.3s ease;
        }
        
        .play-button:hover {
            transform: scale(1.1);
            background-color: #e53e3e;
        }
        
        .category-filter {
            transition: all 0.3s ease;
        }
        
        .category-filter:hover {
            background-color: #4a5568;
            transform: scale(1.05);
        }
    </style>
</head>
<body class="min-h-screen">
    <!-- Header -->
    <header class="bg-gray-900 bg-opacity-90 backdrop-blur-sm border-b border-gray-700 sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center space-x-4">
                    <div class="w-10 h-10 bg-red-600 rounded-lg flex items-center justify-center">
                        <i class="fas fa-film text-white text-xl"></i>
                    </div>
                    <h1 class="text-2xl font-bold text-white">CinePúblico</h1>
                </div>
                
                <nav class="hidden md:flex space-x-6">
                    <a href="#" class="text-gray-300 hover:text-white transition-colors">Inicio</a>
                    <a href="#" class="text-gray-300 hover:text-white transition-colors">Películas</a>
                    <a href="#" class="text-gray-300 hover:text-white transition-colors">Series</a>
                    <a href="#" class="text-gray-300 hover:text-white transition-colors">Categorías</a>
                </nav>
                
                <div class="flex items-center space-x-4">
                    <button class="bg-red-600 hover:bg-red-700 text-white px-6 py-2 rounded-lg font-semibold transition-colors">
                        <i class="fas fa-user-plus mr-2"></i>Registrarse
                    </button>
                    <button class="bg-gray-700 hover:bg-gray-600 text-white px-6 py-2 rounded-lg font-semibold transition-colors">
                        <i class="fas fa-sign-in-alt mr-2"></i>Ingresar
                    </button>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero-gradient py-20">
        <div class="container mx-auto px-4">
            <div class="text-center">
                <h2 class="text-4xl md:text-6xl font-bold text-white mb-6">
                    Disfruta Cine Clásico <span class="text-red-400">Gratis</span>
                </h2>
                <p class="text-xl text-gray-100 mb-8 max-w-2xl mx-auto">
                    Películas de dominio público en español, completamente legales y gratuitas para tu entretenimiento.
                </p>
                <div class="flex justify-center space-x-4">
                    <button class="bg-white text-purple-700 px-8 py-3 rounded-lg font-semibold text-lg hover:bg-gray-100 transition-colors">
                        <i class="fas fa-play-circle mr-2"></i>Ver Ahora
                    </button>
                    <button class="bg-transparent border-2 border-white text-white px-8 py-3 rounded-lg font-semibold text-lg hover:bg-white hover:text-purple-700 transition-colors">
                        <i class="fas fa-info-circle mr-2"></i>Más Info
                    </button>
                </div>
            </div>
        </div>
    </section>

    <!-- Ad Banner -->
    <div class="container mx-auto px-4 py-6">
        <div class="ad-container">
            <div class="text-center text-gray-400">
                <i class="fas fa-ad text-3xl mb-2"></i>
                <p>Espacio Publicitario</p>
                <p class="text-sm">Anúnciate aquí y llega a miles de cinéfilos</p>
            </div>
        </div>
    </div>

    <!-- Categories -->
    <section class="py-12 bg-gray-800">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-white mb-8 text-center">Categorías Populares</h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <div class="category-filter bg-gray-700 p-4 rounded-lg text-center cursor-pointer hover:bg-gray-600 transition-colors">
                    <i class="fas fa-theater-masks text-3xl text-red-400 mb-2"></i>
                    <h3 class="font-semibold">Clásicos</h3>
                </div>
                <div class="category-filter bg-gray-700 p-4 rounded-lg text-center cursor-pointer hover:bg-gray-600 transition-colors">
                    <i class="fas fa-ghost text-3xl text-red-400 mb-2"></i>
                    <h3 class="font-semibold">Terror</h3>
                </div>
                <div class="category-filter bg-gray-700 p-4 rounded-lg text-center cursor-pointer hover:bg-gray-600 transition-colors">
                    <i class="fas fa-laugh text-3xl text-red-400 mb-2"></i>
                    <h3 class="font-semibold">Comedia</h3>
                </div>
                <div class="category-filter bg-gray-700 p-4 rounded-lg text-center cursor-pointer hover:bg-gray-600 transition-colors">
                    <i class="fas fa-heart text-3xl text-red-400 mb-2"></i>
                    <h3 class="font-semibold">Romance</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Featured Movies -->
    <section class="py-16">
        <div class="container mx-auto px-4">
            <div class="flex justify-between items-center mb-8">
                <h2 class="text-3xl font-bold text-white">Películas Destacadas</h2>
                <a href="#" class="text-red-400 hover:text-red-300 transition-colors">
                    Ver todas <i class="fas fa-arrow-right ml-2"></i>
                </a>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Movie 1 -->
                <div class="movie-card rounded-lg overflow-hidden">
                    <div class="relative">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/8568ccaf-dd94-4973-939b-c92ca7c0705c.png" alt="Póster de la película clásica Metrópolis con robots futuristas y arquitectura art déco en blanco y negro" class="w-full h-64 object-cover" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/50c2dfd6-af02-4c27-aa47-a5fdac1d8335.png?text=Imagen+no+disponible'">
                        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 hover:opacity-100 transition-opacity flex items-center justify-center">
                            <button class="play-button bg-red-600 text-white p-4 rounded-full">
                                <i class="fas fa-play text-xl"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-semibold text-white mb-2">Metrópolis</h3>
                        <p class="text-gray-400 text-sm mb-3">1927 • Ciencia Ficción • 2h 33m</p>
                        <div class="flex justify-between items-center">
                            <span class="bg-yellow-500 text-black px-2 py-1 rounded text-sm font-semibold">8.3/10</span>
                            <span class="text-gray-400 text-sm">HD</span>
                        </div>
                    </div>
                </div>

                <!-- Movie 2 -->
                <div class="movie-card rounded-lg overflow-hidden">
                    <div class="relative">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/673a8777-fadf-451e-b57f-36b39d729e9f.png" alt="Póster de Nosferatu mostrando al vampiro con uñas largas y expresión siniestra en estilo expresionista alemán" class="w-full h-64 object-cover" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/cf84bf13-db80-4e93-b967-9b4bb8e9615a.png?text=Imagen+no+disponible'">
                        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 hover:opacity-100 transition-opacity flex items-center justify-center">
                            <button class="play-button bg-red-600 text-white p-4 rounded-full">
                                <i class="fas fa-play text-xl"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-semibold text-white mb-2">Nosferatu</h3>
                        <p class="text-gray-400 text-sm mb-3">1922 • Terror • 1h 34m</p>
                        <div class="flex justify-between items-center">
                            <span class="bg-yellow-500 text-black px-2 py-1 rounded text-sm font-semibold">7.9/10</span>
                            <span class="text-gray-400 text-sm">HD</span>
                        </div>
                    </div>
                </div>

                <!-- Movie 3 -->
                <div class="movie-card rounded-lg overflow-hidden">
                    <div class="relative">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6d6d8b21-bebe-4721-a385-678d5eca802a.png" alt="Póster de Tiempos Modernos con Charlie Chaplin atrapado en engranajes industriales con su característico bigote y sombrero" class="w-full h-64 object-cover" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/86cd4f08-8a12-4085-9217-376faa233935.png'">
                        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 hover:opacity-100 transition-opacity flex items-center justify-center">
                            <button class="play-button bg-red-600 text-white p-4 rounded-full">
                                <i class="fas fa-play text-xl"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-semibold text-white mb-2">Tiempos Modernos</h3>
                        <p class="text-gray-400 text-sm mb-3">1936 • Comedia • 1h 27m</p>
                        <div class="flex justify-between items-center">
                            <span class="bg-yellow-500 text-black px-2 py-1 rounded text-sm font-semibold">8.5/10</span>
                            <span class="text-gray-400 text-sm">HD</span>
                        </div>
                    </div>
                </div>

                <!-- Movie 4 -->
                <div class="movie-card rounded-lg overflow-hidden">
                    <div class="relative">
                        <img src="https://placehold.co/400x600/4a5568/e2e8f0" alt="Póster de El Acorazado Potemkin con marineros en rebelión y escenas dramáticas en blanco y negro del famoso acorazado" class="w-full h-64 object-cover" onerror="this.src='https://placehold.co/400x600/4a5568/e2e8f0?text=Imagen+no+disponible'">
                        <div class="absolute inset-0 bg-black bg-opacity-50 opacity-0 hover:opacity-100 transition-opacity flex items-center justify-center">
                            <button class="play-button bg-red-600 text-white p-4 rounded-full">
                                <i class="fas fa-play text-xl"></i>
                            </button>
                        </div>
                    </div>
                    <div class="p-4">
                        <h3 class="text-xl font-semibold text-white mb-2">El Acorazado Potemkin</h3>
                        <p class="text-gray-400 text-sm mb-3">1925 • Drama • 1h 15m</p>
                        <div class="flex justify-between items-center">
                            <span class="bg-yellow-500 text-black px-2 py-1 rounded text-sm font-semibold">8.0/10</span>
                            <span class="text-gray-400 text-sm">HD</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sidebar Ad -->
    <div class="container mx-auto px-4 py-8">
        <div class="ad-container">
            <div class="text-center p-6">
                <i class="fas fa-megaphone text-4xl text-red-400 mb-4"></i>
                <h3 class="text-xl font-semibold text-white mb-2">Tu Anuncio Aquí</h3>
                <p class="text-gray-400">Llega a miles de amantes del cine clásico</p>
                <button class="mt-4 bg-red-600 hover:bg-red-700 text-white px-6 py-2 rounded-lg transition-colors">
                    Anunciarse
                </button>
            </div>
        </div>
    </div>

    <!-- All Movies Grid -->
    <section class="py-16 bg-gray-800">
        <div class="container mx-auto px-4">
            <h2 class="text-3xl font-bold text-white mb-8 text-center">Todas las Películas</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-6">
                <!-- Additional movie cards would go here -->
                <div class="movie-card rounded-lg p-4 text-center">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/6b49a4d2-faac-475a-b1d0-691692580311.png" alt="Póster de película clásica El Gabinete del Doctor Caligari con diseño expresionista alemán" class="w-full h-48 object-cover rounded mb-3" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/4a180916-0570-4609-9b9b-3811fa417db8.png?text=Imagen+no+disponible'">
                    <h4 class="text-white font-semibold">El Gabinete del Dr. Caligari</h4>
                </div>
                <div class="movie-card rounded-lg p-4 text-center">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/ab99afaf-6d32-4295-87fc-9406138b2d49.png" alt="Póster de La Pasión de Juana de Arco con rostro dramático de la protagonista" class="w-full h-48 object-cover rounded mb-3" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/fed11021-6d49-4ccc-908f-788e79931e80.png?text=Imagen+no+disponible'">
                    <h4 class="text-white font-semibold">La Pasión de Juana de Arco</h4>
                </div>
                <div class="movie-card rounded-lg p-4 text-center">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/d263df4b-78ec-4787-96d0-74ba5f0ef1be.png" alt="Póster de El Hombre de la Cámara mostrando técnicas cinematográficas soviéticas" class="w-full h-48 object-cover rounded mb-3" onerror="this.src='https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/10b59d52-f382-4a9c-9191-12bfada68c42.png'">
                    <h4 class="text-white font-semibold">El Hombre de la Cámara</h4>
                </div>
                <div class="movie-card rounded-lg p-4 text-center">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/170a754b-01d0-4d4e-91e8-b3e8f7e5cda1.png" alt="Póster de Luzes da Cidade con Chaplin en situación cómica característica" class="w-full h-48 object-cover rounded mb-3" onerror="this.src='https://placehold.co/200x300/4a5568/e2e8f0?text=Imagen+no+disponible'">
                    <h4 class="text-white font-semibold">Luces de la Ciudad</h4>
                </div>
                <div class="movie-card rounded-lg p-4 text-center">
                    <img src="https://placehold.co/200x300/4a5568/e2e8f0" alt="Póster de El Gran Dictador con Chaplin parodiando a Hitler en blanco y negro" class="w-full h-48 object-cover rounded mb-3" onerror="this.src='https://placehold.co/200x300/4a5568/e2e8f0?text=Imagen+no+disponible'">
                    <h4 class="text-white font-semibold">El Gran Dictador</h4>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="text-white text-xl font-semibold mb-4">CinePúblico</h3>
                    <p class="text-gray-400">Tu destino para películas de dominio público en español. Contenido legal y gratuito.</p>
                </div>
                <div>
                    <h4 class="text-white font-semibold mb-4">Enlaces Rápidos</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Inicio</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Películas</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Series</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Categorías</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-white font-semibold mb-4">Legal</h4>
                    <ul class="space-y-2">
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Términos de Servicio</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Política de Privacidad</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-white transition-colors">DMCA</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="text-white font-semibold mb-4">Publicidad</h4>
                    <p class="text-gray-400 mb-4">¿Interesado en anunciarte?</p>
                    <button class="bg-red-600 hover:bg-red-700 text-white px-4 py-2 rounded transition-colors">
                        Contactar
                    </button>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-8 text-center">
                <p class="text-gray-400">© 2024 CinePúblico. Todos los derechos reservados para los respectivos titulares.</p>
            </div>
        </div>
    </footer>

    <script>
        // Simple JavaScript for interactivity
        document.addEventListener('DOMContentLoaded', function() {
            // Play button functionality
            const playButtons = document.querySelectorAll('.play-button');
            playButtons.forEach(button => {
                button.addEventListener('click', function() {
                    alert('Función de reproducción simulada. En una implementación real, esto iniciaría el video.');
                });
            });

            // Category filter functionality
            const categoryFilters = document.querySelectorAll('.category-filter');
            categoryFilters.forEach(filter => {
                filter.addEventListener('click', function() {
                    const category = this.querySelector('h3').textContent;
                    alert(`Filtrando por categoría: ${category}`);
                });
            });

            // Simulate ad clicks
            const adContainers = document.querySelectorAll('.ad-container');
            adContainers.forEach(ad => {
                ad.addEventListener('click', function() {
                    alert('Redirigiendo a página de publicidad. En una implementación real, esto llevaría a la página del anunciante.');
                });
            });
        });
    </script>
</body>
</html>
