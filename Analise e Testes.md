# Azure Inteligência Artificial(IA) - Configurar o Modelo e Validar os Resultados
Objetivo demostrar o resultado dos testes de experimento.

### Ferramentas utilizadas:

- Azure: https://azure.microsoft.com/pt-br/get-started/azure-portal/
- Azure ML: https://ml.azure.com/
- Serviço da Azure: ``` Azure Machine Learning ```

### Pontos Importantes:

 - Caso esteja realizando apenas um prática de estudo, no final excluir tudo que foi construído nesse laboratório. Desta forma, minimiza o risco de ser cobrado algum valor. Lembre-se você está em um ambiente real de produção.
 - Links uteis com detalhamento:
    * https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/02-content-safety.html
    * https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html

### Resumo (Passo-a-passo): Configuração Machine Learning:

 - Verificar se tem algum erro e tratar caso apresente
 - Registrar o "Modelo"
 - Ir me "Metrics" verificar o resultado
   
### Detalhamento (Passo-a-passo): Configuração Machine Learning

01 - Após concluir o passo anterior com o status de concluído. Pode valir se está tudo ok clicando nas outras abas e verificar se apresentou algum erro. Se apresentar algum erro investigar, pois pode ser configuração ou os dados utilizados está com alguma problema de formato, ou padrões erroneo.

![image](https://github.com/user-attachments/assets/47923b9c-424f-4faf-b0d6-3c376c8623c0)

02 - Após validação, ir para ``` Models ``` e registar

![image](https://github.com/user-attachments/assets/e8a46d45-dd9f-4156-88a6-27f1ced7dd5f)

03 - Nesta parte "Select Job", deve selecionar o modelo criado

![image](https://github.com/user-attachments/assets/2f352779-7463-4ed7-9551-d6957a7a6eef)

04 - Agora se tiver tudo certo o sistema já configura automaticamente. Apresenta até uma mensagem informativa. Então, so manter as configurações

![image](https://github.com/user-attachments/assets/1c25ff4a-3cb9-4070-8ea2-86ae4596d19c)

05 - Preencher com os dados para regitrar o modelo e clicar botão "Next":
   * Nome: deve ser unico e não pode ser com dados sensiveis.
   * Description: descrever conforme faz sentido ao seu modelo.
   * Version: Como estamos realizando um novo. Iniciamos com a versão "1".
   * Tag: Opcional.
   
   ![image](https://github.com/user-attachments/assets/d0add228-6c50-49ec-9e0c-affad3ca8373)

06 - Tela de revisão das configurações e clicar em "Register"

![image](https://github.com/user-attachments/assets/68198c9c-fe04-4174-ba4a-34ee4875a7b7)

07 - Após registro, então, voltar para o menu "Jobs" e ir na Aba de "Metrics". O resultado será apresentado do experimento.

![image](https://github.com/user-attachments/assets/b8c3e375-a375-4565-98e1-6a7bd7607704)

![image](https://github.com/user-attachments/assets/6e2796b9-b521-459d-b048-b1c17750d476)

08 - Voltar para aba "Overview" para configurarmos o deploy e testar o modelo:

![image](https://github.com/user-attachments/assets/238ce396-d4f7-4d7e-a426-dfe91549e612)

09 - Agora, precisamos configurar o seridor que irá rodar esse experimento. fechar com o click no botão ``` Deploy  ```
   * Instance count: 3
   * Vitual machine: Standard_E4s_v3 .....

     Caso essa opção não esteja disponivel, selecionar outro. Se não for valida, então vai apresentar uma mensagem abaixo do campo com o alerta.
   * Endpoint: New
     
   Demais campos manter a configuração padrão

![image](https://github.com/user-attachments/assets/c9486ea4-2b02-43db-a848-606e0cb534e2)

Aguardar o processo concluído sem sair da tela

![image](https://github.com/user-attachments/assets/e1e80e90-41f7-433a-9c7a-97cb9c1f2d60)

10 - Agora, ir até a opção ``` Endpoints  ```, selecionar Endpoint criado.

![image](https://github.com/user-attachments/assets/15833d77-a85e-44fc-8c3b-cd25fa15a9d4)

Caso esse ultimo passo apresente erro: ResourceOperationFailure: ``` Resource provider [N/A] isn't registered with Subscription [N/A]  ```. Então, deve realizar uma configuração e refazer a confiuração acima.

   * Ir no portal da Azure: https://portal.azure.com/#home, fazer o login
   * Na barra de pesquisa, escrever "Subscription"
   * Selecionar o Subscription Name
   * Vai abrir um novo menu, então selecionar "Resource providers"
   * Selecionar:
      * Microsoft.Cdn
      * Microsoft.CostManagement
   * Clicar no botão acima "Register".
   
   ![image](https://github.com/user-attachments/assets/79e279f1-96a9-4301-978a-71128c464908)

   Links de ajuda: 
     * https://learn.microsoft.com/en-us/answers/questions/1983847/error-while-creating-a-managed-online-endpoint-in
     * https://learn.microsoft.com/en-us/answers/questions/2129910/resource-provider-(n-a)-isnt-registered-with-subsc

### Próximo Passo

https://github.com/douglasrobert/Explorando-o-Machine-Learning-automatizado-no-Azure-Machine-Learning/blob/main/Configurar%20o%20Modelo%20e%20Validar%20os%20Resultados.md



