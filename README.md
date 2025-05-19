# Trabalho-de-Grafo.-

Simulador de Incêndios Florestais
Este projeto simula a propagação de fogo em uma floresta representada por um grafo, e a atuação de caminhões de bombeiro para conter os incêndios. O cenário é configurado por dois arquivos de entrada: vertices.txt e arestas.txt.

Estrutura dos Arquivos
vertices.txt
Cada linha representa uma árvore ou ponto da floresta, no seguinte formato:

<Nome> <PotênciaDeQueima> <Tipo>
Nome: Identificador do vértice (por exemplo: A, B, C...).

PotênciaDeQueima: Tempo total que o vértice queima antes de ser completamente destruído, caso não seja apagado.

Tipo:

0 → Posto de Brigadista

1 → Fonte de água 

2 → Árvore 

Exemplo:

A 5 2
B 5 2
C 5 2
D 0 1
E 0 1
F 0 0
G 4 2
H 3 2
I 0 1

arestas.txt
Cada linha define uma conexão entre dois vértices com um determinado custo (tempo de deslocamento):


<Origem> <Destino> <Peso>
Origem e Destino: nomes dos vértices conectados.

Peso: tempo necessário para atravessar essa conexão.

Exemplo:


A B 4
B C 5
B D 3
C E 6
D F 3
F G 7
G H 5
H I 4
Obs: O grafo é não-direcionado – os caminhos funcionam em ambos os sentidos.
