Protocolos que habilitam autenticação única
*******************************************

O Cidadão.BR foi projetado e implementado com foco em interoperabilidade, então
respeita e segue os padrões de mercado para habilitar a autenticação única, ou Single Sign-
On. O padrão mais proeminente e utilizado é OAuth, projetado para trabalhar com o procolo
HTTP e ele é essencialmente uma forma de permitir que tokens de acesso sejam emitidos para
clientes terceiros por um servidor de autorização, com a aprovação do proprietário dos
recursos (o usuário normalmente). O OAuth é complemento do protocolo OpenID e tem
relação direta com o OpenID Connect (OIDC), que é uma camada de autenticação construída
em “cima” da versão 2.0 do OAuth.

Sob uma visão de fluxo, o OAuth é uma forma de delegação de acesso a API’s. A
versão 2.0 do OAuth provê fluxos de autorização para aplicações web, desktop, celulares e até
dispositivos IoT. O OAuth 2.0 não suporta, em sua especificação, assinatura digital,
criptografia e verificação do cliente. Ele depende completamente do protocolo TLS (Transport
Layer Security) para obter algum nível de confidencialidade e autenticação do servidor.

A especificação não dita nem detalha como se emitiria os tokens, qual seria seu
formato, implementações específicas e etc. Para isso foi escolhido o padrão JWT (JSON Web
Token). Esses objetos são projetados para serem compactos, passíveis de serem enviados na
URL e usáveis especialmente num contexto de SSO em navegadores. Ele é utilizado
tipicamente para passar a identidade de usuários autenticados entre um provedor de
identidade e um provedor serviço. Eles podem ser criptografados e autenticados.


