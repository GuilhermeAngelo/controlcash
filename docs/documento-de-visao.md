# Documento de visão

## Equipe e definição de papéis

| Membro                              | Papel             | Email                           |
| ----------------------------------- | ----------------- | ------------------------------- |
| Adriel Faria dos Santos             | Gerente, Analista | adriel.fsantos@outlook.com      |
| Alef Luciano Silva                  | Analista          | alef.silva.123@ufrn.edu.br      |
| Bianca Laise Medeiros Cassiano      | Analista          | bianca.medeiros.098@ufrn.edu.br |
| Cintia Campos de Queiroz            | Analista          | cintia.campos.109@ufrn.edu.br   |
| Guilherme Angelo de Medeiros        | Analista          | guilhermeangelo2001@gmail.com   |
| Hilário Petronio de Medeiros Dantas | Analista          | hilariod94@gmail.com            |

## Matriz de copetências

| Membro    | Competências                                                 |
| --------- | ------------------------------------------------------------ |
| Adriel    | Typescript, Javascript, Python, HTML, CSS, Git, SQL, MongoDB |
| Alef      | JavaScript, HTML, CSS, Python, SQL, C                        |
| Bianca    | JavaScript, HTML, CSS, Python, SQL, C++, C                   |
| Cintia    | Comunicação, Proatividade, Liderança                         |
| Guilherme | Python, HTML, Javascript, Git                                |
| Hilário   | Python, HTML, Javascript, Git                                |

## Descrição do projeto

A necessidade do sistema de controle de caixa surgiu com o aumento do fluxo de
vendas de um comércio. O projeto tem como ideal facilitar a logística de entrada
e saída monetária da empresa comercial em questão, bem como o monitoramento de
forma simplificada do estoque, promovendo uma melhoria da eficiência
operacional e do controle das operações financeiras.

### Perfis dos usuários

O sistema poderá ser utilizado por três tipos de usuário.

#### Perfil Gerente

Este usuário tem permissão a todas as áreas do sistema.

#### Perfil Vendedor

Este usuário terá acesso ao controle de venda, controle de pagamentos,
controle de prestações pendentes, formas de pagamento, e gestão de clientes.

#### Perfil Administrador Financeiro

Este usuário terá acesso ao controle de pagamentos e manter despesas.

### Requisitos funcionais

#### RF01 - Manter usuário

Descrição: O sistema deve permitir o cadastro, listagem, visualização e edição
de novos usuários no sistema. Um usuário tem CPF, nome completo, email, data de
nascimento, endereço, salário, telefone, cargo, senha e status. Na listagem
apenas o CPF, nome completo, cargo e status são exibidos. Na visualização de
detalhes todos os atributos são exibidos, exceto senha. A edição de todos os
dados é permitida, mas para alteração de senha, salário ou status o gerente
deve fornecer sua própria senha para confirmar a ação.

Ator: Gerente

#### RF02 - Manter venda

Descrição: O sistema deve permitir o cadastro, listagem e visualização das vendas
realizadas. Cada venda deve conter infromação como data, hora, cliente, itens de
venda, valor total, pagamento e status. Na listagem, apenas informações básicas da venda (data, cliente, valor total e status) devem ser exibidas.

Ator: Vendedor

#### RF03 - Manter produto

Descrição:O sistema deve permitir o cadastro, listagem, visualização e edição de
produtos comercializados pela empresa. Cada produto deve conter informações como
nome, código, descrição, preço de venda e quantidade em estoque. Na listagem,
apenas as informações básicas do produto (nome, código, praço de venda)
devem ser exibidas.

Ator: Gerente

#### RF04 - Pesquisar produto

Descrição: O sistema deve permitir a pesquisa de produtos cadastrados, com a
possibilidade de filtar por nome e categoria. Os resultados da pesquisa devem
exibir as informações básicas dos produtos (nome, código, e preço de venda).

Ator: Gerente, Vendedor

#### RF05 - Manter item de venda

Descrição: O sistema deve permitir ao vendedor adicionar, editar ou remover um
item de venda em uma venda. Cada item deve ter informações como produto,
quantidade, e preço unitário.

Ator: Vendedor

#### RF06 - Manter pagamento de venda

Descrição: O sistema deve permitir ao perfil de vendedor registrar e gerenciar o
pagamento de uma venda. O perfil de vendedor deve selecionar o tipo de pagamento
(dinheiro, cartão de crédito, cartão de débito, etc.) e confirmar o pagamento
recebido. O sistema deve calcular o troco em caso de pagamento em dinheiro.

Ator: Vendedor

#### RF07 - Manter forma de pagamento

Descrição: O sistema deve permitir ao perfil de administrador adicionar, editar
ou remover formas de pagamento aceitas pela loja, como cartões de crédito,
débito, dinheiro, transferência bancária, entre outros. As informações de cada
forma de pagamento devem incluir nome, descrição e taxas aplicáveis (se houver).

