# Random-Walks-1D-2D
Task of Física Estatística Computacional

Task description:

Podemos gerar e analisar eficientemente caminhadas aleatórias no computador.

(a) Escreva uma rotina para gerar caminhadas aleatórias de N passos em d  (=1 ou 2) dimensões, com cada passo uniformemente distribuído no intervalo (-1/2, 1/2) em cada dimensão. (Primeiro, gere os passos como um array N x d e, então, faça uma soma cumulativa.) Faça um gráfico de x_t por t para poucas caminhadas de 10.000 passos. Faça um gráfico de x por y para poucas caminhadas aleatórias bidimensionais com N = 10, 1.000, e 100.000 (tente manter a razão de aspecto do gráfico XY em um.) Se você multiplicar o número de passo por 100, a distância final da caminhada aumenta por cerca de 10 vezes?

Cada caminhada aleatória é diferente e imprevisível, mas o ensemble de caminhadas aleatórias tem propriedades elegantes e previsíveis. 

P.s.: Um ensemble é uma construção usada com frequência na física estatística e se refere a um conjunto muito grande de sistemas preparados exatamente da mesma forma e, portanto, sujeitos exatamente às mesmas condições. Ao analisar esse ensemble, conseguimos extrair propriedades gerais (estatísticas) a cerca do fenômeno que pretendemos estudar. Neste caso, um conjunto grande de caminhadas aleatórias geradas com sequências diferentes de números aleatórios pode ser entendida como um ensemble. 

(b) Escreva uma rotina para determinar os pontos finais de W caminhadas aleatórias com N passos cada em d=2 dimensões. Faça um gráfico de dispersão das coordenadas finais de 10.000 caminhadas aleatórias com N=1 e 10, superpostos no mesmo gráfico.  Perceba que as caminhadas longas estão distribuídas em um padrão simétrico e circular, enquanto as caminhadas de um único passo tem uma distribuição de probabilidades quadrada. 

Essa é uma simetria emergente! Apesar do caminhante dar passos maiores nas diagonais de um quadrado, um caminhante que dá vários passos tem uma simetria rotacional quase perfeita. 

A propriedade mais útil de uma caminhada aleatória é o teorema central do limite. Os pontos finais de um ensemble de caminhadas aleatórias de N passos em uma dimensão com passos com desvio quadrático médio (RMS) de tamanho a tem uma distribuição de probabilidades Gaussiana (ou Normal) quando N\to \infty,

 \rho(x)=\frac{1}{\sqrt{2\pi} \sigma}\text{exp}\left(-x^2/2\sigma^2\right), 
com \sigma=\sqrt{N}a.

(c) Calcule o desvio quadrático médio (RMS), a para passos uniformemente distribuidos no intervalo (-1/2, 1/2) em uma dimensão. Escreva uma rotina que plota um histograma dos pontos finais de W caminhadas aleatórias com N passos e 50 caixas (bins), junto com a previsão da equação acima para x no intervalo (-3\sigma, 3\sigma). Faça um histograma com W=10.000 e N=1, 2, 3 e 5. Quão rápido a distribuição Gaussiana se torna uma boa aproximação para uma caminhada aleatória?
