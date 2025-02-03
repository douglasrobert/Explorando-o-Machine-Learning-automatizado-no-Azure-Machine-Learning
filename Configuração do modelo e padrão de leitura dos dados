Azure Inteligência Artificial(IA) - Configuração do modelo e padrão de leitura dos dados
Objetivo é configurar o serviço de Machine Learning para ler a base de dados e apresentar os resultado.

Ferramentas utilizadas:
Azure: https://azure.microsoft.com/pt-br/get-started/azure-portal/
Azure ML: https://ml.azure.com/
Serviço da Azure: Azure Machine Learning
Pontos Importantes:
Caso esteja realizando apenas um prática de estudo, no final excluir tudo que foi construído nesse laboratório. Desta forma, minimiza o risco de ser cobrado algum valor. Lembre-se você está em um ambiente real de produção.

Links uteis com detalhamento:

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html

https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html

Resumo (Passo-a-passo): Configuração Machine Learning:
Ir para "Go to Resouce"
Clicar em "Launch studio"
Abrirá uma pagina nova então selecionar o workspace criando anteriormente
Clicar no botão "Automated ML"
Selecionar o item "New automated job"
Preencher "Basic setting"
Preencher "Task type & data"
Detalhamento para configuração Machine Learning:

01 - Clicar no botão no final da tela: Go to Resouce
02 - Clicar no botão Launch studio
03 - Então, abrirá uma nova pagina com endereço: https://ml.azure.com/. Pode acontece de abrir e não está logado. Então precisa fazer o login. Após fazer o login, clicar em "Automated ML"

Perceba que o Workspace que você criou no passo anterior (https://github.com/WanderBernardo/AzureIA_MachineLearning_Workspace), já aparece.

Caso não apareça, então, clicar em "All workspaces" e selecionar o Workspaces que foi criado anteriormente.

04 - Selecionar a item: New Automated job

05 - A partir de agora, preencher conforme o padrão solicitado. Pois estamos executando exercicio disponibilizado pela microsoft. Mas na vida real, incluir os dados compativel com modelo que estão desenvolvendo. Pós preenchimento clicar em Next

Job name: mslearn-bike-automl
Experiment name: Padrão do sistema, não alterar.
New experiment name: mslearn-bike-rental
Description: Automated machine learning for bike rental prediction
Tag: none

06 - Preencher com os dados Task type & data

Select task type: aqui que tipo de tarefa será realizado: uma regressão, classificação, entre outras. No nosso caso, será uma Regressão

07 - Na parte Select data , clicar no botão Create . Então, vai abrir uma tela para preencher, após preenchimento clicar em: Next

Data type:
Name: Não incluir dados sensiveis ou confidencias. No nosso modelo será: bike-rentals
Description: Historic bike rental data
Type: Table (mltable) - Aqui tem link para mais informações para melhor o entendimento do tipo de dados você consegue trabalhar. No nosso caso estamos usando um CSV.

Data source: Selecionar a opção From local files depois Next

Nesta proxima tela mantém a configuração padrão em seguida Next

Datastore type: Azure Blob Storage
Name: workspaceblobstore

08 - Neste próximo passo, será necessário baixar o arquivo de exemplo que vamos usar e descompactar (em anexo). Link para baixar: https://aka.ms/bike-rentals
09 - Então deve fazer o upload do arquivo e Next
10 - Agora, o neste próximo passo o sistema vai validar as configurações. Quando concluir vai mostrar a tela com resumo das configurações e o botão create ativo. Click no bortão e aguardar concluir. Não sair da tela até concluir.
11 - Vai apresentar uma mensagem de sucesso na parte superior e em seguida, selecionar a opção criado, pois foi o que você criou nos passos anterior e Next
12 - Agora neste passo, a configuração necessaria é selecionar Target column: rentals (Integer)

E abaixo do campo acima selecionar e ajustar: View additional configuration settings

Então, vai abrir uma nova tela onde vai precisar desmarcar as 3 opções:

* - Explain best model
* - Enable ensemble stacking
* - Use all supported models E na opção: Allowed models, selecionar "RandomForest" e "LightGBM"

Reforçando, que essa configuração é para o nosso exemplo. Cada caso, precisa ser analisado qual configuração será necessário.

13 - Agora, nessa parte da configuração "Limits", irá configurar o tempo limite timeout, máximo de avaliação etc. Basicamente, são os paramêtros para indicar o limite e tempo de pesquisas vai ser realizado para apresentar o resultado.
14 - Neste parte, Validate and test, preencher conforme abaixo e Next

Validation type: Train-validation split
Percentage validation of data: 10
Test data: None

15 - Agora, selecionar as configuração o desempenho que gostaria dedicar para realizar essa tarefa. Mantém a configuração padrão. Então, Next
16 - Vai apresentar uma tela com resumo das configurações realizadas e clicar em Submit training job

Não saia da tela. Aguardar concluir:

Status de concluído:

Próximo Passo
