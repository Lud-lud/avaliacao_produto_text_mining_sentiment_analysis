# Análise de sentimentos de comentários avaliativos sobre um produto vendido em um e-commerce

### Análise descritiva
Neste projeto, foi realizada uma análise de sentimentos utilizando comentários de avaliação publicados sobre anúncios do Mercado Livre que vendiam a mochila representada abaixo:

<img width=300px src='https://raw.githubusercontent.com/Lud-lud/text_mining_sentiment_analysis/refs/heads/main/foto_mochila.png' alt='foto do produto'>

A análise por meio de nuvem de palavras mostrou os seguintes bigramas negativos:

<img width=500px src='https://github.com/Lud-lud/text_mining_sentiment_analysis/blob/main/nuvem_bigramas.png' alt='nuvem de bigramas'>

Observou-se que as palavras negativas ocorrem com menor frequência do que suas correspondentes afirmativas:

<img width=500px src='https://raw.githubusercontent.com/Lud-lud/text_mining_sentiment_analysis/refs/heads/main/frequencia_tokens.png' alt='frequência de tokens afirmativos e negativos'>

A nuvem de sentimentos mostrou uma leve tendência de maior frequência de sentimentos negativos:

<img width=500px src='https://raw.githubusercontent.com/Lud-lud/text_mining_sentiment_analysis/refs/heads/main/nuvem_sentimentos.png' alt='nuvem de sentimentos'>

Esta tendência pode ser confirmada por análise quantitativa de sentimentos, na qual foram observados 71 registros de sentimentos positivos a mais do que negativos.

Foi desenvolvido um índice geral de satisfação para compreender a magnitude deste valor, que varia de -1 a 1 (quanto mais próximo de -1, mais negativo; quanto mais próximo de 1, mais positivo). O índice foi de 0,23, indicando que o sentimento geral foi levemente positivo. A percepção de fragilidade do produto possivelmente impediu que o índice fosse ainda mais positivo.

### Análise preditiva

Foram desenvolvidos dois modelos de classificação, Naive Bayes e Suport Vector Machine (SVM), a partir de avaliações de produtos no site Buscapé.

A acurácia do modelo Naive Bayes foi de 86,75% e o SVM, 90,12%.

Os modelos foram aplicados aos 700 comentários sobre a mochila e verificou-se que, com Naive Bayes, 669 foram classificados como negativos e 31 como positivos, e com SVM, todos os comentários foram classificados como negativos. Isso se deve às diferenças na sensibilidade e especificidade dos modelos.

Uma breve análise visual indica que a acurácia dos comentários negativos com o modelo Naive Bayes é de 100%, enquanto a dos positivos é de 50%.

Veja todos os detalhes do projeto [aqui](https://github.com/Lud-lud/avaliacao_produto_text_mining_sentiment_analysis/blob/main/text_mining_sentiment_analysis_portuguese_r.ipynb).
