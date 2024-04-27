
# Abadono Zero

- #### Link para os diagramas [aqui](https://drive.google.com/drive/folders/1nJ14rC7VMY--lSyHyKkfx7KL_4W7L1ep?usp=sharing).

- #### Descrição: 
&nbsp;&nbsp;&nbsp;&nbsp;O projeto consiste no desenvolvimento de uma aplicação web dedicada à coleta de informações sobre o comportamento dos tutores em relação à adoção, compra e eventual abandono de cães. Por meio de um formulário de fácil acesso, os tutores poderão fornecer dados relevantes, enquanto a aplicação os armazena e organiza em uma base de dados estruturada. Dessa forma, essas informações serão essenciais para compreender as razões por trás do abandono de animais a partir de uma análise detalhada das condições dos tutores envolvidos. 
- #### Arquitetura: 
&nbsp;&nbsp;&nbsp;&nbsp;MVC (Model-View-Controller)
- #### Ferramenta de Diagramação: 
&nbsp;&nbsp;&nbsp;&nbsp;A ferramenta utilizada foi o [draw.io](https://app.diagrams.net/).
- ### Modelos (Models):
<div align="center">
<sub>Quadro 01 - Entidades</sub>
</div>
<div align="center">

| Entidade | Descrição | Atributos |
| ------- | -------- | ------------|
| Usuários   | Armazena os dados essenciais para a realização do cadastro e a chave para o próximo formulário.    | ID, data de cadastramento, email, senha, data de nascimento, foreign key formulário |
| Formulário 0   | Armazena os dados do formulário inicial com os dados do usuário e a chave para qual será o formulário que ele irá responder em seguida.    | ID, nome, nome social, celular, país, estado/região, cidade, bairro, escolaridade, constituição familiar, faixa de renda familiar, tipo de moradia, número de moradores da casa, foreign key formulários|
| Formulário 1 (presente)  | Armazena os dados correspondentes às perguntas feitas a quem possui cachorro.    | ID, Pergunta 1, Pergunta 2, ...|
| Formulário 2 (passado)   | Armazena os dados correspondentes às perguntas feitas a quem já teve algum cachorro.    | ID, Pergunta 1, Pergunta 2, ...|
| Formulário 3 (futuro) | Armazena os dados correspondentes às perguntas feitas a quem quer ter cachorro.    | ID, Pergunta 1, Pergunta 2, ...|
| Formulário 4 (null)  | Armazena os dados correspondentes às perguntas feitas a quem não tem e não quer ter cachorro.    | ID, Pergunta 1, Pergunta 2, ...|

</div>
<div align="center">
<sup>Fonte: Material produzido pela autora (2024)</sup>
</div>
&nbsp;&nbsp;&nbsp;&nbsp;A entidade Usuários relaciona-se com a entidade Formulário 0, sendo que para um usuário pode haver várias respostas (é possível responder novamente após determinado período de tempo); portanto, as relações são 1:N. Ademais, a entidade Formulário 0 relaciona-se com as entidades Formulário 1, Formulário 2, Formulário 3 e Formulário 4, sendo que para cada vez que o Formulário 0 é preenchido é possível responder apenas uma vez a algum dos demais formulários; logo, a relação é 1:1.

- ### Controladores (Controllers):
- Tela do Administrador <br>
&nbsp;&nbsp;&nbsp;&nbsp;Liste os controladores do seu projeto e suas responsabilidades.
<div align="center">
<sub>Qaudro 2 - Controllers</sub>
</div>

<div align="center">

| Methods | Parâmetros |
| ------- | -------- |
| Texto   | Texto    |
| Texto   | Texto    |
| Texto   | Texto    |

</div>

<div align="center">
<sup>Fonte: Material produzido pela autora (2024)</sup>
</div>

Descreva as ações (methods) de cada controlador e seus parâmetros de entrada e saída.
&nbsp;&nbsp;&nbsp;&nbsp;Explique como os controladores interagem com os modelos e views.
- Tela do Administrador <br>
&nbsp;&nbsp;&nbsp;&nbsp;Liste os controladores do seu projeto e suas responsabilidades.
<div align="center">
<sub>Qaudro 2 - Controllers</sub>
</div>

<div align="center">

| Methods | Parâmetros |
| ------- | -------- |
| Texto   | Texto    |
| Texto   | Texto    |
| Texto   | Texto    |

</div>

<div align="center">
<sup>Fonte: Material produzido pela autora (2024)</sup>
</div>

Descreva as ações (methods) de cada controlador e seus parâmetros de entrada e saída.
&nbsp;&nbsp;&nbsp;&nbsp;Explique como os controladores interagem com os modelos e views.

- Tela do Administrador <br>
&nbsp;&nbsp;&nbsp;&nbsp;Liste os controladores do seu projeto e suas responsabilidades.
<div align="center">
<sub>Qaudro 2 - Controllers</sub>
</div>

<div align="center">

| Methods | Parâmetros |
| ------- | -------- |
| Texto   | Texto    |
| Texto   | Texto    |
| Texto   | Texto    |

</div>

<div align="center">
<sup>Fonte: Material produzido pela autora (2024)</sup>
</div>

Descreva as ações (methods) de cada controlador e seus parâmetros de entrada e saída.
&nbsp;&nbsp;&nbsp;&nbsp;Explique como os controladores interagem com os modelos e views.

- ### Views (Views):
&nbsp;&nbsp;&nbsp;&nbsp;Liste as views do seu projeto e sua função.

- #### Infraestrutura:
&nbsp;&nbsp;&nbsp;&nbsp;Descreva os componentes de infraestrutura do seu projeto, como bancos de dados, APIs externas e outras dependências.
Explique como a infraestrutura se integra à arquitetura MVC.
Justifique as escolhas feitas e como elas impactam o projeto.

- #### Implicações da Arquitetura:
&nbsp;&nbsp;&nbsp;&nbsp;Descreva as implicações da arquitetura em termos de escalabilidade, manutenção, testabilidade e outros aspectos importantes.
