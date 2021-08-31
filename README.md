# entity-relationship-diagrams

## Exercícios de Modelagem – Prática 1

### Instruções:
- Realizar o Modelo Conceitual (Relacionamentos e atributos (cardinalidades mínimas e máximas).
- Postar as imagens de cada estudo de caso até 01/09/2021
- Pode ser realizado em grupo de até 3 alunos.

## Estudo de Caso 1 – Controle de frequência de empregados 
Deseja-se projetar a base de dados de um sistema de controle de frequência de empregados de uma organização. Através de um diagrama entidade-relacionamento, deve ser modelada esta base de dados.

A base de dados não deve conter redundância de dados. O modelo ER deve ser representado com a notação vista em aula. O modelo deve apresentar, ao menos, entidades, relacionamentos, atributos, especializações, identificadores e grau de cardinalidade mínima e máxima. Não utilizar atributos multi-valorados.

A base de dados deve manter dados sobre empregados. Cada empregado é identificado por um código e tem um nome. Para fins de controle de frequência, há dois tipos de empregados. Um tipo de empregado é o que tem horário livre. Empregados deste tipo podem trabalhar em qualquer horário do dia. Para estes empregados basta saber quantas horas devem trabalhar ao longo do mês, bem como, qual é o menor período em horas que devem trabalhar. Exemplificando, há alguns empregados que não devem trabalhar menos que duas horas cada vez.

Empregados de segundo tipo devem trabalhar em horários fixos. A semana de trabalho do empregado deste tipo está organizada em turnos. Um turno (1) inicia em um dia da semana e um horário e (2) termina em um dia da semana (possivelmente diferente do de início) e em um horário. O empregado pode trabalhar dois turnos no mesmo dia da semana. Cada dia da semana é identificado por um código (algo como "d", "s", . . . ) e tem um nome (algo como "domingo", "segunda-feira", . . . ). (Adaptado - Heuser, 2008).

## Estudo de Caso 2 – Estudo de Caso: Controle de Cinemas

Após várias reuniões com os futuros usuários do sistema, relacionamos uma série de regras do negócio e que serão a base para o desenvolvimento do diagrama ER:

- A empresa de distribuição possui vários cinemas em diversas localidades;
- Cada cinema possui uma identificação única, um nome fantasia, um endereço completo, incluindo rua, avenida, bairro, município, estado e sua capacitação de lotação;
- Os filmes podem ser dos mais variados gêneros e nacionalidade;
- Cada filme é registrado com um título original, e se for filme estrangeiro, possuirá também o título em português, o gênero, sua duração e seu país de origem, informações sobre os atores que compõem seu elenco, e o seu diretor. Existirá um único diretor para cada filme;
- Alguns cinemas apresentam mais de um filme em cartaz, sendo, nesses casos, sessões alternadas com um filme e outro;
- As sessões possuem horários que variam de acordo com a duração do filme, havendo sempre um intervalo de aproximadamente 15 minutos entre elas;
- Os atores de um filme podem, obviamente, atuar em diversos filmes, assim como o diretor de um filme pode também ser ator nesse filme ou, ainda mais, ser ator em outro filme. Um ator possui as seguintes características: um número de identificação, um nome, uma nacionalidade e uma idade;
- As sessões de cinema devem ter seu público registrado diariamente, para que se permita a totalização dos assistentes quando o filme sair de cartaz, ou qualquer instante.
Nas reuniões de levantamento, os usuários nos passaram as seguintes necessidades de informação:
- Apuração do publico por município, por cinema e por sessão de cada cinema;
- Permitir uma forma de consulta, que dado um determinado ator, sejam localizados os cinemas onde estão em cartaz os filmes em que esse ator atua;
- Em quais cinemas está sendo exibido um determinado gênero de filme;
- Em quais cinemas estão sendo exibidos filmes nacionais.


## Estudo de Caso 3 – Biblioteca Municipal de Literolândia 

A comissao municipal de cultura da cidade de Literolândia, uma cidade de 40.000 habitantes no interior de Sao Paulo, se reuniu para discutir alguns assuntos relacionados a cultura na cidade. Nessa reuniao foram levantados alguns problemas nas rotinas da biblioteca municipal, e foi entao votado por unanimidade pela informatizagao do cadastro de acervo da biblioteca e dos processos de aquisigao e emprestimos. A biblioteca conta hoje com um acervo de 30.000 itens, classificados em: Livros, Revistas, Fitas de video, Hemeroteca, etc., cada item do acervo possui um nOmero variavel de cópias, nem todas as cópias estao disponiveis para emprestimo pois, existem exemplares raros que so podem ser consultados na biblioteca. Os livros do acervo podem ter um ou mais autores sendo que somente um autor é considerado como o autor principal, os outros sac) co-autores. Qualquer cidadão Literolandense pode usar a biblioteca para consulta, porem para retirar livros ele deve ser cadastrado como usuario da biblioteca, o cadastro consiste em preencher uma ficha com seus dados pessoais (nome, data de nascimento, local de nascimento, enderego, bairro, telefone, profissao e escolaridade), e fornecer um comprovante de enderego e uma foto 3X4 para a confecgao da uma carteira de identificagao de usuario. Os emprestimos de itens do acervo sac) registrados em um livro de emprestimos que contem o nome do usuario, o item emprestado, a cópia que foi emprestada (identificada pelo número de tombo que é único para cada cópia), a data de saida, a data de devolução, quando o usuario devolve o item sao registrados no mesmo livro, os dias de atraso e o valor da multa, caso ele entregue com atraso. Nao existem limites de empréstimos em aberto por usuário, mas o prazo para devolução é de 7 dias. Se o usuário devolver é cobrada uma taxa diaria de multa por dia de atraso. Para melhorar a busca ao acervo os usuarios devem ter a possibilidade de busca ao cadastro por: Título do item do acervo, autor ou assunto. Para ajudar o trabalho das bibliotecárias deve ser emitido um relatorio diario com os empréstimos em atraso. Como analise estatística do use da biblioteca devem ser emitidos relatOrios com o total de empréstimos no mês por tipo de item do acervo, por item do acervo e por faixa etaria de idade de usuário.
