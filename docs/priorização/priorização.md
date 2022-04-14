# <center> First Things First

## Histórico de versão
| Data | Versão | Autor | Descrição |
| :-: | :-: | :-: | :-: |
| 12/04/2022 | 0.1 | Eduardo Gurgel | Criação do documento |
| 13/04/2022 | 0.2 | Eduardo Gurgel | Inserir tabela |
| 14/04/2022 | 0.3 | Eduardo Gurgel | Finalização dos detalhes |

<div align="justify">

## 1. Introdução
"First Things First" é uma técnica que tem como objetivo priorizar em relação à implementação de certas funcionalidades, considerando fatores que impactam na disponibilização delas aos usuários da aplicação.

## 2. Metologia
É construída uma tabela de forma que pondere os posionamentos do cliente e do desenvolvedor. Para isso, devem ser seguidos em oito etapas:

- Etapa 1: Listar todos os requisitos em uma tabela, retirando aqueles dependentes de outro requisito.

- Etapa 2: Estimar o _Benefício Relativo_ que cada recurso fornece ao cliente ou ao negócio, de 1 a 9, em que 1 é o menos significativo e 9 o mais significativo.

- Etapa 3: Estimar a _Penalidade Relativa_ que o negócio sofreria, se o recurso não fosse incluído, de 1 a 9, em que 1 é o com menor penalidade e 9 maior penalidade.

- Etapa 4: A coluna _Valor Total_ é a soma do (_Benefício Relativo_ * _Peso Relativo_ + _Penalidade Relativa_ * _Peso Relativo_).

- Etapa 5: Estimar o _Custo Relativo_ de implementação de cada requisito, de 1 a 9.

- Etapa 6: Estimar o _Risco Relativo_ ao risco a cada requisito de uma escala de 1 a 9.

- Etapa 7: Calcular a _Prioridade_ para cada requisito pela fórmula: _Valor %_ / (_Custo %_ * _Peso Custo_ + _Risco %_ * _Peso Risco_). 

- Etapa 8: Ordenar a lista em ordem decrescente de prioridade.


## 3. Tabela de Referência - Requisitos Funcionais e Não Funcionais
| ID | Requisito | Técnica Utilizada |
| :-: | :- | :- |
| RF01 | O usuário deve ser capaz de fazer o login através do gov.br | [Representação](../modelagem/nfrframework.md) |
| RF02 | O usuário deve ser capaz de visualizar o cronograma da prova | [Representação](../modelagem/nfrframework.md) |
| RF03 | O usuário deve ser capaz de acompanhar sua inscrição | [Representação](../modelagem/nfrframework.md) |
| RF04 | O usuário deve ser capaz de acompanhar pedido de isenção de taxa de inscrição | [Representação](../modelagem/nfrframework.md) |
| RF05 | O usuário deve ser capaz de ter acesso aos avisos e às notícias | Agregação (RF02, RF04, RF06, RF14) |
| RF06 | O usuário deve ser capaz de verificar as perguntas frequentes e as orientações | [Representação](../modelagem/nfrframework.md) |
| RF07 | O usuário deve ser capaz de visualizar/baixar/imprimir sua nota de provas do Enem | [Representação](../modelagem/nfrframework.md) |
| RF08 | O usuário deve ser capaz de visualizar/baixar/imprimir sua vista pedagógica das provas do Enem | [Representação](../modelagem/nfrframework.md) |
| RF09 | O usuário deve ser capaz de visualizar/baixar/imprimir sua redação das provas do Enem | [Representação](../modelagem/nfrframework.md) |
| RF10 | O usuário deve ser capaz de visualizar/baixar/imprimir seu gabarito das provas do Enem | [Representação](../modelagem/nfrframework.md) |
| RF11 | O usuário deve ser capaz de visualizar/baixar/imprimir as provas do Enem | [Representação](../modelagem/nfrframework.md) |
| RF12 | O usuário deve ser capaz de visualizar/baixar/imprimir simulados do Enem | [Representação](../modelagem/nfrframework.md) |
| RF13 | O usuário deve ser capaz de visualizar métricas de desempenho dos participantes | Agregação (RF07, RF08, RF11) |
| RF14 | O usuário deve ser capaz de consultar escopo de conteúdo do exame | Agregação (RF12) |
| RN01 | O aplicativo deve ter compatibilidade com qualquer sistema operacional | [Representação](../modelagem/nfrframework.md) |
| RN02 | O aplicativo deve recusar o acesso de pessoas não autorizadas | [Representação](../modelagem/nfrframework.md) |
| RN03 | O aplicativo deve proteger os dados dos usuários | [Representação](../modelagem/nfrframework.md) |
| RN04 | O aplicativo deve ser acessível para Pessoas com Deficiência (PcD) | [Representação](../modelagem/nfrframework.md) |
| RN05 | O aplicativo deve consegui suportar uma grande quantidade de acessos simultâneos | [Representação](../modelagem/nfrframework.md) |
| RN06 | O aplicativo deve ter baixo tempo de espera mesmo durante períodos de grande fluxo | [Representação](../modelagem/nfrframework.md) |
| RN07 | O aplicativo deve deve ter ter uma interface amigável na qual com no máximo 3 cliques o usuário consiga realizar a ação desejada | [Representação](../modelagem/nfrframework.md) |
| RN08 | O aplicativo deve deve se adaptar bem a dispositivos mobile | [Representação](../modelagem/nfrframework.md) |
| RN09 | O aplicativo deve possuir funcionalidades em modo offline | [Representação](../modelagem/nfrframework.md) |

## 4. Priorização First Things First
| Funcionalidade | Benefício relativo | Penalidade | Valor Total | Valor % | Custo Relativo | Custo % | Risco relativo | Risco % | Prioridade |
| -------------- | ------------------ | ---------- | ----------- | ------- | -------------- | ------- | -------------- | ------- | ---------- |
| RF14 |9|7|16|8,0808|7|7,4468|4|4,1237|0,6983|
| RF02 |8|8|16|8,0808|5|5,3191|7|7,2164|0,6446|
| RF03 |9|9|18|9,0909|7|7,4468|7|7,2164|0,6199|
| RF09 |9|7|16|8,0808|7|7,4468|7|7,2165|0,5510|
| RF10 |8|7|15|7,5757|7|7,4468|7|7,2165|0,5166|
| RF11 |8|7|15|7,5757|7|7,4468|7|7,2165|0,5166|
| RF08 |8|7|15|7,5757|7|7,4468|7|7,2165|0,5166|
| RF01 |9|9|18|9,0909|8|8,5106|9|9,2784|0,5110|
| RF06 |6|4|10|5,0505|5|5,3191|5|5,1546|0,4822|
| RF07|7|7|14|7,0707|7|7,4468|7|7,2165|0,4822|
| RF12 |7|7|14|7,0707|7|7,4468|7|7,216|0,4822|
| RF04 |7|5|12|6,0606|6|6,3829|8|8,2474|0,4142|
| RF05 |7|2|9|4,5454|6|6,3829|6|6,1856|0,3616|
| RF13 |7|3|10|5,0505|8|8,5106|9|9,2784|0,2839|
| Total |109|89|198|100|94|100|97|100|7,0814|

## 5. Referências
First Things First: Prioritizing Requirements. E.Wiegers, Karl. Disponível em: https://www.processimpact.com/articles/prioritizing.pdf. Acesso em 17 de agosto de 2021.
