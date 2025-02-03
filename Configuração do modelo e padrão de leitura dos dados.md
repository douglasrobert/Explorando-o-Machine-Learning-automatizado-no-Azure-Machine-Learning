# Azure Inteligência Artificial(IA) - Serviço Machine Learning Workspace
Objetivo desse laboratório é demonstrar o processo de configuração para criar um modelo de previsão com seus devidos pontos de extremidade configurados.

### Ferramentas utilizadas:

- Azure: https://azure.microsoft.com/pt-br/get-started/azure-portal/
- Serviço da Azure: ``` Azure Machine Learning ```

### Pontos Importantes:

 - Iniciaremos a configuração do painel de Serviço da Azure. Portanto, a conta já deve está criada.
 - Caso esteja realizando apenas um prática de estudo, no final excluir tudo que foi construído nesse laboratório. Desta forma, minimiza o risco de ser cobrado algum valor. Lembre-se você está em um ambiente real de produção.
 - Links uteis com detalhamento:
   
    * https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html
      
    * https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html

### Resumo (Passo-a-passo): Configuração Machine Learning:

 - Selecionar o serviço de IA Machine Learning
 - Escolher a opção "New Workspace" no botão "Create"
 - Preencher os dados solicitados a Aba "Basics"
 - Demais configurações manter o padrão
 - Validar as configuração e criar

### Detalhamento (Passo-a-passo): Configuração Machine Learning

01 - Selecionar o serviço Azure Machine Learning:

![image](https://github.com/user-attachments/assets/6200a8ae-da6f-4de1-a456-94ca8f9cc6be)

02 - Clicar no botão "Create" na e na opção "New Workspace":

![image](https://github.com/user-attachments/assets/df0da2a7-d736-45a0-9c6f-1fa7468595af)

03 - Preencher os dados solicitados a Aba "Basics":

### - Resource details: 
   * Subscription: é a conta que você está logado. É como se você a sua empresa. Repositótorio geral de tudo que é criado, a Pasta principal. Já vem preenchido de padrão, Esse 
 padrão é criado automaticamente quando realiza o cadastro. Mas pode ser criado outras opções.
   * Resource group: é uma sub-repositório do "Subscription".

Imagina uma gaveteiro onde o gaveteiro inteiro é ``` Subscriptiom ``` e uma gaveta desse gaveteiro é o Resource group.

Essa configuração não tem um padrão exato, fica a critério da empresa. A configuração deve seguir um padrão que é melhor para você, empresa, instituição etc. Por exemplo, divido em projetos, Departamentos, Prédio etc.

 ![image](https://github.com/user-attachments/assets/e75b5773-9022-45b1-944e-a64d9e2afe47)
 Conforme imagem acima perceba que a link destacacado em azul para Saber mais (Learn more...)

 ### - Workspace details
   * Name: nome do seu projeto, modelo (Deve ser único)
   * Region: basicamente, quer dizer em qual servidor da Microsoft você quer salvar. Acredito que também determina a moeda que será cobrado por utilizar esse serviço.
   * Storage account: no nosso exemplo, será preenchido automaticamente, pois estamos criando um novo, então, só manter. Mas caso queira criar uma estrutura pode também. Esse Storage é usado para armazenar os artefatos criados quando rodam o modelo criado.
   * Key Vault: onde é guardando os secredos, certificados, informações confidenciais. No nosso caso, mantemos o que será criado automático. Mas no dia-a-dia, pode ser criado uma estrutura conforme a necessidade.
   * Aplication Insights: basicamente na criação de visões, os graficos para apresentar, monitorar quando tiver novos valores etc.
   * Container registry: manter "None".

![image](https://github.com/user-attachments/assets/224699c0-9be1-4fb2-89ae-cc5a2342dfd8)
Reforçando, caso queira entender melhor os campos acima tem o link destacacado em azul para Saber mais (Learn more...)

04 - Demais Abas: vamos manter o padrão, pois estamos realizando uma configuração basica e iremos excluir esse modelo no final.
   * Networking: configuração de privacidade do seu modelo(Publico/Privado)
   * Encryption: usar encryptação
   * Identity: usar o controle de acesso
   * Tags: muito usado para criar filtros. Por exemplo: Quero fazer rateio para lançamento de custo por Departamento, então, cria as tags por departamento. Conforme sua necessidade.

   ![image](https://github.com/user-attachments/assets/c11e66d3-cccc-464f-b26a-5a1b4a8a9837)


04 - Validar as configurações realizada na Aba ``` Review + create ``` e em seguida clicar no botão ``` create ``` 

Caso não apresente a mensagem  ``` Validaded passed ```, precisa rever as configurações.

![image](https://github.com/user-attachments/assets/be73b4ea-8eff-408a-a6b5-bec0c47d43c3)

Após clicar no botão ``` create ``` , não é o ideal sair da tela. Deixa o processo ser concluído.

![image](https://github.com/user-attachments/assets/1628971a-0c07-4d7b-98a5-d784d2662c51)

### Próximo Passo:

https://github.com/WanderBernardo/AzureIA_MachineLearning_ConfigModel_SetData
