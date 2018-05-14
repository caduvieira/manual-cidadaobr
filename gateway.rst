Gateway de API
==============

Os tokens emitidos pelo servidor de autorização, já autenticados pelo provedor de
identidades do Cidadão.BR devem ser aceitos pelo usuário; ou seja, ele deve confirmar que
autoriza a aplicação fim a ter acesso a informações necessárias pela aplicação. Por exemplo, a
aplicação Meu INSS precisa acessar e ler o CPF, o NIT e o Nome completo; após autenticar
com sucesso, o usuário precisará permitir o acesso a esses atributos, que compõe o token JWT
emitido. Se ele não permitir, a aplicação não poderá trabalhar corretamente, então o usuário
nem poderá acessar ela.

Os protocolos OAuth 2.0 e JWT são utilizados no contexto de controle de acesso à
API’s, assim fica simples trabalhar com aplicações responsivas, híbridas e nativas de
dispositivos móveis. Para simplificar a forma de trabalho, ter mais governança e
interoperabilidade, cada infraestrutura dessas aplicações utiliza um Gateway de API, um tipo
de software de middleware que controla o acesso às API dos serviços construídos e
suportados. Aplicações internas à infraestrutura da Dataprev utilizam um Gateway na rede
interna. Aplicações externas, terão que possuir seu próprio software, publicá-lo e suportá-lo na
sua própria rede interna ou externa, conforme o caso.

Este Gateway receberá e manterá esses tokens JWT, aplicações que não mantém
estado precisarão armazenar o token recebido do servidor de autorização para que a cada
invocação da API anexem o token, para continuarem autorizadas a utilizá-la.
