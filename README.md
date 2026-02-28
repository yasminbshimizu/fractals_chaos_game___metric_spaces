# <p align="center"> ❄️ Jogo do Caos: Estudo de métricas para geração de fractais ❄️ </p>
<p align="center"> Projeto desenvolvido durante a disciplina de Espaços Normados, sob orientação do Prof. Dr. Vinícius F. Wasques, explorando métricas euclidiana, da soma e do máximo para formação de estruturas fractais. </p>

<p align="center">
<img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge"/>
</p>

<div align="center">
  <img src="https://github.com/user-attachments/assets/ccb6f5f1-0e07-4eb2-aa7c-5f681c57a59c" alt="Descrição da imagem" width="1000"/>
</div>

## 📝 Fractais e o Jogo do Caos

 **Fractais** são estruturas geométricas com padrões repetitivos e alta simetria, seja por translação, rotação, reflexão ou inversão [1]. São estudados desde a antiguidade e tem sido aprofundados recentemente, em aplicações como química do estado sólido e genética molecular [1,2,3]. 
    Um dos fractais mais populares é o **triângulo de Sierpinski**, gerado de forma iterativa de modo que a área preenchida do triângulo base tenda a zero e a área vazia tenda a sua área total [2,3]. Outra forma de gerar o triângulo de Sierpinski é através do “**Jogo do Caos**”, um algoritmo iterativo baseado na distância entre pontos, consistindo nas seguintes etapas:

1. Delimitação de uma região triângular;
2. Sorteio de um ponto aletório na região;
3. Cálculo da distância entre o ponto definido anteriormente e um vértice aleatório da região triangular;
4. Determinação do ponto médio (metade da distância) entre os pontos sorteados;
5. Retorno ao passo 3.

O fractal é nítido após milhares de iterações. Também é possível mudar parâmetros do algoritmo, como a forma geométrica base, a **fração da distância**, a forma geométrica base, ou o **espaço métrico** [3]. 


## 🎯 Objetivos
Este trabalho tem como objetivo **explorar conceitos de espaços métricos para a geração de fractais** com **ferramentas computacionais**. Assim, os pontos de interesse são: 

*  Simular o Jogo do Caos clássico;
*   Alterar a proporção da distância caminhada, utilizando razões menor e maior que $\frac{1}{2}$ entre 0 e 1, e maior que 1;
*   Variar as métricas utilizadas, com a euclidiana, da soma e do máximo;
*   Visualizar a evolução temporal da geração de fractais;
*   Comparar os diferentes padrões formados.

## ❄️ Resultados

Aplicando, incialmente, o caso clássico com metade da distância, observa-se o surgimento do padrão esperado para o triângulo de Sierpinski. Com a alteração das razões da distância no intervalo $(0,1)$, os padrões observados são semelhantes, mudando o tamanho dos triângulos internos formados e alterando a área preenchida da figura. Para razões maiores que um, os pontos extrapolam o triângulo, mas ainda seguem uma geometria fractal simétrica em relação à região triangular, se expandindo em todas as direções ao se distanciar do centro --- aqui, é importante ressaltar que o padrão fractal emergente varia a cada geração devido à aleatoriedade do processo. Alterando as métricas utilizadas na construção do fractal, o padrão observado também difere bastante do fractal original, de modo que as regiões mais e menos preenchidas estão associadas aos conjuntos de pontos médios em cada caso. 

## 🗂️ Arquivos

* <code> chaos_game_euclidian.ipynb </code>: geração de fractais utilizando a métrica euclidiana, variando frações da distância caminhada.
* <code> chaos_game_max.ipynb </code>: geração de fractais utilizando a métrica do máximo.
* <code> chaos_game_sum.ipynb </code>: geração de fractais utilizando a métrica da soma.
* <code> mean_points_geometry.ipynb </code>: métricas, esferas, pontos médios e suas representações geométricas.

## 📚 Referências
[1] MEAKIN, P. Fractal structures. Progress in Solid State Chemistry, v. 20, n. 3, p. 135–233, jan. 1990. DOI: 10.1016/0079-6786(90)90001-v.

[2]MARTÍNEZ-CRUZ, Miguel-Ángel; PATIÑO-ORTIZ, Julián; PATIÑO-ORTIZ, Miguel; BALANKIN, Alexander S. Some insights into the Sierpiński triangle paradox. Fractal and Fractional, v. 8, n. 11, p. 655, nov. 2024. DOI: 10.3390/fractalfract8110655.

[3] DEVANEY, R. L. Fractal Patterns and Chaos Games. The Mathematics Teacher, v. 98, n. 4, p. 228–233, nov. 2004.

[4] LIMA, E. L. _Espaços métricos_. Projeto Euclides. Instituto de Matemática Pura e Aplicada, CNPq, 1977.
LCCN: 78382414.

[5] BOGDEWICZ, A.; GRZYBOWSKI, J. Unique metric segments in the hyperspace over a strictly convex Minkowski space. Beiträge zur Algebra und Geometrie / Contributions to Algebra and Geometry, v. 54, n. 1, p. 453–467, jul. 2012. DOI: 10.1007/s13366-012-0108-4.
