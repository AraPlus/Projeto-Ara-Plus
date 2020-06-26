# Descrição dos Testes Funcionais de Bancada (in vitro)

## 1) Levantamento da Relação PEEP x Pressão Expiratória Máxima (Vál. VAP) x Freq. Respiratória x Volume Inspirado

### Descrição

### Resultados

Fig. 1: 

![](teste_2020_06_21_fig1.jpeg)

1.1 - VAP tem dispersão da pressão de atuação

1.2 - Sensor condicionado tem boa correlação e linearidade.

1.3 - Equação de ajuste do sensor precisa ser atualizada com o valor do pico dinâmico

1.4 - Será necessário estabelecer procedimento de calibração (analógica e/ou digital)


Fig. 2:

![](teste_2020_06_21_fig2.jpeg)

2.1 - Setup da PEEP impacta na pressão máxima.

2.2 - Pressão máxima tem alta correlação com a soma do setup PEEP+VAP.


Fig. 3:

![](teste_2020_06_21_fig3.jpeg)

3.1 – Hipótese: a pressão máxima (VAP) deve ser ajustada em função de curvas para cada valor de PEEP ajustado.

Fig. 4:

![](teste_2020_06_21_fig4.jpeg)

4.1 - Existe uma correlação razoável entre o volume e a diferença de pressão (VAP-PEEP).

4.2 - Hipótese: Para uma determinada complacência, o volume varia proporcionalmente com a posição do AMBU para qualquer ajuste das válvulas.

4.3 - Hipótese: Para uma determinada complacência, o volume por ciclo não varia proporcionalmente com o tempo de inspiração.



## 2) Calibração Estática do Sensor de Pressão

### Descrição

Levantar curva de pressão medida pelo sensor MPX5500DP comparando com uma medição de pressão estática (com manômetro U ou manômetro analógico)


![](teste_2020_05_31_calibracao_estatica_fig1.png)

Diagrama elétrico do circuito de condicionamento de pressão utilizado no AraPlus


![](teste_2020_05_31_calibracao_estatica_fig2.png)

Implementação do circuito de condicionamento 


![](teste_2020_05_31_calibracao_estatica_fig3.png)

Foto do manômetro em U caseiro utilizado na calibração


### Resultados

![](teste_2020_05_31_calibracao_estatica_fig4.png)




## 3) Calibração Dinâmica (valores simulados)

Comparação das curvas de pressão e volume obtidas com um sensor de reverência (Analisador de Gases Fluke VT650) com as curvas de pressão obtidas com o simulador https://girardi.blumenau.ufsc.br/sdvm/, para os mesmos parâmetros ventilatórios.

## 4) Calibração Dinâmica (valores experimentais)

Comparação das curvas de pressão com um sensor de reverência, com as curvas de pressão efetivamente medidas com o sensor MPX5500DP. Obs: o analisador  Fluke aparentemente só exporta com uma frequência de amostragem máxima de 1Hz, o que não dá uma boa resolução das curvas. A solução seria usar o sensor Magnamed Ventmeter que tem interface RS232.