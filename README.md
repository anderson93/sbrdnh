# Projeto de Regressão Múltipla usando Redes Multilayer Perceptron

  Projeto realizado como trabalho de conclusão da matéria de Redes Neurais, ministrada pelo Prof. Dr. Mêuser Valença. O trabalho foi realizado por mim e pela [@patyd](https://github.com/patyd).

# Dados

  Os dados foram fornecidos pelo professor, são medições do nível de água da barragem do município Sobradinho-BA. As medições compreendem de 1931 a 2015, dentre os meses de Janeiro a Dezembro.

# Análise exploratória dos dados
  
   Foi feito uma análise estatística e exploratória dos dados, a fim de se confirmar teorias relacionadas à estrutura e dinâmica dos dados. Por serem dados de caráter temporal, há-se a necessidade de trata-los como tal, analisamos assim a correlação, estacionaridade Dickey-Fuller, tendências, sazonalidades, resíduos, autocorrelação entre outros.

# Modelagem da rede neural
  
  Através dos resultados das análises dos dados, podemos sugerir arquiteturas para a rede neural e então testar essas hipóteses:

* Meses como entrada: [1, 2, 3, 6, 12]
* Funções de ativação: ['PReLU', 'LeakyReLU','tanh','relu']
* Camadas escondidas: [5, 12, 16, 24, 36]
* Número de iterações máxima: [600]

  Para esses testes, criamos a combinação de todos os parâmetros para testarmos todas as possibilidades possíveis. Utilizamos também optimizadores para evitar overfitting e outros métodos para evitar o aumento do erro ao longo das iterações.

# Resultados

  Apresentamos então os resultados baseados na métrica Loss e Mean Average Error. Baseado nos resultados dos testes, selecionamos a melhor arquitetura da rede.
