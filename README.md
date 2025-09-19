# Playbook_GR<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Playbook operacional com IA para gerenciar workflow completo de dropshipping">
    <meta name="keywords" content="dropshipping, workflow, ai, playbook, automação">
    <title>Playbook Dropshipping AI - Workflow Completo</title>
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #3b82f6;
            --secondary: #8b5cf6;
            --success: #10b981;
            --warning: #f59e0b;
            --danger: #ef4444;
        }

        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .glass-effect {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .step-card {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            cursor: pointer;
        }

        .step-card:hover {
            transform: translateY(-5px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0,0,0,0.2);
        }

        .completed {
            background: linear-gradient(135deg, #10b981, #059669) !important;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .animate-fade-in {
            animation: fadeIn 0.5s ease-out;
        }
    </style>
</head>
<body>
    <!-- Container Principal -->
    <div class="min-h-screen p-4 md:p-8">
        <div class="max-w-7xl mx-auto">
            
            <!-- Header -->
            <header class="text-center mb-10 animate-fade-in">
                <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">
                    🚀 Workflow AI Dropshipping
                </h1>
                <p class="text-white/80 text-lg">
                    Sistema completo de gestão com especialistas de IA
                </p>
            </header>

            <!-- Barra de Progresso -->
            <div class="glass-effect rounded-xl p-6 mb-8">
                <div class="flex justify-between items-center mb-4">
                    <h3 class="font-semibold">Progresso do Pipeline</h3>
                    <span class="text-sm text-gray-600">
                        <span id="completed">0</span> de 6 etapas
                    </span>
                </div>
                <div class="w-full bg-gray-200 rounded-full h-3">
                    <div id="progressBar" class="bg-gradient-to-r from-blue-500 to-purple-500 h-3 rounded-full transition-all duration-500" style="width: 0%"></div>
                </div>
            </div>

            <!-- Grid de Cards -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                
                <!-- Card 1: Caçador de Tendências -->
                <div class="step-card glass-effect rounded-2xl p-6" data-step="1">
                    <div class="flex items-center mb-4">
                        <div class="w-16 h-16 bg-red-500 rounded-full flex items-center justify-center text-white text-2xl">
                            🎯
                        </div>
                        <div class="ml-4">
                            <h3 class="text-xl font-bold">Caçador de Tendências</h3>
                            <p class="text-sm text-gray-600">Mineração de produtos</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <a href="https://chatgpt.com/g/g-68c90a7117208191b8431e847f539881-cacador-de-tendencias" 
                           target="_blank" 
                           class="block w-full px-4 py-2 bg-red-500 text-white text-center rounded-lg hover:bg-red-600 transition">
                            <i class="fas fa-external-link-alt mr-2"></i>Abrir GPT
                        </a>
                        
                        <div class="bg-red-50 border-l-4 border-red-400 p-3 rounded">
                            <p class="text-xs font-semibold text-red-800">Prompt Sugerido:</p>
                            <p class="text-xs text-red-700 mt-1">
                                "Analise tendências de inovações práticas para [nicho]..."
                            </p>
                        </div>
                        
                        <label class="flex items-center">
                            <input type="checkbox" class="mr-2" onchange="updateProgress()">
                            <span class="text-sm">Etapa concluída</span>
                        </label>
                    </div>
                </div>

                <!-- Card 2: O Analista -->
                <div class="step-card glass-effect rounded-2xl p-6" data-step="2">
                    <div class="flex items-center mb-4">
                        <div class="w-16 h-16 bg-green-500 rounded-full flex items-center justify-center text-white text-2xl">
                            🕵️
                        </div>
                        <div class="ml-4">
                            <h3 class="text-xl font-bold">O Analista</h3>
                            <p class="text-sm text-gray-600">Análise de viabilidade</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <a href="https://chatgpt.com/g/g-68c8b9a2e6a88191870120d5c65b02c4-analista-de-produtos-vencedores" 
                           target="_blank" 
                           class="block w-full px-4 py-2 bg-green-500 text-white text-center rounded-lg hover:bg-green-600 transition">
                            <i class="fas fa-external-link-alt mr-2"></i>Abrir GPT
                        </a>
                        
                        <div class="bg-green-50 border-l-4 border-green-400 p-3 rounded">
                            <p class="text-xs font-semibold text-green-800">Input Hierárquico:</p>
                            <p class="text-xs text-green-700 mt-1">
                                1. Anúncio viral | 2. Página produto | 3. Link fornecedor
                            </p>
                        </div>
                        
                        <label class="flex items-center">
                            <input type="checkbox" class="mr-2" onchange="updateProgress()">
                            <span class="text-sm">Etapa concluída</span>
                        </label>
                    </div>
                </div>

                <!-- Card 3: Estrategista -->
                <div class="step-card glass-effect rounded-2xl p-6" data-step="3">
                    <div class="flex items-center mb-4">
                        <div class="w-16 h-16 bg-gray-600 rounded-full flex items-center justify-center text-white text-2xl">
                            ♟️
                        </div>
                        <div class="ml-4">
                            <h3 class="text-xl font-bold">Estrategista</h3>
                            <p class="text-sm text-gray-600">Classificação do produto</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <a href="https://chatgpt.com/g/g-68cb0e4fc8e88191a22611f4cd549391-estrategista-de-portifolio" 
                           target="_blank" 
                           class="block w-full px-4 py-2 bg-gray-600 text-white text-center rounded-lg hover:bg-gray-700 transition">
                            <i class="fas fa-external-link-alt mr-2"></i>Abrir GPT
                        </a>
                        
                        <div class="bg-gray-50 border-l-4 border-gray-400 p-3 rounded">
                            <p class="text-xs font-semibold text-gray-800">Classificação:</p>
                            <p class="text-xs text-gray-700 mt-1">
                                💰 Lucrativo | 🏆 Vencedor
                            </p>
                        </div>
                        
                        <label class="flex items-center">
                            <input type="checkbox" class="mr-2" onchange="updateProgress()">
                            <span class="text-sm">Etapa concluída</span>
                        </label>
                    </div>
                </div>

                <!-- Card 4: Copywriter -->
                <div class="step-card glass-effect rounded-2xl p-6" data-step="4">
                    <div class="flex items-center mb-4">
                        <div class="w-16 h-16 bg-blue-500 rounded-full flex items-center justify-center text-white text-2xl">
                            ✍️
                        </div>
                        <div class="ml-4">
                            <h3 class="text-xl font-bold">Copywriter</h3>
                            <p class="text-sm text-gray-600">Criação de copy</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <a href="https://chatgpt.com/g/g-68c8c34c285081919757c4d7d1efbc06-copywriter-estrategista-45" 
                           target="_blank" 
                           class="block w-full px-4 py-2 bg-blue-500 text-white text-center rounded-lg hover:bg-blue-600 transition">
                            <i class="fas fa-external-link-alt mr-2"></i>Abrir GPT
                        </a>
                        
                        <div class="bg-blue-50 border-l-4 border-blue-400 p-3 rounded">
                            <p class="text-xs font-semibold text-blue-800">Elementos essenciais:</p>
                            <p class="text-xs text-blue-700 mt-1">
                                Headline | Benefícios | CTA | Garantia
                            </p>
                        </div>
                        
                        <label class="flex items-center">
                            <input type="checkbox" class="mr-2" onchange="updateProgress()">
                            <span class="text-sm">Etapa concluída</span>
                        </label>
                    </div>
                </div>

                <!-- Card 5: Mestre dos Criativos -->
                <div class="step-card glass-effect rounded-2xl p-6" data-step="5">
                    <div class="flex items-center mb-4">
                        <div class="w-16 h-16 bg-purple-500 rounded-full flex items-center justify-center text-white text-2xl">
                            🎬
                        </div>
                        <div class="ml-4">
                            <h3 class="text-xl font-bold">Mestre Criativos</h3>
                            <p class="text-sm text-gray-600">Roteiro de vídeo</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <a href="https://chatgpt.com/g/g-68c8c73797288191a954864bacfeb06d-mestre-dos-criativos" 
                           target="_blank" 
                           class="block w-full px-4 py-2 bg-purple-500 text-white text-center rounded-lg hover:bg-purple-600 transition">
                            <i class="fas fa-external-link-alt mr-2"></i>Abrir GPT
                        </a>
                        
                        <div class="bg-purple-50 border-l-4 border-purple-400 p-3 rounded">
                            <p class="text-xs font-semibold text-purple-800">Modo de criação:</p>
                            <p class="text-xs text-purple-700 mt-1">
                                Storyboard detalhado com cenas e transições
                            </p>
                        </div>
                        
                        <label class="flex items-center">
                            <input type="checkbox" class="mr-2" onchange="updateProgress()">
                            <span class="text-sm">Etapa concluída</span>
                        </label>
                    </div>
                </div>

                <!-- Card 6: Artista Digital -->
                <div class="step-card glass-effect rounded-2xl p-6" data-step="6">
                    <div class="flex items-center mb-4">
                        <div class="w-16 h-16 bg-amber-500 rounded-full flex items-center justify-center text-white text-2xl">
                            🎨
                        </div>
                        <div class="ml-4">
                            <h3 class="text-xl font-bold">Artista Digital</h3>
                            <p class="text-sm text-gray-600">Geração de imagens</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <a href="https://chatgpt.com/g/g-68c8ce400e588191864005c1be2eca80-artista-digital-prompt-engineer" 
                           target="_blank" 
                           class="block w-full px-4 py-2 bg-amber-500 text-white text-center rounded-lg hover:bg-amber-600 transition">
                            <i class="fas fa-external-link-alt mr-2"></i>Abrir GPT
                        </a>
                        
                        <div class="bg-amber-50 border-l-4 border-amber-400 p-3 rounded">
                            <p class="text-xs font-semibold text-amber-800">Formatos de saída:</p>
                            <p class="text-xs text-amber-700 mt-1">
                                Feed: 1080x1080 | Stories: 1080x1920
                            </p>
                        </div>
                        
                        <label class="flex items-center">
                            <input type="checkbox" class="mr-2" onchange="updateProgress()">
                            <span class="text-sm">Etapa concluída</span>
                        </label>
                    </div>
                </div>

            </div>

            <!-- Botão Reset -->
            <div class="text-center mt-8">
                <button onclick="resetAll()" class="px-6 py-3 bg-red-500 text-white rounded-lg hover:bg-red-600 transition">
                    <i class="fas fa-redo mr-2"></i>Resetar Workflow
                </button>
            </div>

        </div>
    </div>

    <script>
        function updateProgress() {
            const checkboxes = document.querySelectorAll('input[type="checkbox"]');
            const checked = document.querySelectorAll('input[type="checkbox"]:checked');
            const progress = (checked.length / checkboxes.length) * 100;
            
            document.getElementById('progressBar').style.width = progress + '%';
            document.getElementById('completed').textContent = checked.length;
            
            // Atualizar visual dos cards
            checkboxes.forEach((checkbox, index) => {
                const card = checkbox.closest('.step-card');
                if (checkbox.checked) {
                    card.classList.add('completed');
                } else {
                    card.classList.remove('completed');
                }
            });
            
            // Salvar no localStorage
            const state = Array.from(checkboxes).map(cb => cb.checked);
            localStorage.setItem('workflowState', JSON.stringify(state));
        }

        function resetAll() {
            if (confirm('Deseja resetar todo o workflow?')) {
                document.querySelectorAll('input[type="checkbox"]').forEach(cb => {
                    cb.checked = false;
                });
                updateProgress();
                localStorage.removeItem('workflowState');
            }
        }

        // Restaurar estado ao carregar
        window.addEventListener('DOMContentLoaded', () => {
            const savedState = localStorage.getItem('workflowState');
            if (savedState) {
                const state = JSON.parse(savedState);
                const checkboxes = document.querySelectorAll('input[type="checkbox"]');
                checkboxes.forEach((cb, index) => {
                    cb.checked = state[index] || false;
                });
                updateProgress();
            }
        });
    </script>
</body>
</html>
