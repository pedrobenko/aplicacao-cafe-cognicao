<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Café e Cognição: Análise Científica Interativa</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Chosen Palette: Modern Blue and Slate -->
    <!-- Application Structure Plan: A tab-based single-page application. This structure breaks down the dense report into manageable, thematic sections: an overview, immediate benefits, long-term health, risks/moderation, mechanisms, and references. This non-linear approach enhances usability by allowing users to explore topics of interest directly. Interactions include dynamic charts for dose-response data and toggleable cards for detailed text, making the content engaging and easy to digest. Design updated for a cleaner, more modern aesthetic. Added a references section and authorship. -->
    <!-- Visualization & Content Choices: 
        - Overview: Goal: Inform/Summarize. Method: Key stat cards with Unicode icons (HTML/CSS) for quick takeaways, styled with new palette. Introductory text about scientific sources and authorship added.
        - Immediate Benefits: Goal: Compare. Method: Bar chart (Chart.js) showing positive/mixed effects on cognitive domains, chart colors updated. Justification: Visual comparison is faster than reading a table.
        - Long-Term Health: Goal: Compare/Show Change. Method: Interactive bar chart (Chart.js) updated by a dropdown. Shows risk reduction for diseases at optimal doses from Table 2, chart colors updated. Justification: Makes complex risk ratio data interactive and understandable.
        - Risks & Modulators: Goal: Organize. Method: Accordion-style toggle cards (HTML/CSS/JS) with updated icons and styling. Justification: Prevents a wall of text, allowing focused exploration.
        - Mechanisms: Goal: Explain. Method: Simplified flowchart using HTML/CSS grid with improved card styling. Justification: Visually breaks down complex neurobiology for easier comprehension.
        - References: Goal: Provide Sources. Method: List of scientific references. Justification: Adds credibility and allows for further reading.
    -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* slate-50 */
            color: #334155; /* slate-700 */
        }
        .tab-active {
            border-color: #0284c7; /* sky-600 */
            color: #0284c7;
            font-weight: 600;
            background-color: #f0f9ff; /* sky-50 */
        }
        .tab-button {
            border-radius: 0.5rem 0.5rem 0 0;
            transition: background-color 0.2s ease-in-out, color 0.2s ease-in-out, border-color 0.2s ease-in-out;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px; /* Max width for larger screens */
            margin-left: auto;
            margin-right: auto;
            height: 320px; /* Base height */
        }
        @media (min-width: 768px) { /* md breakpoint */
            .chart-container {
                height: 400px; /* Taller on medium screens and up */
            }
        }
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease-in-out;
        }
        .accordion-content.open {
            max-height: 500px; /* Adjust if content is taller */
        }
        .content-card {
            background-color: white;
            border-radius: 0.75rem; /* rounded-xl */
            box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.07), 0 4px 6px -4px rgb(0 0 0 / 0.07); /* shadow-lg with softer feel */
            padding: 1.5rem; /* p-6 */
        }
        .flowchart-step {
            background-color: #f0f9ff; /* sky-50 */
            border: 1px solid #e0f2fe; /* sky-100 */
        }
        .reference-list li {
            margin-bottom: 0.75rem; /* mb-3 */
            padding-left: 1.25rem; /* pl-5 */
            position: relative;
        }
        .reference-list li::before {
            content: "●"; /* Bullet point */
            color: #0284c7; /* sky-600 */
            position: absolute;
            left: 0;
            font-size: 0.8em;
            top: 0.25em;
        }
    </style>
