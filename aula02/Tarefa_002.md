### Tarefa 002 - 28/07/2021 - Pesquisa Rest API


## Rest API

![How API works. Source: Medium](https://miro.medium.com/max/700/1*-SWhP6Ft-2s3U2w-_IUeuQ.png)

*Fonte da imagem: How API works. Source: Medium*

**API**

Application Programming Interface (Interface de Programação de Aplicativo), ou API é uma interface e como toda interface serve para permitir a interação, sendo indicada para a integração entre aplicações; é um intermediário de software que permite que dois aplicativos se comuniquem; pode ser referida como uma ponte que se comunica entre o cliente e o servidor. 

*Ex.: A API é simplesmente como um garçom em um hotel, que atende a solicitação do cliente fornecendo o prato ou comida necessária, neste caso, o Cliente solicita uma Solicitação e uma resposta é atendida por meio da API.*


**Rest**

A API RESTful também é conhecida como um serviço da web RESTful que é baseado na tecnologia Representation State Transfer (REST), sugere criar um objeto dos dados solicitados pelo cliente e enviar os valores do objeto em resposta ao usuário. Basicamente, REST, é um estilo de arquitetura, bem como uma abordagem para fins de comunicação que é frequentemente usada no desenvolvimento de vários serviços web.

    Definição: É uma interface de programa de aplicativo (API) que usa solicitações HTTP para dados GET, PUT, POST e DELETE.


**API REST**

Uma API, ou interface de programação de aplicativo, é um conjunto de regras que definem como os aplicativos ou dispositivos podem se conectar e se comunicar uns com os outros. Uma API REST é uma API que está em conformidade com os princípios de design do REST, ou estilo de arquitetura de transferência de estado representacional. Por esse motivo, às vezes, as APIs REST são chamadas de APIs RESTful. 

Definido pela primeira vez em 2000 pelo cientista da computação Dr. Roy Fielding em sua tese de doutorado, o REST fornece um nível relativamente alto de flexibilidade e liberdade para desenvolvedores. Essa flexibilidade é apenas um motivo pelo qual as APIs REST surgiram como um método comum para conectar componentes e aplicativos em uma arquitetura de microsserviços. Alguns sites como o Facebook e o Twitter disponibilizam algumas dessas APIs a desenvolvedores externos para construir suas próprias ferramentas e sistemas. 

Podemos nos comunicar com APIs REST usando solicitações HTTP, da mesma forma que você faria para navegar em um site ou carregar uma imagem. Podemos fazer solicitações HTTP para determinados urls de API e esses urls retornariam as informações solicitadas, ou podemos enviar dados para um url de API para alterar alguns dados em um banco de dados.

Normalmente, enviamos solicitações HTTP para uma URL que definimos em nossa API REST e ela executaria uma determinada tarefa para nós ou retornaria um determinado bit de dados. A maioria das APIs hoje em dia retornaria uma resposta para nós na forma de JSON.

Os aplicativos modernos de hoje usam o conceito de API REST, a API REST nada mais é do que o estilo arquitetônico para acessar os recursos por meio de diferentes serviços Web Restful. A API REST hoje em dia, usa quase todos os tipos de aplicativos, ou seja, aplicativos da Web e também aplicativos nativos

1. Métodos importantes da API REST:  

   * Método HTTP GET
   Método GET, é utilizado para obter ou buscar todos ou recursos específicos entre o servidor da web. Este método é comumente usado para mostrar dados para o lado do cliente.

   * Método HTTP POST
   O método POST é utilizado para passar os dados do cliente para o servidor. 

   * Método HTTP PUT
   O método PUT é o método para atualizar os dados presentes no Banco de Dados, este método pode ser usado para alterar os valores que são salvos no Banco de Dados.

   * Método HTTP DELETE
   Como o nome fala, usamos o método HTTP DELETE para deletar recursos específicos ou todos entre o Banco de Dados.

2. Conjunto de recomendações e restrições para serviços da Web RESTful: ( _vale ressaltar que não é uma regra_) 

   * Cliente-servidor
   É idêntico ao funcionamento de um navegador. O aplicativo faz uma solicitação para um URL específico. A solicitação é roteada para um servidor da web que retorna uma página HTML. Essa página pode conter referências a imagens, folhas de estilo e JavaScript, que geram mais solicitações e respostas.

   * Stateless
   REST não tem estado: a solicitação do cliente deve conter todas as informações necessárias para responder a uma solicitação. 

   * Armazenável em cache
   Uma resposta deve ser definida como armazenável em cache ou não.

   * Em camadas
   O cliente solicitante não precisa saber se está se comunicando com o servidor real, um proxy ou qualquer outro intermediário. Com o REST, os componentes em rede são um recurso ao qual o usuário solicita acesso - como uma caixa preta cujos detalhes de implementação não são claros. Todas as chamadas são sem estado; nada pode ser retido pelo serviço RESTful entre as execuções.

   * Interface
   Uma interface uniforme deve ser usada entre o cliente e o servidor para todas as APIs. Uma vez que o desenvolvedor tenha trabalhado em uma API de uma classe, ele deve ser facilmente capaz de trabalhar em outras APIs da mesma classe. Ao aplicar uma interface uniforme, a arquitetura é simplificada e a compreensão das APIs é aprimorada. Torna-se mais fácil para alguém implementar a API, pois a interface padrão é a mesma. 

        Os quatro princípios orientadores da interface uniforme são os seguintes:
        - Baseada em recursos;
        - Manipulação de recursos por meio de representações;
        - Mensagens autodescritivas; 
        - Hipermídia como motor do estado do aplicativo (HATEOAS);

3. Os formatos de dados que a API REST suporta incluem:

      * application / json
      * aplicação / xml
      * aplicativo / x-wbe + xml
      * application / x-www-form-urlencoded
      * multipart / form-data

**Fonte** 

- https://www.ibm.com/cloud/learn/rest-apis
- https://brijeshpanchal1618.medium.com/what-is-a-restful-api-and-its-methods-63195758cde2
- https://www.sitepoint.com/rest-api/
- https://searchapparchitecture.techtarget.com/definition/RESTful-API
- https://medium.com/@lazlojuly/what-is-a-restful-api-fabb8dc2afeb