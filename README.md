<h3>Web Services RESTful e Spring</h3>


Representational State Transfer (REST) - É um modelo arquitetural que a web se baseia. Possui algumas regras básicas!

Web: escalável (possibilita vários usuários e páginas), incremental (se adapta a novas tecnologias), simples (http), extensível, global (independente do local, o alcance é mundial). 

Application Programming Interface (API) - Permite que sistemas distintos se interagem de alguma forma (interface padrão de comunicação entre dois módulos/sistemas distintos). 
Constraints para ser considerado API REST: 
- cliente/servidor;
- stateless (não mantém estado);
- cache;
- interface uniforme (modelar e gerenciar recursos);
- sistema em camadas (permitir que a requisição passe por elementos intermediários); 
- código sob demanda;
- representações (formato no qual o cliente solicita no momento);
- Hypermedia as the Engine of Application State (Hateoas) - permite que a partir de um determinado recurso, é demonstrado as futuras ações a partir do estado atual;

Hypertext Transfer Protocol (HTTP): Modelo request/response 
Física;
Enlace;
Rede IP (camada responsável for fazer com que a informação saia de um lugar e chega até outro);
Transporte TCP (identificar qual aplicaçaõ na qual se deseja comunicar);
Aplicação HTTP (codifica/configura o que a aplicação vai fazer);

Universal Resource Identifier (URI).

Métodos e respotas HTTP

* GET - utilizado quando existe a necessidade de se obter um recurso;
* POST - utiliza-se o método POST quando deseja criar um recurso;
* PUT - semelhante ao método POST, esse método permite atualizar um recurso já existente;
* DELETE - é utilizado quando existe a necessidade de remoção de um recurso;

Respostas:
* 1xx: informações gerais;
* 2xx: sucesso;
* 3xx: redicerionamento;
* 4xx: erro no cliente;
* 5xx: erro no servidor;

JSON - JavaScript Object Notation: formato para intercâmbio de dados.
Notação: sistema de caracteres para representar dados, por exemplo, número e palavras. 
Portabilidade: transmite informações independente de tecnologia utilizada.
Facilidade de entendimento: representa dados de maneira padronizada em relação aos conceitos universais de programação.


```
Sintaxe:

Objeto
[
{
"nome": "Workshop Rest",
"instrutor": "Emílio Dias",
"duracao": "6hrs"
},
{
"nome": "Workshop Rest",
"instrutor": "Normandes Junior",
"duracao": "6hrs"
}
]

* Nesse caso, o objeto JSON possui 3 atributos (chave-valor). Além disso, adicionou-se as listas de informações, nesse caso, uma lista com 2 objetos.

*Números, Strings, Objetos e Booleanos:
{
"nome": "Workshop Rest",
"instrutor": {"nome": "Normandes Junior"},  //dentro de um objeto é possível ter um atributo que também é um objeto.
"duracao": 6,
"ativo": true
}

```
Modelo de Maturidade Richardson:

** Nível 0: POX - Plain Old XML:
* Modelo RPC (exposição para execução de métodos remotos);
* HTTP apenas como transporte;
* Semelhante ao uso de SOAP ou XML-RPC;

<p align="center">
  <img width="500" src="https://github.com/Jennyads/Web-Services-RESTful-e-Spring/blob/main/Imagens/niveo%200.png">
</p>
observação: nesse nível, usa-se verbos para obter a URI.

** Nível 1 - Já consegue mapear recursos.

** Nível 2: Utilização dos métodos e respostas do protocolo HTTP de forma adequada.
<p align="center">
  <img width="500" src="https://github.com/Jennyads/Web-Services-RESTful-e-Spring/blob/main/Imagens/n%C3%ADvel%202.png">
</p>

