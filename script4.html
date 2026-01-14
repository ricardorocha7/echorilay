// =============== TOGGLE SIDEBAR ===============
document.getElementById('open_btn').addEventListener('click', function () {
    const sidebar = document.getElementById('sidebar');
    sidebar.classList.toggle('open-sidebar');
});

// =============== GRÁFICO DE SATISFAÇÃO ===============
let tipoAtual = 'bar';
let chart = null;
const canvas = document.getElementById('meuGrafico');

// Só inicializa se o canvas existir (evita erro se não tiver gráfico)
if (canvas) {
    const ctx = canvas.getContext('2d');

    const labels = ["Elogios", "Decepções", "Melhorias"];
    const barValues = [76, 34, 23];
    const colors = ["#8e9287ff", "#555555ff", "#020213ff"];

    function createChart() {
        if (chart) {
            chart.destroy();
        }

        chart = new Chart(ctx, {
            type: tipoAtual,
            data: {
                labels: labels,
                datasets: [{
                    data: barValues,
                    backgroundColor: colors,
                    borderWidth: 1,
                    borderRadius: tipoAtual === 'bar' ? 6 : 0
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'top',
                        labels: {
                            usePointStyle: true,
                            pointStyle: 'circle',
                            generateLabels(chart) {
                                const data = chart.data;
                                return data.labels.map((label, i) => ({
                                    text: label,
                                    fillStyle: data.datasets[0].backgroundColor[i],
                                    strokeStyle: data.datasets[0].backgroundColor[i],
                                    lineWidth: 0,
                                    hidden: !chart.getDataVisibility(i),
                                    index: i
                                }));
                            }
                        }
                    }
                },
                scales: tipoAtual === 'bar' ? {
                    y: { beginAtZero: true }
                } : {}
            }
        });
    }

    // Inicializa o gráfico ao carregar
    window.onload = function () {
        createChart();

        const botao = document.getElementById('toggleGraph');
        if (botao) {
            botao.addEventListener('click', () => {
                tipoAtual = tipoAtual === 'bar' ? 'pie' : 'bar';
                createChart();
                botao.textContent = tipoAtual === 'bar' ? '⇆ Alterar gráfico' : '⇆ Alterar gráfico';
            });
        }
    };
}
