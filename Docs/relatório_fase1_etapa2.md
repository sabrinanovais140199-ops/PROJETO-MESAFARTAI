O motor NLU foi desenvolvido com o objetivo de identificar as intenções dos usuários no sistema de doação de alimentos, reconhecendo mensagens sobre doações, solicitações de alimentos e consultas de status. Para isso, foi utilizado o algoritmo Random Forest junto com a técnica TF-IDF. A seguir, apresento os principais resultados e possíveis melhorias do modelo.

1. Foram utilizadas 80 árvores de decisão no Random Forest. O modelo não utiliza neurônios.

2. O threshold utilizado foi de 0,60 (60%), definindo o nível mínimo de confiança para as previsões.

3. Na primeira execução, a frase sobre doar 30 kg de banana foi identificada como cadastrar_doacao, com 92,5% de confiança. As outras três frases foram classificadas como fallback, com confiança de 41%, 49% e 42%.

4. Para melhorar os resultados, podemos adicionar mais frases ao treinamento, incluir sinônimos, equilibrar as categorias e testar diferentes parâmetros e algoritmos.

5. O Random Forest foi escolhido por combinar várias árvores de decisão, identificar padrões nos textos e estimar probabilidades. Porém, é necessário compará-lo com outros algoritmos para confirmar se é o método mais adequado.
