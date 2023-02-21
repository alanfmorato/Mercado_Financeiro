# Mercado_Financeiro

Com a movimentação no mercado financeiro tomando grandes proporções ao longo dos últimos anos, decidi analisar alguns dados sobre isso.

Primeiramente fiz uma análise simpls da correlaçâo entre as variáveis, onde descobrimos que a quantidade de negócios tem correlação com o volume e quantidade de ações.

![image](https://user-images.githubusercontent.com/102003274/220444987-5fc3ae9c-2bfa-437c-90cb-dc0ba82dba37.png)


Após descobrir a dependência entre as variáveis, comecei uma análise de séries temporais, onde percebe-se que houve um grande pico de movimentações em 2019, e após isso houve uma queda em 2020, podendo haver correlação com o COVID-19.

![image](https://user-images.githubusercontent.com/102003274/220445262-2fd92030-2be2-46ea-8378-9e7622d9ed79.png)

Após treinar o modelo com a variável principal sendo a coluna negócios, e as variáveis secundárias sendo Volume e acoes, chegamos a um modelo de 78% de acuracidade no treino e 83% no previsto.

Para testar o modelo, podemos passar os seguintes atributos:
Volume = 
acoes = 
entrada = [[Volume,acoes]]
modelo.predict(entrada)[0]

Com isso ele vai calcular o número de negócios que vão ser realizados.
