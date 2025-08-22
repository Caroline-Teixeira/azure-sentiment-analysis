# Análise de Sentimentos com Language Studio no Azure AI

A análise de sentimento e a mineração de opiniões são recursos oferecidos pelo Microsoft Azure, os quais ajudam você a descobrir o que as pessoas pensam sobre sua marca ou tópico analisando texto em busca de sinais de sentimento positivo ou negativo. Eles também podem vincular esses sentimentos a aspectos específicos do texto.
Esse repositório mostra alguns exemplos de testes na plataforma. Os procedimentos foram realizados como parte do Bootcamp Randstad - Análise de Dados, promovido pela DIO.

## Passo 1 - Criação de um recurso de linguagem no portal da Azure

1. Crie a conta no Azure. Pode-se usar a conta Microsoft.
2. Em seguida crie um recurso acessando o site https://portal.azure.com:
  <img width="1293" height="590" alt="image" src="https://github.com/user-attachments/assets/4da12657-f40d-45e4-9c26-b0f6800f0f21" />
3. Clique em **IA + Machine Learning** e em seguida **Serviço de Linguagem** :
<img width="1298" height="595" alt="azure 2" src="https://github.com/user-attachments/assets/611cb367-84fb-4a6b-9d40-6a1e9b499a5f" />
<br>
4. Caso não queria adicionar outras features, clique em **Continue to create your resource** :
<img width="1298" height="595" alt="azure 3" src="https://github.com/user-attachments/assets/6366368a-55b9-45ce-bd35-fb5a1f9db43b" />
5. Preencha todos os campos obrigatórios, depois clique me **Examinar + Criar** :
<img width="1298" height="595" alt="azure 4" src="https://github.com/user-attachments/assets/a45cc984-965e-4633-af79-e20dc7f0ca07" />
<img width="1298" height="595" alt="azure 5" src="https://github.com/user-attachments/assets/bdcab614-4c12-4f25-8cc5-5c4b4679762e" />
6. Após a etapa de verificação, clique em **criar** e aguarde a implementação ser concluída:
<img width="1298" height="595" alt="azure 6" src="https://github.com/user-attachments/assets/1bce28d7-055e-4269-9665-aa26ddf0ba8b" />
<img width="1298" height="595" alt="azure 7" src="https://github.com/user-attachments/assets/498a884f-614e-4c05-b8a0-59d233884a3b" />
<img width="1298" height="595" alt="azure 8" src="https://github.com/user-attachments/assets/cfa5428c-8bda-4f05-b6bc-8a1d14e5803f" />

## Passo 2 - Análise de Sentimentos

1. Acesse https://language.cognitive.azure.com/ e entre com sua conta Microsoft.
2. Ao logar, selecione o recurso Azure recém criado:
<img width="1298" height="595" alt="azure 9" src="https://github.com/user-attachments/assets/46c75313-76e1-467a-a781-643d821605a4" />
3. Na tela inicial, selecione **Classify text** e depois em **Analyse Sentime and mine opinions**
<img width="1298" height="595" alt="azure 10" src="https://github.com/user-attachments/assets/8220d40a-9cdf-4354-bf9e-dd6f2b8728ad" />
<img width="1298" height="595" alt="azure 11" src="https://github.com/user-attachments/assets/ffc49342-84ee-469d-a781-13d6f4290a39" />
4. Selecione o idioma e insira o texto a ser analisado.
<img width="1298" height="595" alt="azure 12" src="https://github.com/user-attachments/assets/fe7edba5-66e6-4c73-bb4a-5b3fd7b5745e" />

## Resultados

Foram analisados duas opiniões diferentes sobre o mesmo produto / serviço. Disponível em: https://www.zattini.com.br/p/scarpin-vizzano-salto-medio-bico-fino-E11-7358-006

### Opinião 1
Abaixo podemos ver o resultado da análise de sentimento de uma opinião positiva.
<br>
```Amo a marca Vizzano. É um produto que eu compro e indico de olhos fechados. Espero que continue assim, para não decepcionar o cliente que que confia e compra os calçados Vizzano.```

Ao analisar ```Amo a marca Vizzano```, o resultado é positivo (100%), em que o cliente mostra satisfação em relação ao produto.

<img width="489" height="332" alt="azure 13" src="https://github.com/user-attachments/assets/c5b06889-d640-4095-b65d-877a272fb860" /><img width="489" height="332" alt="azure 14" src="https://github.com/user-attachments/assets/83953315-4fa0-4dd0-8712-1312e42eeb3f" />

Agora ao analisar ```É um produto que eu compro e indico de olhos fechados.```, obtemos um comportamento interessante: de acordo com a ferramenta o sentimento é majoritariamente neutro (96%), sendo que deveria ser considerado majoritariamente positiva, já que a cliente confia bastante na marca para comprar "de olhos fechados".
<br>
<img width="489" height="332" alt="azure 15" src="https://github.com/user-attachments/assets/93de4769-f3e2-4645-baef-6f74a20a868a" />

Finalizando, a frase final foi classificada como positiva, em que a cliente espera que a marca continue entregando produtos de qualidade.
<img width="740" height="327" alt="azure 16" src="https://github.com/user-attachments/assets/7f249f0f-daf8-4aa5-973d-91a4d5a41935" />
