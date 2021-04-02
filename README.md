# Stack de Gateway Utilizada

Utilizamos o Api Connect da IBM para fazer o papel de Gateway e termos os recursos de segurança, portal do desenvolvedor, analytics, monetização e ciclo de vida das API's.

O serviço é free para até 50K de chamadas/mês. Isso atende muito bem para nosso projeto. Mais informações sobre IBM Cloud - [https://cloud.ibm.com/catalog/services/api-connect#about](https://cloud.ibm.com/catalog/services/api-connect#about).

## Sobre as API's e como utilizar

Foram construídas três API's que foram expostas no Gateway:

1. Support - API responsável por abrir casos de suporte
2. Catalog - API responsável por listar filmes e séries do catálogo
3. User - API responsável por azer login, gerenciar o perfil do usuário

Você precisa passar uma api-key no header, além de um token bearer como Authorization. Ambos são por cliente. Criamos uma para o professor Tadeu. Abaixo tem as chaves deestes headers para serem utilizadas.

`X-IBM-Client-Id: 6680a9a0-a5d2-4958-9d82-dafacef3eb19`

`Authorization: Bearer eyJpc3MiOiJ0b3B0YWwuY29tIiwiZXhwIjoxNDI2NDIwODAwLCJodHRwOi8vd`

## Developer Portal

Mais informações sobre os detalhes das API's, estrutura de dados e exemplos de payloads para chamar, assim como executar testes, você pode fazer diretamente no [portal do desenvolvedor](https://fiap-marciomdantascombr-dev.developer.us.apiconnect.ibmcloud.com).

Este portal também permite de forma self-service com que qualquer pessoa crie uma conta, faça login, depois veja as API's, crie um app que por sua vez com este app pode assinar alguma API com algum plano de 100 chamadas por segundo ou por hora e assim consiga utilizar as API's de forma independente, tornando o processo totalmente seguro no que tange ao recebimento das api-keys para uso.
