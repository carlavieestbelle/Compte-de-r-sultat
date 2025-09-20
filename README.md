<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Le Compte de Résultat de A à Z</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8;
        }
        .chart-container {
            position: relative;
            width: 100%;
            height: 350px;
        }
        .formula-box {
            background-color: #eef2ff;
            border-left: 4px solid #3b82f6;
            color: #1e3a8a;
        }
        .card {
            background-color: white;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -2px rgb(0 0 0 / 0.1);
        }
        .puzzle-piece {
            border-radius: 0.5rem;
            padding: 0.75rem 1rem;
            font-weight: 600;
            border-width: 1px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .kpi-card {
            padding: 1.5rem;
            border-radius: 0.75rem;
            text-align: center;
            flex-grow: 1;
        }
        .kpi-title {
            font-weight: 600;
            font-size: 1.1rem;
        }
        .kpi-value {
            font-weight: 700;
            font-size: 2.25rem;
            letter-spacing: -0.05em;
        }
        .definition-item strong {
            color: #1e3a8a;
        }
    </style>
</head>
<body class="text-gray-800">

    <div class="container mx-auto p-4 md:p-8">
        <header class="text-center mb-10">
            <h1 class="text-4xl md:text-5xl font-bold text-blue-900 mb-2">Le Compte de Résultat Simplifié</h1>
            <p class="text-lg text-gray-600">Le film de la performance financière de votre entreprise sur une année.</p>
        </header>

        <main class="space-y-12">
            <section class="card p-6 text-center">
                <h2 class="text-2xl font-bold text-blue-800 mb-4">Qu'est-ce que le Compte de Résultat ?</h2>
                <p class="max-w-3xl mx-auto">
                    Imaginez le compte de résultat comme un résumé de tout l'argent qu'une entreprise a gagné (les <strong class="text-blue-600">produits</strong>) et dépensé (les <strong class="text-red-600">charges</strong>) sur une période donnée. Son objectif est simple : savoir si l'entreprise a réalisé un <strong class="text-green-600">bénéfice</strong> ou une <strong class="text-red-600">perte</strong>.
                </p>
                <div class="formula-box p-4 mt-6 inline-block">
                    <p class="text-xl font-semibold">Résultat Net = Total des Produits - Total des Charges</p>
                </div>
            </section>

            <section class="card p-6">
                <h2 class="text-2xl font-bold text-blue-800 mb-4 text-center">Les Termes Clés à Connaître</h2>
                <div class="grid grid-cols-1 md:grid-cols-2 gap-x-8 gap-y-6 mt-6 text-left">
                    <div class="definition-item">
                        <strong>Produits :</strong>
                        <p class="text-gray-600">Toutes les sources de revenus pour l'entreprise. C'est l'argent qui rentre.</p>
                    </div>
                    <div class="definition-item">
                        <strong>Charges :</strong>
                        <p class="text-gray-600">Toutes les dépenses nécessaires pour faire fonctionner l'entreprise. C'est l'argent qui sort.</p>
                    </div>
                    <div class="definition-item">
                        <strong>Chiffre d'Affaires (CA) :</strong>
                        <p class="text-gray-600">Le montant total des ventes de biens ou services. C'est le produit principal issu de l'activité de base (l'exploitation).</p>
                    </div>
                     <div class="definition-item">
                        <strong>Résultat d'Exploitation :</strong>
                        <p class="text-gray-600">Le bénéfice généré uniquement par l'activité principale de l'entreprise, avant les aspects financiers et les impôts.</p>
                    </div>
                     <div class="definition-item">
                        <strong>Produits Financiers :</strong>
                        <p class="text-gray-600">Les revenus tirés des placements de trésorerie (intérêts, dividendes...). C'est l'argent que l'argent de l'entreprise rapporte.</p>
                    </div>
                     <div class="definition-item">
                        <strong>Charges Financières :</strong>
                        <p class="text-gray-600">Les coûts liés aux dettes de l'entreprise, principalement les intérêts payés sur les emprunts.</p>
                    </div>
                     <div class="definition-item">
                        <strong>Résultat Net (Bénéfice / Perte) :</strong>
                        <p class="text-gray-600">Le chiffre final, après avoir tout compté. C'est ce qu'il reste vraiment à l'entreprise à la fin de l'année.</p>
                    </div>
                </div>
            </section>
            
            <section class="card p-6">
                <h2 class="text-2xl font-bold text-blue-800 mb-6 text-center">La Composition du Résultat de "MaBoutique SARL"</h2>
                <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">Visualisons les deux familles qui composent le résultat de notre exemple : les Produits (les gains) et les Charges (les dépenses).</p>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
                    <div>
                        <h3 class="text-xl font-bold text-blue-800 mb-4 text-center">D'où vient l'argent ? (Les Produits)</h3>
                        <div class="flex flex-col sm:flex-row gap-4">
                            <div class="kpi-card bg-green-100 border border-green-200">
                                <p class="kpi-title text-green-800">Ventes (Chiffre d'Affaires)</p>
                                <p class="kpi-value text-green-900">100 000 €</p>
                                <p class="text-green-700 text-sm">Activité principale</p>
                            </div>
                             <div class="kpi-card bg-emerald-100 border border-emerald-200">
                                <p class="kpi-title text-emerald-800">Produits financiers</p>
                                <p class="kpi-value text-emerald-900">500 €</p>
                                <p class="text-emerald-700 text-sm">Placements</p>
                            </div>
                        </div>
                    </div>
                    <div>
                         <h3 class="text-xl font-bold text-blue-800 mb-4 text-center">Où va l'argent ? (Les Charges)</h3>
                         <div class="chart-container">
                            <canvas id="chargesChart"></canvas>
                        </div>
                    </div>
                </div>
            </section>

            <section class="card p-6">
                <h2 class="text-2xl font-bold text-blue-800 mb-6 text-center">Exemple Pratique : Assemblons le Puzzle</h2>
                
                <div class="text-center mb-8">
                    <h3 class="text-xl font-bold text-blue-700 mb-2">Étape 1 : Identifier les pièces du puzzle</h3>
                    <p class="text-gray-600 max-w-2xl mx-auto">Voici toutes les informations financières de l'année. Chaque élément est une "pièce" que nous allons devoir classer.</p>
                </div>
                
                <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4 max-w-4xl mx-auto mb-10">
                    <div class="puzzle-piece bg-green-100 text-green-800 border-green-300"><span>Ventes de marchandises</span> <span>+ 100 000 €</span></div>
                    <div class="puzzle-piece bg-emerald-100 text-emerald-800 border-emerald-300"><span>Produits financiers</span> <span>+ 500 €</span></div>
                    <div class="puzzle-piece bg-red-100 text-red-800 border-red-300"><span>Achats de marchandises</span> <span>- 40 000 €</span></div>
                    <div class="puzzle-piece bg-orange-100 text-orange-800 border-orange-300"><span>Salaires et charges</span> <span>- 25 000 €</span></div>
                    <div class="puzzle-piece bg-amber-100 text-amber-800 border-amber-300"><span>Loyer et autres</span> <span>- 10 000 €</span></div>
                    <div class="puzzle-piece bg-rose-100 text-rose-800 border-rose-300"><span>Charges financières</span> <span>- 1 500 €</span></div>
                    <div class="puzzle-piece bg-violet-100 text-violet-800 border-violet-300"><span>Impôts sur les sociétés</span> <span>- 6 000 €</span></div>
                </div>

                <div class="text-center mb-8">
                     <h3 class="text-xl font-bold text-blue-700 mb-2">Étape 2 : Assembler le Compte de Résultat</h3>
                    <p class="text-gray-600 max-w-2xl mx-auto">Maintenant, plaçons chaque pièce dans la bonne catégorie. Suivez les couleurs !</p>
                </div>

                <div class="overflow-x-auto max-w-4xl mx-auto">
                    <table class="w-full min-w-max text-left">
                        <thead>
                            <tr class="border-b-2 border-blue-200 bg-blue-50">
                                <th class="p-3 font-semibold text-blue-800">Libellé</th>
                                <th class="p-3 font-semibold text-blue-800 text-right">Montant (€)</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="font-semibold bg-gray-100"><td class="p-3 text-gray-700" colspan="2">PRODUITS (Ce qu'on a gagné)</td></tr>
                            <tr class="bg-green-100">
                                <td class="p-3 pl-6 text-green-800 font-semibold">Ventes de marchandises</td>
                                <td class="p-3 text-right text-green-800 font-semibold">100 000</td>
                            </tr>
                            <tr class="bg-emerald-100">
                                <td class="p-3 pl-6 text-emerald-800 font-semibold">Produits financiers</td>
                                <td class="p-3 text-right text-emerald-800 font-semibold">500</td>
                            </tr>
                             <tr class="border-y-2 border-blue-200">
                                <td class="p-3 pl-6 font-bold text-blue-800">Total des Produits</td>
                                <td class="p-3 text-right font-bold text-blue-800">100 500</td>
                            </tr>

                            <tr class="font-semibold bg-gray-100"><td class="p-3 text-gray-700" colspan="2">CHARGES (Ce qu'on a dépensé)</td></tr>
                            <tr class="bg-red-100">
                                <td class="p-3 pl-6 text-red-800 font-semibold">Achats de marchandises</td>
                                <td class="p-3 text-right text-red-800 font-semibold">- 40 000</td>
                            </tr>
                             <tr class="bg-orange-100">
                                <td class="p-3 pl-6 text-orange-800 font-semibold">Salaires et charges sociales</td>
                                <td class="p-3 text-right text-orange-800 font-semibold">- 25 000</td>
                            </tr>
                             <tr class="bg-amber-100">
                                <td class="p-3 pl-6 text-amber-800 font-semibold">Loyer et autres charges externes</td>
                                <td class="p-3 text-right text-amber-800 font-semibold">- 10 000</td>
                            </tr>
                            <tr class="bg-rose-100">
                                <td class="p-3 pl-6 text-rose-800 font-semibold">Charges financières</td>
                                <td class="p-3 text-right text-rose-800 font-semibold">- 1 500</td>
                            </tr>
                            <tr class="bg-violet-100">
                                <td class="p-3 pl-6 text-violet-800 font-semibold">Impôts sur les sociétés</td>
                                <td class="p-3 text-right text-violet-800 font-semibold">- 6 000</td>
                            </tr>
                            <tr class="border-y-2 border-red-200">
                                <td class="p-3 pl-6 font-bold text-red-800">Total des Charges</td>
                                <td class="p-3 text-right font-bold text-red-800">- 82 500</td>
                            </tr>
                        </tbody>
                    </table>
                </div>

                <div class="text-center mt-10">
                     <h3 class="text-xl font-bold text-blue-700 mb-2">Étape 3 : Calculer le Résultat Final</h3>
                    <p class="text-gray-600 max-w-2xl mx-auto mb-4">Il ne reste plus qu'à appliquer notre formule magique !</p>
                    <div class="max-w-xl mx-auto p-6 bg-green-100 rounded-lg shadow-lg border border-green-200">
                        <p class="text-lg text-gray-700">Total Produits - Total Charges = Résultat Net</p>
                        <p class="text-2xl font-bold text-green-800 my-2">
                            <span class="text-blue-800">100 500 €</span> - <span class="text-red-800">82 500 €</span> = <span class="text-green-900">18 000 €</span>
                        </p>
                        <p class="text-xl font-bold text-green-900">🎉 MaBoutique SARL a réalisé un BÉNÉFICE de 18 000 € ! 🎉</p>
                    </div>
                </div>
            </section>
        </main>
    </div>

<script>
    const FONT_COLOR = '#1e3a8a';
    const GRID_COLOR = '#e0e7ff';

    const processLabels = (labels) => {
        return labels.map(label => {
            if (label.length > 20) {
                const words = label.split(' ');
                const lines = [];
                let currentLine = '';
                words.forEach(word => {
                    if ((currentLine + ' ' + word).length > 20) {
                        lines.push(currentLine.trim());
                        currentLine = word;
                    } else {
                        currentLine += ' ' + word;
                    }
                });
                lines.push(currentLine.trim());
                return lines;
            }
            return label;
        });
    };
    
    const ctxCharges = document.getElementById('chargesChart').getContext('2d');
    new Chart(ctxCharges, {
        type: 'bar',
        data: {
            labels: processLabels([
                'Achats de marchandises', 
                'Salaires et charges', 
                'Loyer et autres', 
                'Impôts sur les sociétés', 
                'Charges financières'
            ]),
            datasets: [{
                label: 'Répartition des Charges en €',
                data: [40000, 25000, 10000, 6000, 1500],
                backgroundColor: [
                    '#f87171', // red-400
                    '#fb923c', // orange-400
                    '#fbbf24', // amber-400
                    '#a78bfa', // violet-400
                    '#f472b6'  // rose-400
                ],
                borderColor: [
                    '#b91c1c',
                    '#c2410c',
                    '#b45309',
                    '#6d28d9',
                    '#be185d'
                ],
                borderWidth: 1,
                borderRadius: 4
            }]
        },
        options: {
            indexAxis: 'y',
            responsive: true,
            maintainAspectRatio: false,
            plugins: {
                legend: {
                    display: false
                },
                tooltip: {
                    callbacks: {
                        title: function(tooltipItems) {
                            const item = tooltipItems[0];
                            let label = item.chart.data.labels[item.dataIndex];
                            if (Array.isArray(label)) {
                              return label.join(' ');
                            }
                            return label;
                        }
                    }
                }
            },
            scales: {
                y: {
                    ticks: { color: FONT_COLOR, font: { size: 12 } },
                    grid: { display: false }
                },
                x: {
                    ticks: { color: FONT_COLOR },
                    grid: { color: GRID_COLOR }
                }
            }
        }
    });
</script>

</body>
</html>
