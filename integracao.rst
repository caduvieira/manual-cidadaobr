Procedimento de integração
**************************

Para uma nova aplicação se integrar, é necessário que ela se identifique e que possua uma chave criptográfica que a autorize a atuar junto ao provedor de identidades e do servidor de autorização. Esse procedimento, no contexto do Cidadão.BR, é descrito abaixo:

1. Enviar um e-mail para a caixa cidadaobr.dtp@dataprev.gov.br, com as informações a
seguir:
    1. Nome abreviado ou acrônimo que identifique unicamente a aplicação;
    2. Descrição sucinta da aplicação ou serviços;
    3. Descrição mais detalhada da aplicação;
    4. Endereço (URL) da aplicação, na Internet;
    5. Endereço (URL) de sucesso ou retorno após autenticação;
    6. Definir as formas de liberação ou grant type, entre: implícito, por senha ou credenciais de cliente (implicit, password, client_credentials).
2. Aguardar o prazo máximo de 5 dias úteis para a configuração desta nova aplicação no backend do provedor de identidades e serviço de autorização do Cidadão.BR.
3. Será retornado a chave de criptografia específica para configuração da solução de 'cliente' OAuth 2.0. A chave será enviada num arquivo .7z protegido por senha. A senha será a concatenação do nome abreviado da aplicação, os 6 primeiros caracteres da URL (após o https://), um hífen, os 6 últimos caracteres da URL de sucesso, outro hífen e uma sequência de 4 caracteres aleatórios que poderão ser recuperados entrando em contato telefônico com a equipe de Gestão de Serviço
    1. Essa chave é um segredo compartilhado para validação do token JWT, ele deverá ser gerenciado pelo Gateway de API


Contatos na Dataprev
---------------------

============================  =====  ==============================
 Nome                                     Email
============================  =====  ==============================
Alan do Nascimento Santos     
Beatriz Merguiso Garrido      
Ridai Govinda Pombo           
Maciel de Souza Moura         
Marcelo Silva Santos
“Equipe Cidadão.BR Dataprev”          cidadaobr.dtp@dataprev.gov.br
============================  =====  ==============================

