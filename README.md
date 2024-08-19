# Estudo para Discretização e Classificação para Reduzir a Evasão de Abandono de Carrinho em E-commerce

No caso de uso proposto como exemplo durante a aula, foi apresentada a previsão de churn em empresas de telecomunicações. A ideia central foi demonstrar como as técnicas de discretização e classificação podem ser usadas para prever e reduzir o número de evasões de clientes. Essas técnicas permitem que a empresa identifique quais clientes têm maior probabilidade de cancelar seus contratos e migrarem para concorrentes, permitindo assim a implementação de estratégias de retenção, como a oferta de descontos ou melhorias no serviço.

Com base nisso, resolvi aplicar os estudos de discretização e classificação para o uso de evasão de abandono de carrinho em e-commerce.




# RESULTADOS

![image](https://github.com/user-attachments/assets/94c5ca3e-a0c6-4cbb-9da8-402bd349dbee)


**Árvore de Decisão:**

- Acurácia: 53.33% — Isso significa que o modelo previu corretamente cerca de 53.33% das vezes no conjunto de teste.
- Validação Cruzada (10-fold): 58.8% — A validação cruzada sugere que, em média, o modelo teve um desempenho de 58.8% de acurácia em diferentes subconjuntos dos dados.

Interpretação: A Árvore de Decisão teve um desempenho modesto, sugerindo que o modelo pode estar tendo dificuldades para capturar os padrões complexos nos dados.

**Rede Neural MLP:**

- Acurácia: 53.33% — Igual à Árvore de Decisão, indicando que, no conjunto de teste, a Rede Neural MLP também não conseguiu superar este limite.
- Validação Cruzada (10-fold): 59.0% — A validação cruzada sugere uma ligeira melhora em relação à Árvore de Decisão, mas ainda é baixa.

Interpretação: Embora a Rede Neural MLP tenha um potencial para capturar padrões complexos, esses resultados indicam os dados disponíveis não são ideais para esse tipo de modelo.

**Naive Bayes:**

- Acurácia: 60.00% — O Naive Bayes teve o melhor desempenho em termos de acurácia, prevendo corretamente 60% dos casos no conjunto de teste.
- Validação Cruzada (10-fold): 60.7% — Isso indica uma consistência decente na generalização dos dados e sugere que o Naive Bayes está se saindo melhor que os outros modelos nesta tarefa específica.

Interpretação: O Naive Bayes, sendo um modelo mais simples e probabilístico, conseguiu captar padrões nos dados de maneira mais eficaz que os outros dois modelos. Isso pode indicar que os dados são adequados para um modelo mais linear ou que as suposições simplificadas do Naive Bayes funcionam bem com esse conjunto de dados.





# RESPONDENDO AS PERGUNTAS 

Como podemos utilizar a discretização e a classificação da mesma forma em uma empresa ou indústria? Responda conforme o apresentado durante a aula.


### Aplicação na Prevenção de Abandono de Carrinho em E-commerce

De forma semelhante, essas mesmas técnicas podem ser aplicadas para ***prevenir o abandono de carrinho em e-commerce***. 
O abandono de carrinho é um problema crítico para lojas online, onde clientes adicionam itens ao carrinho, mas não finalizam a compra. A aplicação de discretização e classificação permite prever quais clientes estão mais propensos a abandonar o carrinho e, assim, permite a implementação de medidas para incentivar a conclusão da compra.

### Discretização
Em ambos os casos, a discretização é a técnica usada para transformar variáveis contínuas, como o tempo gasto em um site ou o tempo de uso de um serviço, em categorias discretas (como "Curto", "Médio", "Longo"). Isso facilita a análise e a aplicação de modelos de machine learning. No e-commerce, por exemplo, o tempo que um cliente passa na página do produto pode ser discretizado para identificar comportamentos associados ao abandono do carrinho.

### Classificação
A classificação é usada para prever comportamentos com base nas variáveis discretizadas. No caso das telecomunicações, a classificação é usada para prever quais clientes têm maior probabilidade de churn (ou seja, de deixar a empresa). No e-commerce, a classificação pode ser usada para prever quais clientes têm maior probabilidade de abandonar o carrinho.

#### Exemplo Prático em E-commerce

- Coleta de Dados: Informações como o tempo gasto na página do produto, o número de visitas ao site, o número de itens no carrinho e o histórico de compras são coletadas para análise.

- Discretização: Esses dados são discretizados. Por exemplo, o tempo na página pode ser categorizado como "Curto", "Médio" ou "Longo", e o valor total do carrinho como "Baixo", "Médio" ou "Alto".

- Classificação: Modelos de machine learning, como Árvore de Decisão, Rede Neural MLP e Naive Bayes, são aplicados para prever se um cliente abandonará o carrinho. A variável alvo aqui seria "Abandono de Carrinho" (sim ou não).

- Implementação de Estratégias de Retenção: Com base nas previsões, a empresa pode enviar um e-mail de lembrete, oferecer um desconto, ou fornecer outros incentivos para que o cliente finalize a compra.

- Assim como a previsão de churn em telecomunicações ajuda a reduzir a perda de clientes, a aplicação das mesmas técnicas em e-commerce pode reduzir significativamente o abandono de carrinho. Ao identificar clientes com maior probabilidade de abandonar suas compras, as empresas podem intervir de maneira proativa para aumentar as taxas de conversão e, consequentemente, a receita.


