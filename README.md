# Trabalho de Estrutura de Dados

Este trabalho tem como objetivo implementar e analisar dois algoritmos de ordenação: HeapSort e ShellSort. Os algoritmos foram desenvolvidos na linguagem C conforme solicitado na atividade.

O HeapSort é um algoritmo de ordenação baseado em uma estrutura chamada Heap, representada por uma árvore binária completa. Sua complexidade é O(n log n) em todos os casos, o que torna seu desempenho previsível. O funcionamento do algoritmo ocorre em duas etapas principais: a construção do Max-Heap e a remoção sucessiva do maior elemento da estrutura, seguida da reorganização do heap através da função heapify.

O ShellSort é uma melhoria do algoritmo Insertion Sort. Ele utiliza uma sequência de intervalos chamados gaps para comparar e ordenar elementos que estão distantes entre si. Conforme o algoritmo avança, o valor do gap diminui até chegar a 1, momento em que ocorre uma ordenação semelhante ao Insertion Sort. A complexidade do ShellSort depende da sequência de gaps utilizada, podendo variar aproximadamente entre O(n log n) e O(n²).

No programa foi utilizado o vetor [30, 12, 45, 6, 18, 3] para demonstrar o funcionamento dos algoritmos. Na construção do Max-Heap, o maior elemento passa a ocupar a raiz da estrutura, resultando na representação em vetor [45, 18, 30, 6, 12, 3].

A estrutura do repositório contém os seguintes arquivos: o arquivo "ordenacao.c", que possui a implementação dos algoritmos HeapSort e ShellSort, e o arquivo README.md com a descrição do trabalho.

Para compilar o programa pode-se utilizar o compilador GCC com o comando:

gcc ordenacao.c -o ordenação

Após a compilação, o programa pode ser executado com o comando:

./ordenacao

A execução do programa mostra o vetor original e os vetores ordenados utilizando HeapSort e ShellSort.

Como conclusão, observa-se que o HeapSort possui complexidade garantida de O(n log n), sendo indicado para aplicações que necessitam de previsibilidade no tempo de execução. O ShellSort apresenta bom desempenho na prática, porém sua complexidade depende da sequência de gaps utilizada.