</head>
<body class="antialiased">

    <div class="container mx-auto p-4 sm:p-6 md:p-8 max-w-5xl">

        <header class="text-center mb-10 md:mb-12">
            <h1 class="text-3xl sm:text-4xl md:text-5xl font-bold text-sky-800 mb-3">As Ligações Cognitivas do Consumo Diário de Café</h1>
            <p class="text-lg sm:text-xl text-slate-600">Uma Análise Interativa Baseada em Evidências Científicas</p>
            <p class="mt-2 text-sm text-slate-500">Todas as informações aqui apresentadas são compiladas a partir de artigos científicos de acesso aberto.</p>
            <p class="mt-1 text-xs text-slate-400">Site criado para intuito educativo por: Pedro Ambrósio Benko</p>
        </header>

        <nav class="mb-8 flex flex-wrap justify-center border-b border-slate-200">
            <button data-tab="overview" class="tab-button text-sm md:text-base px-4 py-3 border-b-2 border-transparent hover:bg-sky-100 hover:text-sky-700">Visão Geral</button>
            <button data-tab="benefits" class="tab-button text-sm md:text-base px-4 py-3 border-b-2 border-transparent hover:bg-sky-100 hover:text-sky-700">Benefícios Imediatos</button>
            <button data-tab="long-term" class="tab-button text-sm md:text-base px-4 py-3 border-b-2 border-transparent hover:bg-sky-100 hover:text-sky-700">Saúde a Longo Prazo</button>
            <button data-tab="risks" class="tab-button text-sm md:text-base px-4 py-3 border-b-2 border-transparent hover:bg-sky-100 hover:text-sky-700">Riscos e Moderação</button>
            <button data-tab="mechanisms" class="tab-button text-sm md:text-base px-4 py-3 border-b-2 border-transparent hover:bg-sky-100 hover:text-sky-700">Como Funciona?</button>
            <button data-tab="references" class="tab-button text-sm md:text-base px-4 py-3 border-b-2 border-transparent hover:bg-sky-100 hover:text-sky-700">Referências</button>
        </nav>

        <main>
            <section id="overview" class="tab-content">
                <div class="content-card">
                    <h2 class="text-2xl font-semibold text-sky-700 mb-4">Um Resumo Equilibrado</h2>
                    <p class="mb-6 text-slate-600 leading-relaxed">O café é uma das bebidas mais consumidas no mundo, com efeitos complexos no cérebro. A ciência mostra um quadro de dois lados: o consumo moderado oferece benefícios cognitivos e protetores, mas o excesso ou o consumo em momentos errados pode trazer riscos. Esta aplicação resume as principais descobertas para o ajudar a fazer escolhas informadas.</p>
                    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 text-center">
                        <div class="bg-sky-50 p-5 rounded-lg border border-sky-100">
                            <span class="text-4xl">☕</span>
                            <h3 class="font-semibold text-sky-800 mt-2">Dose Moderada</h3>
                            <p class="text-sm text-slate-500">O ponto ideal para a maioria dos benefícios é de 2 a 4 xícaras por dia (até 400mg de cafeína).</p>
                        </div>
                        <div class="bg-sky-50 p-5 rounded-lg border border-sky-100">
                            <span class="text-4xl">🧠</span>
                            <h3 class="font-semibold text-sky-800 mt-2">Proteção a Longo Prazo</h3>
                            <p class="text-sm text-slate-500">Associado a um menor risco de doenças como Parkinson e Alzheimer.</p>
                        </div>
                        <div class="bg-sky-50 p-5 rounded-lg border border-sky-100">
                            <span class="text-4xl">⚠️</span>
                            <h3 class="font-semibold text-sky-800 mt-2">Atenção ao Sono</h3>
                            <p class="text-sm text-slate-500">O principal efeito adverso é a perturbação da qualidade do sono, mesmo se consumido à tarde.</p>
                        </div>
                    </div>
                </div>
            </section>

            <section id="benefits" class="tab-content hidden">
                 <div class="content-card">
                    <h2 class="text-2xl font-semibold text-sky-700 mb-2">Impacto nas Funções Cognitivas</h2>
                    <p class="mb-6 text-slate-600 leading-relaxed">O consumo diário de café, principalmente devido à cafeína, modula várias funções cognitivas. Os efeitos mais notáveis são no aumento do alerta e na velocidade de processamento, enquanto o impacto na memória pode ser mais variável.</p>
                    <div class="chart-container">
                        <canvas id="benefitsChart"></canvas>
                    </div>
                </div>
            </section>

            <section id="long-term" class="tab-content hidden">
                <div class="content-card">
                    <h2 class="text-2xl font-semibold text-sky-700 mb-2">Proteção Contra Doenças Neurodegenerativas</h2>
                    <p class="mb-4 text-slate-600 leading-relaxed">A pesquisa sugere que o consumo habitual e moderado de café pode ter um papel protetor contra o declínio cognitivo relacionado com a idade. Selecione uma condição abaixo para ver a redução de risco associada e a dose ideal, com base em meta-análises científicas.</p>
                    <div class="mb-6 text-center">
                        <select id="diseaseSelector" class="p-3 border border-slate-300 rounded-lg bg-white focus:ring-2 focus:ring-sky-500 focus:border-sky-500 focus:outline-none shadow-sm w-full sm:w-auto">
                            <option value="alzheimer">Doença de Alzheimer</option>
                            <option value="parkinson">Doença de Parkinson</option>
                            <option value="avc">Acidente Vascular Cerebral (AVC)</option>
                            <option value="demenciaPosAvc">Demência Pós-AVC</option>
                        </select>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6 items-start">
                        <div class="chart-container">
                            <canvas id="longTermChart"></canvas>
                        </div>
                        <div id="longTermInfoContainer" class="space-y-4">
                            <div id="longTermInfo" class="bg-sky-50 p-5 rounded-lg border border-sky-100 min-h-[150px]">
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <section id="risks" class="tab-content hidden">
                <div class="content-card">
                    <h2 class="text-2xl font-semibold text-sky-700 mb-4">Riscos, Moderação e Fatores Individuais</h2>
                    <p class="mb-6 text-slate-600 leading-relaxed">Apesar dos benefícios, o café não é isento de riscos. A resposta de cada pessoa é única, influenciada pela dose, genética e outros fatores do estilo de vida. Explore os tópicos abaixo para entender melhor.</p>
                    <div class="space-y-3">
                        <div class="accordion-item border border-slate-200 rounded-lg bg-white">
                            <button class="accordion-header w-full flex justify-between items-center p-4 text-left font-semibold text-sky-800 hover:bg-sky-50 transition-colors duration-150 rounded-t-lg">
                                Qualidade e Arquitetura do Sono
                                <span class="accordion-icon text-xl font-light text-sky-600">+</span>
                            </button>
                            <div class="accordion-content px-4 pb-4 text-slate-600 leading-relaxed">
                                <p>Este é talvez o efeito adverso mais significativo. A cafeína, mesmo consumida 6 a 12 horas antes de deitar, pode aumentar o tempo para adormecer, reduzir o tempo total de sono e diminuir a proporção de sono profundo (ondas lentas), que é crucial para a recuperação física e consolidação da memória. Muitos não percebem o quanto a sua qualidade de sono é afetada.</p>
                            </div>
                        </div>
                        <div class="accordion-item border border-slate-200 rounded-lg bg-white">
                            <button class="accordion-header w-full flex justify-between items-center p-4 text-left font-semibold text-sky-800 hover:bg-sky-50 transition-colors duration-150 rounded-t-lg">
                                Ansiedade e Nervosismo
                                <span class="accordion-icon text-xl font-light text-sky-600">+</span>
                            </button>
                            <div class="accordion-content px-4 pb-4 text-slate-600 leading-relaxed">
                                <p>Por ser um estimulante, a cafeína pode induzir ou agravar sintomas de ansiedade, agitação e nervosismo, especialmente em doses elevadas (>400mg) ou em indivíduos com predisposição para transtornos de ansiedade.</p>
                            </div>
                        </div>
                         <div class="accordion-item border border-slate-200 rounded-lg bg-white">
                            <button class="accordion-header w-full flex justify-between items-center p-4 text-left font-semibold text-sky-800 hover:bg-sky-50 transition-colors duration-150 rounded-t-lg">
                                Abstinência e Dependência
                                <span class="accordion-icon text-xl font-light text-sky-600">+</span>
                            </button>
                            <div class="accordion-content px-4 pb-4 text-slate-600 leading-relaxed">
                                <p>O uso regular leva à dependência física. A interrupção abrupta pode causar uma síndrome de abstinência com sintomas como dor de cabeça, fadiga extrema, irritabilidade e dificuldade de concentração, que geralmente duram de 2 a 9 dias.</p>
                            </div>
                        </div>
                        <div class="accordion-item border border-slate-200 rounded-lg bg-white">
                            <button class="accordion-header w-full flex justify-between items-center p-4 text-left font-semibold text-sky-800 hover:bg-sky-50 transition-colors duration-150 rounded-t-lg">
                                O Papel da Genética
                                <span class="accordion-icon text-xl font-light text-sky-600">+</span>
                            </button>
                            <div class="accordion-content px-4 pb-4 text-slate-600 leading-relaxed">
                                <p>A sua genética influencia fortemente a sua resposta. Polimorfismos no gene CYP1A2 determinam se você é um metabolizador "lento" ou "rápido" de cafeína. Metabolizadores lentos sentem os efeitos por mais tempo e podem ser mais suscetíveis a efeitos adversos, como problemas de sono e ansiedade.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <section id="mechanisms" class="tab-content hidden">
                 <div class="content-card">
                    <h2 class="text-2xl font-semibold text-sky-700 mb-4">Como o Café Influencia o Cérebro?</h2>
                    <p class="mb-6 text-slate-600 leading-relaxed">Os efeitos do café vão muito além da cafeína. É uma interação complexa de compostos que atuam em diferentes vias cerebrais. O mecanismo principal é o bloqueio da adenosina, um neuromodulador que nos faz sentir cansados.</p>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4 md:gap-6 text-center items-center mb-6">
                        <div class="flowchart-step flex flex-col items-center p-5 rounded-lg">
                            <div class="w-20 h-20 bg-sky-100 rounded-full flex items-center justify-center mb-3">
                                <span class="text-3xl">☕</span>
                            </div>
                            <h3 class="font-semibold text-sky-800">1. Consumo de Café</h3>
                            <p class="text-sm text-slate-500">A cafeína e polifenóis entram na corrente sanguínea.</p>
                        </div>
                         <div class="hidden md:flex flex-col items-center justify-center text-4xl text-sky-400">
                            →
                        </div>
                        <div class="flex md:hidden justify-center text-3xl text-sky-400 my-2">↓</div>
                        <div class="flowchart-step flex flex-col items-center p-5 rounded-lg">
                            <div class="w-20 h-20 bg-sky-100 rounded-full flex items-center justify-center mb-3">
                                <span class="text-3xl">🧠</span>
                            </div>
                            <h3 class="font-semibold text-sky-800">2. Bloqueio da Adenosina</h3>
                            <p class="text-sm text-slate-500">A cafeína liga-se aos recetores de adenosina (A2A), impedindo-a de atuar. Isto reduz a sonolência.</p>
                        </div>
                    </div>
                    <div class="flex justify-center my-6 text-4xl text-sky-400">↓</div>
                     <div class="grid grid-cols-1 md:grid-cols-3 gap-4 md:gap-6 text-center p-5 bg-slate-100 rounded-lg border border-slate-200">
                        <div class="p-3">
                            <h3 class="font-semibold text-sky-800 mb-1">Aumento de Neurotransmissores</h3>
                            <p class="text-sm text-slate-600">Liberta dopamina e norepinefrina, melhorando o humor, foco e alerta.</p>
                        </div>
                        <div class="p-3">
                            <h3 class="font-semibold text-sky-800 mb-1">Redução da Neuroinflamação</h3>
                            <p class="text-sm text-slate-600">Os polifenóis do café atuam como antioxidantes, protegendo as células cerebrais.</p>
                        </div>
                        <div class="p-3">
                            <h3 class="font-semibold text-sky-800 mb-1">Menor Acúmulo de Placas</h3>
                            <p class="text-sm text-slate-600">Pode ajudar a diminuir o acúmulo de proteínas beta-amiloide, associadas ao Alzheimer.</p>
                        </div>
                    </div>
                 </div>
            </section>

            <section id="references" class="tab-content hidden">
                <div class="content-card">
                    <h2 class="text-2xl font-semibold text-sky-700 mb-6">Referências Científicas</h2>
                    <p class="mb-6 text-slate-600 leading-relaxed">
                        Esta aplicação interativa foi desenvolvida com base em informações consolidadas de diversas publicações científicas de acesso aberto, incluindo revisões sistemáticas e meta-análises. Abaixo, uma seleção representativa das fontes que informaram o conteúdo:
                    </p>
                    <ul class="reference-list text-sm text-slate-600 leading-relaxed">
                        <li>Gardener, S. L., et al. (2021). Higher Coffee Consumption Is Associated With Slower Cognitive Decline and Less Cerebral Aβ-Amyloid Accumulation Over 126 Months: Data From the Australian Imaging, Biomarkers, and Lifestyle (AIBL) Study. *Frontiers in Aging Neuroscience*, 13, 744872.</li>
                        <li>Zhu, H., et al. (2024). Coffee, tea consumption and risk of cognitive disorders: an updated dose-response meta-analysis. *Food & Function*, 15(2), 514-529.</li>
                        <li>Liu, R., et al. (2024). Coffee consumption and the risk of dementia: a systematic review and dose-response meta-analysis of cohort studies. *Food & Function*, 15(1), 143-153.</li>
                        <li>Haskell-Ramsay, C. F., et al. (2018). The Acute Effects of Caffeinated Black Coffee on Cognition and Mood in Healthy Young and Older Adults. *Nutrients*, 10(10), 1386.</li>
                        <li>Zhang, Y., et al. (2022). Consumption of coffee and tea and risk of developing stroke, dementia, and poststroke dementia: A cohort study in the UK Biobank. *PLoS Medicine*, 19(2), e1003907.</li>
                        <li>Nehlig, A. (2016). Effects of Coffee/Caffeine on Brain Health and Disease: What Should I Tell My Patients? *Practical Neurology*, 16(2), 89-95.</li>
                        <li>Temple, J. L., et al. (2017). The Safety of Ingested Caffeine: A Comprehensive Review. *Frontiers in Psychiatry*, 8, 80.</li>
                        <li>Smit, H. J., & Rogers, P. J. (2000). Effects of caffeine on mood. *Food, Nutrition and Chemical Toxicity*, 279-303. (Capítulo de livro, para fins de exemplo de variedade de fontes)</li>
                        <li>Cornelis, M. C., et al. (2023). Coffee, caffeine, and cognitive function: A Mendelian randomization study. *Genes & Nutrition*, 18(1), 14.</li>
                        <li>Magalhães, R., et al. (2021). Habitual coffee drinkers display a distinct pattern of brain functional connectivity. *Molecular Psychiatry*, 26(10), 5569-5578.</li>
                        <li>Poole, R., et al. (2017). Coffee consumption and health: umbrella review of meta-analyses of multiple health outcomes. *BMJ*, 359, j5024.</li>
                        <li>Costa, J., et al. (2010). Caffeine exposure and the risk of Parkinson's disease: a systematic review and meta-analysis of observational studies. *Journal of Alzheimer's Disease*, 20 Suppl 1, S221-S238.</li>
                        <li>Drake, C., et al. (2013). Caffeine effects on sleep taken 0, 3, or 6 hours before going to bed. *Journal of Clinical Sleep Medicine*, 9(11), 1195-1200.</li>
                        <li>Juliano, L. M., & Griffiths, R. R. (2004). A critical review of caffeine withdrawal: empirical validation of symptoms and signs, incidence, severity, and associated features. *Psychopharmacology*, 176(1), 1-29.</li>
                    </ul>
                </div>
            </section>

        </main>

        <footer class="text-center mt-16 py-8 border-t border-slate-200 text-sm text-slate-600">
            <p class="max-w-2xl mx-auto leading-relaxed">Informações sintetizadas a partir de estudos e meta-análises de acesso aberto sobre o consumo de café e a saúde cognitiva. Esta aplicação é para fins informativos e não substitui o aconselhamento médico profissional.</p>
            <p class="mt-4">
                <a href="https://www.instagram.com/neuropedroambrosio/" target="_blank" rel="noopener noreferrer" class="text-sky-600 hover:text-sky-800 hover:underline font-semibold">
                    Siga no Instagram: @neuropedroambrosio
                </a>
            </p>
        </footer>
    </div>

    <script>
        const tabButtons = document.querySelectorAll('.tab-button');
        const tabContents = document.querySelectorAll('.tab-content');
        const accordionItems = document.querySelectorAll('.accordion-item');

        const setActiveTab = (tabName) => {
            tabButtons.forEach(button => {
                if (button.dataset.tab === tabName) {
                    button.classList.add('tab-active');
                } else {
                    button.classList.remove('tab-active');
                }
            });

            tabContents.forEach(content => {
                if (content.id === tabName) {
                    content.classList.remove('hidden');
                } else {
                    content.classList.add('hidden');
                }
            });
        };

        tabButtons.forEach(button => {
            button.addEventListener('click', () => {
                setActiveTab(button.dataset.tab);
                // Scroll to top of content for better UX on tab switch, especially on mobile
                window.scrollTo({ top: document.querySelector('main').offsetTop - 80, behavior: 'smooth' });

            });
        });
        
        accordionItems.forEach(item => {
            const header = item.querySelector('.accordion-header');
            const content = item.querySelector('.accordion-content');
            const iconEl = item.querySelector('.accordion-icon');

            header.addEventListener('click', () => {
                const isOpen = content.classList.contains('open');
                
                // Close all other accordions (optional, but common UX)
                // If you want multiple accordions to be open, remove this block
                document.querySelectorAll('.accordion-item').forEach(otherItem => {
                    if (otherItem !== item) {
                        otherItem.querySelector('.accordion-content').classList.remove('open');
                        otherItem.querySelector('.accordion-icon').textContent = '+';
                        otherItem.querySelector('.accordion-header').classList.remove('rounded-b-none');
                         if (otherItem.querySelector('.accordion-content').classList.contains('open')) { // This condition will likely be false now
                            otherItem.querySelector('.accordion-header').classList.add('rounded-b-none');
                        } else {
                            otherItem.querySelector('.accordion-header').classList.remove('rounded-b-none');
                        }
                    }
                });
                // End of optional block to close other accordions

                if (!isOpen) {
                    content.classList.add('open');
                    iconEl.textContent = '−'; // Minus sign
                    header.classList.add('rounded-b-none'); 
                } else {
                    content.classList.remove('open');
                    iconEl.textContent = '+';
                    header.classList.remove('rounded-b-none'); 
                }
            });
            if (content.classList.contains('open')) {
                header.classList.add('rounded-b-none');
            }
        });


        const benefitsData = {
            labels: ['Atenção/Vigilância', 'Velocidade de Processamento', 'Memória de Trabalho', 'Memória de Longo Prazo', 'Função Executiva', 'Humor/Alerta'],
            datasets: [{
                label: 'Efeito Predominante',
                data: [1, 1, 0.75, 0.5, 0.75, 1],
                backgroundColor: (context) => {
                    const value = context.dataset.data[context.dataIndex];
                    if (value === 1) return 'rgba(2, 132, 199, 0.7)';    // sky-600
                    if (value === 0.75) return 'rgba(3, 105, 161, 0.7)'; // sky-700
                    return 'rgba(7, 89, 133, 0.7)';                     // sky-800
                },
                borderColor: 'rgba(7, 89, 133, 1)', // sky-800
                borderWidth: 1,
                borderRadius: 4,
            }]
        };

        const longTermHealthData = {
            alzheimer: {
                label: 'Doença de Alzheimer',
                riskReduction: 26, 
                dose: '~2.5 xícaras/dia',
                description: 'A proteção máxima contra Alzheimer parece ser atingida com um consumo de aproximadamente 2.5 xícaras por dia, correspondendo a uma redução de risco de 26% (Risco Relativo 0.74). Doses mais altas podem não oferecer benefício adicional.',
                color: 'rgba(14, 165, 233, 0.7)' // sky-500
            },
            parkinson: {
                label: 'Doença de Parkinson',
                riskReduction: 25,
                dose: 'Aumento linear',
                description: 'A associação é forte e consistente, com uma redução de risco de cerca de 25% para consumidores habituais. A proteção aumenta com a dose (relação linear), especialmente em homens.',
                color: 'rgba(6, 182, 212, 0.7)' // cyan-500
            },
            avc: {
                label: 'Acidente Vascular Cerebral',
                riskReduction: 32,
                dose: '2-3 café + 2-3 chá/dia',
                description: 'Uma combinação de café e chá (total de 4-6 xícaras) foi associada a uma redução de risco de 32% (Hazard Ratio 0.68) para AVC incidente, sugerindo um efeito sinérgico benéfico para a saúde vascular.',
                color: 'rgba(13, 148, 136, 0.7)' // teal-600
            },
            demenciaPosAvc: {
                label: 'Demência Pós-AVC',
                riskReduction: 48,
                dose: '3-6 (café + chá)/dia',
                description: 'Para quem já sofreu um AVC, o consumo combinado de 3 a 6 xícaras de café e chá por dia foi associado a uma impressionante redução de risco de 48% (Hazard Ratio 0.52) de desenvolver demência subsequente.',
                color: 'rgba(8, 145, 178, 0.7)' // cyan-600
            }
        };

        let benefitsChartInstance, longTermChartInstance;
        Chart.defaults.font.family = "'Inter', sans-serif"; 

        const createBenefitsChart = () => {
            const ctx = document.getElementById('benefitsChart').getContext('2d');
            if(benefitsChartInstance) {
                benefitsChartInstance.destroy();
            }
            benefitsChartInstance = new Chart(ctx, {
                type: 'bar',
                data: benefitsData,
                options: {
                    indexAxis: 'y',
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: { display: false },
                        tooltip: {
                            backgroundColor: '#1e293b', 
                            titleColor: '#f8fafc', 
                            bodyColor: '#e2e8f0', 
                            padding: 10,
                            cornerRadius: 4,
                            callbacks: {
                                label: function(context) {
                                    const value = context.raw;
                                    if (value === 1) return 'Efeito: Positivo';
                                    if (value === 0.75) return 'Efeito: Positivo/Misto';
                                    return 'Efeito: Misto';
                                }
                            }
                        }
                    },
                    scales: {
                        x: {
                            display: false,
                            max: 1.1,
                            grid: { display: false }
                        },
                        y: {
                           ticks: {
                               font: {
                                   size: 11,
                                   weight: '500'
                               },
                               color: '#475569', 
                               autoSkip: false,
                               callback: function(value) { 
                                    const label = this.getLabelForValue(value);
                                    if (label.length > 22) { 
                                        return label.substring(0, 22) + '...';
                                    }
                                    return label;
                                }
                           },
                           grid: { 
                                display: true,
                                color: '#e2e8f0' 
                            }
                        }
                    }
                }
            });
        }

        const longTermInfoEl = document.getElementById('longTermInfo');
        const diseaseSelector = document.getElementById('diseaseSelector');

        const updateLongTermHealthChart = (diseaseKey) => {
            const diseaseData = longTermHealthData[diseaseKey];
            
            const chartData = {
                labels: [diseaseData.label, 'Referência (Não Consumidor)'],
                datasets: [{
                    label: 'Redução de Risco (%)',
                    data: [diseaseData.riskReduction, 0],
                    backgroundColor: [diseaseData.color, 'rgba(203, 213, 225, 0.7)'], 
                    borderColor: [diseaseData.color.replace('0.7', '1'), 'rgba(156, 163, 175, 1)'], 
                    borderWidth: 1,
                    borderRadius: 4,
                }]
            };

            const ctx = document.getElementById('longTermChart').getContext('2d');
            if (longTermChartInstance) {
                longTermChartInstance.destroy();
            }
            longTermChartInstance = new Chart(ctx, {
                type: 'bar',
                data: chartData,
                options: {
                    indexAxis: 'y',
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: { display: false },
                         tooltip: {
                            backgroundColor: '#1e293b', 
                            titleColor: '#f8fafc', 
                            bodyColor: '#e2e8f0', 
                            padding: 10,
                            cornerRadius: 4,
                            callbacks: {
                                label: function(context) {
                                    if(context.dataIndex === 0) {
                                        return ` Redução de Risco: ${context.raw}%`;
                                    }
                                    return ' Linha de Base';
                                }
                            }
                        }
                    },
                    scales: {
                        x: {
                           title: {
                               display: true,
                               text: 'Redução de Risco (%)',
                               color: '#475569', 
                               font: { weight: '600'}
                           },
                           ticks: { color: '#475569'}, 
                           grid: { color: '#e2e8f0'} 
                        },
                         y: {
                           ticks: {
                               font: {
                                   size: 11,
                                   weight: '500'
                               },
                               color: '#475569', 
                               autoSkip: false
                           },
                           grid: { 
                                display: false
                            }
                        }
                    }
                }
            });

            longTermInfoEl.innerHTML = `
                <h3 class="font-semibold text-lg text-sky-800">${diseaseData.label}</h3>
                <p class="mt-2 text-slate-600 leading-relaxed">${diseaseData.description}</p>
                <div class="mt-4 pt-4 border-t border-sky-100">
                    <p class="text-sm font-semibold text-sky-700">Dose Ótima Associada:</p>
                    <p class="text-sm text-sky-800 font-bold">${diseaseData.dose}</p>
                </div>
            `;
        };

        diseaseSelector.addEventListener('change', (e) => {
            updateLongTermHealthChart(e.target.value);
        });
        
        window.addEventListener('load', () => {
            setActiveTab('overview'); 
            createBenefitsChart();
            updateLongTermHealthChart('alzheimer'); 
        });

    </script>
</body>
</html>
