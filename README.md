# Repositório de dados para desenvolvimento de sistema de Avaliação Automática de Respostas Abertas

### Introdução
Este repositório é destinado ao armazenamento e compartilhamento da base de dados utilizada para o desenvolvimento de um sistema de Avaliação Automática de Respostas Abertas. A base de dados é composta por dois tipos de dados, originados de atividades e avaliações realizados por alunos da disciplina de Metodologia de Pesquisa em Psicologia 3, da PUC-GO, ministrada pelo professor Weber Martins. O primeiro tipo de dados consistem em resumos de esquemas sobre quatro temas relacionados à disciplina e foi utilizada para a implementação de *word embeddings*, usando o *word2vec*, essa coleção será denominada
*dataset Resumos*. O segundo tipo consiste em 242 respostas curtas de uma questão dissertativa
que é recorrentemente aplicada e arquivada desde o primeiro semestre de 2016, com a nota
final associada essa base de dados será referida como dataset Cientificidade, devido ao enunciado da
questão: **“Justifique a cientificidade da Psicologia.”**.

### Detalhes das bases de dados
O primeiro tipo de dados está contido no arquivo `resumos.txt`, que é um simples arquivo de texto que contém um resumo por linha.

O segundo tipo de dados está contido nos arquivos `preprocessado.csv` e `preprocessado_sem_stopwords.csv`, sendo que no primeiro arquivo estão contidas as questões na íntegra e no segundo arquivo estão as questões após a remoção das *stopwords* contidas no arquivo `stopwords.txt`. Ambos os arquivos estão no formato csv. Sendo que a primeira linha é um cabeçalho e em cada linha seguinte temos a resposta seguida da nota atribuída pelo avaliador. A nota está em uma escala de 0 à 10. Os dois arquivos foram pré processados utilizando o script contido no arquivo `preprocess.ipynb` e a lista de *stopwords*.