Ator: Administrador financeiro

#### RF08 - Manter prestação

Descrição: O sistema deve permitir que os usuários do sistema insiram, atualizem
e consultem as informações de prestação de contas do caixa, incluindo o
saldo inicial, as entradas e saídas de dinheiro, o saldo final e o responsável
pela movimentação do caixa.

Ator: Gerente, Vendedor

#### RF09 - Manter cliente

Descrição: O sistema deve permitir que os usuários do sistema insiram, atualizem
e consultem as informações dos clientes, incluindo o nome, endereço, telefone,
e-mail. Os usuários devem ser capazes de criar, excluir e modificar os registros
de clientes conforme necessário, além de visualizar um histórico das transações
de cada cliente com o caixa.

Ator: Gerente, Vendedor

#### RF10 - Manter telefone

Descrição: O sistema deve permitir que os usuários insiram, atualizem e
consultem as informações dos telefones relacionados aos clientes, incluindo o
número de telefone, o tipo de telefone, e o cliente associado. Os usuários devem
ser capazes de visualizar todas as informações do telefone de um cliente em uma
única tela, sem a necessidade de navegar por várias telas.

Ator: Gerente, Vendedor

#### RF11 - Manter endereço

Descrição: O sistema deve permitir que informações associadas ao endereço dos
usuários possam ser inseridas, atualizadas, editadas ou excluidas. Isso inclui
campos para inserir o nome da rua, número da residência, complemento, bairro,
cidade, estado e CEP. Os endereços registrados devem ser possíveis de
recuperação.

Ator: Gerente, Vendedor

#### RF12 - Manter fornecedor

Descrição: O sistema controle de caixa deve ser capaz de manter informações
relacionadas aos seus fornecedores, isso inclui o registro de detalhes como
nome, endereço, número de telefone, e endereço de e-mail. Com isso, a
funcionalidade deve possuir a capacidade de casdatrar, atualizar e deletar tais
informações, assim também como deve possibilitar a vizualização das informações
cadastradas.

Ator: Gerente

#### RF13 - Manter pedido

Descrição: O sistema deve ser capaz de armazenar e gerenciar os pedidos
realizados, possuindo a capacidade de inserir, atualizar, exibir os pedidos
realizados, assim com excluir pedidos. As informações relacionadas ao pedido são
quatidade, produto, fornecedor, usuário, data prevista de entrega,
data de realização do pedido. Os campos possuem o intuito de possuir
as informações necessárias para realização do pedido.

Ator: Gerente

#### RF14 - Manter despesa

Descrição: O sistema deve permitir ao usuário cadastrar, visualizar, editar e
excluir despesas. Uma despesa tem nome, valor e se a despesa é periódica.

Ator: Administrador financeiro, Gerente.

#### RF15 - Manter categoria de produto

Descrição: O sistema deve permitir ao usuário cadastrar, visualizar, editar e
excluir categorias de produtos. A categoria possui nome e status.

Ator: Gerente.

#### RF16 - Relatar movimentação

Descrição: O sistema irá calcular o movimento de entrada e saída do caixa em um
intervalo de datas com base nas vendas, reposições de estoque, sálarios pagos
e despesas.

Ator: Gerente

#### RF17 - Relatar estoque baixo

Descrição: O sistema contará com um dashboard de estoque onde serão exibidos os
produtos com estoque baixo

Ator: Gerente

### Requisitos não funcionais

| Código | Descrição                                                              |
| ------ | ---------------------------------------------------------------------- |
| RNF01  | Usuários com menos privilégios de acesso, tem ação limitada no sistema |
| RNF02  | O sistema deve ter boa experiência de uso                              |
| RNF03  | O sistema deve ser responsivo                                          |
| RNF04  | As senhas dos usuários devem ser armazenadas de forma criptografada    |
| RNF05  | O sistema sempre deve ter no mínimo um gerente ativo                   |
| RNF06  | O sistema deve ser acessível pelos navegadores Chrome e Firefox        |

### Riscos

| Data       | Risco                                  | Prioridade | Responsável | Status  | Providência/Solução    |
| ---------- | -------------------------------------- | ---------- | ----------- | ------- | ---------------------- |
| 02/04/2023 | Não aprendizado do framework escolhido | Alta       | Gerente     | Vigente | Reforço de estudos     |
| 02/04/2023 | Inconsistência entre requisitos        | Alta       | Todos       | Vigente | Reunião de alinhamento |
| 02/04/2023 | Má divisão de tarefas                  | Média      | Gerente     | Vigente | Redivisão de tarefas   |
| 02/04/2023 | Atraso de cronograma                   | Baixa      | Gerente     | Vigente | Reoganização de equipe |

## Referências

[Modelo de documento de visão do BSI](https://docs.google.com/document/d/1DPBcyGHgflmz5RDsZQ2X8KVBPoEF5PdAz9BBNFyLa6A/edit)
