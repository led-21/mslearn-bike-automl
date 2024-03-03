## Trabalhando com Machine Learning na Prática no Azure ML

No exercício proposto foi utilizado o recurso de aprendizado de máquina automatizado do Azure para treinar, avaliar e implantar um modelo que prevê preços de aluguéis de bicicletas.

- No Portal do Azure foi criado um recurso Azure Machine Learning;
- No Estúdio do Azure Machine Learning foi criado um trabalho chamado mslearn-bike-automl, o tipo de tarefa escolhida foi a Regressão e os dados de aluguéis de bicicletas foram obtidos através da URL: https://aka.ms/bike-rentals;
- As tarefas foram configuradas seguindo as especificações do link: [mslearn-ai-fundamentals (microsoftlearning.github.io)](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html), após o trabalho foi submetido para treinamento;
- O treinamento foi criado em Mar 2, 2024 7:50 PM e durou 9min 26.11s;
- Foram analisadas as métricas do melhor modelo;
- O modelo predict-rentals foi implantado com sucesso, sendo testado através de seu ponto de extremidade;

### Dados teste:

`{
   "Inputs": { 
     "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]    
   },   
   "GlobalParameters": 1.0
 }`

### Resultado:

`{
1 item
"Results":[
1 item
0
:
float349.57274611440243
]
}`

- O laboratório foi concluído.
