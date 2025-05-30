# Análise de Tópicos com LDA

Este projeto tem como objetivo aplicar técnicas de Processamento de Linguagem Natural (PLN) para realizar **análise de tópicos** em um conjunto de dados textuais. Utiliza-se o modelo **Latent Dirichlet Allocation (LDA)** para identificar automaticamente os principais temas abordados nos textos analisados.

## Objetivos

- Realizar pré-processamento textual em um corpus de documentos.
- Identificar e extrair tópicos latentes utilizando LDA.
- Visualizar os tópicos de forma clara e interpretável.
- Oferecer uma base para tomada de decisões a partir da análise temática dos dados.

## Tecnologias Utilizadas

- **Python 3.10+**
- **Jupyter Notebook**
- **NLTK** – Tokenização, stopwords, stemming
- **spaCy** – Tokenização e lematização
- **gensim** – Treinamento do modelo LDA
- **pyLDAvis** – Visualização interativa dos tópicos
- **pandas / matplotlib** – Análise e visualização auxiliar de dados


## Etapas do Processo

1. **Carregamento dos Dados**
   - Os dados textuais são importados de fontes como arquivos CSV ou bancos de dados.

2. **Pré-processamento**
   - Limpeza textual (remoção de pontuação, símbolos e números).
   - Tokenização.
   - Remoção de stopwords.
   - Lematização ou stemming.

3. **Criação do Dicionário e Corpus**
   - Conversão dos documentos para o formato exigido pelo modelo LDA (bag-of-words).

4. **Treinamento do Modelo LDA**
   - Definição da quantidade de tópicos.
   - Treinamento do modelo usando `gensim.models.LdaModel`.

5. **Visualização dos Tópicos**
   - Uso do `pyLDAvis` para exibir tópicos em uma visualização interativa que mostra a distribuição e o conteúdo de cada tópico.

6. **Análise dos Resultados**
   - Interpretação qualitativa dos tópicos.
   - Identificação de palavras-chave por tópico.
   - Atribuição de tópicos predominantes por documento.

## Resultados Esperados
Gráficos de distribuição de tópicos.
Palavras-chave associadas a cada tópico.
Atribuição de tópicos aos textos de entrada. 

## Considerações Finais
Este projeto serve como base para aplicações mais amplas de análise temática, como mineração de opiniões, segmentação de conteúdo, e apoio à curadoria de textos. A estrutura modular permite fácil adaptação a novos datasets e ajustes nos parâmetros do modelo.