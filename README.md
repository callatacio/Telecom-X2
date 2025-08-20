# Telecom-X2


Telecom X - Parte 2: Prevendo Churn

Resumo do que foi feito e os principais insights obtidos:

Pipeline de Modelagem Preditiva
Pré-processamento de Dados:

Mantive a limpeza e a normalização dos dados que realizamos na primeira parte.

As variáveis categóricas (como gender, InternetService, Contract, etc.) foram transformadas em um formato numérico, usando a técnica de One-Hot Encoding.

As variáveis numéricas (tenure, MonthlyCharges, TotalCharges) foram padronizadas para garantir que todas tivessem a mesma escala, o que é fundamental para a performance de muitos algoritmos de Machine Learning.

O conjunto de dados foi dividido em 80% para treino e 20% para teste, garantindo uma avaliação imparcial.

Treinamento e Avaliação de Modelos:

Treinei dois modelos de classificação: Regressão Logística e Random Forest Classifier.

A acurácia de ambos os modelos no conjunto de teste foi de 80%, o que é um bom resultado, considerando o tamanho e a natureza dos dados.

Resultados e Interpretação Estratégica:

Os modelos validam e aprofundam os insights da nossa análise exploratória, confirmando as variáveis mais importantes na previsão da evasão de clientes. O modelo Random Forest foi particularmente útil para entender quais fatores têm maior peso na decisão de um cliente de cancelar.

Aqui estão os 3 principais fatores que influenciam a evasão, ranqueados por ordem de importância:

Tempo de Contrato (tenure): A variável tenure é, de longe, o fator mais importante. A análise da média de permanência já havia indicado que clientes que cancelam têm uma média de permanência (17.51 meses) muito menor do que os que permanecem (39.88 meses). Isso mostra que a lealdade do cliente é o preditor mais forte de permanência.

Encargos Totais (TotalCharges): Os valores totais cobrados também são um fator crucial. A importância dessa variável pode sugerir que os clientes insatisfeitos com os serviços não permanecem tempo suficiente para acumular um alto valor de cobrança, reforçando a relação com a permanência (tenure).

Encargos Mensais (MonthlyCharges): A taxa mensal de serviço é o terceiro fator mais relevante. Isso pode indicar que clientes que têm um alto valor de cobrança mensal, sem os benefícios percebidos para justificar o custo, são mais propensos a cancelar.

Conclusão e Próximos Passos
Os modelos preditivos demonstram que o tempo de permanência do cliente e os valores cobrados são os fatores mais importantes na previsão de evasão.

Para a Telecom X, isso significa que as estratégias de retenção devem ser focadas em:

Identificar Clientes Recém-Chegados: O foco deve ser nos clientes com baixo tempo de permanência, pois eles são os mais propensos a cancelar.

Monitorar Custos: Deve ser feita uma análise para entender se os clientes com alta cobrança mensal percebem o valor do serviço, evitando que o preço seja um fator de insatisfação.

Com os modelos treinados e os insights sobre as variáveis mais importantes, a equipe de Machine Learning tem um ponto de partida sólido para criar modelos ainda mais sofisticados e desenvolver ações de retenção.
