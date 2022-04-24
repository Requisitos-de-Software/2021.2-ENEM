## 1. Introdução

O NFR Framework é uma abordagem para representar e analisar Requisitos Não-Funcionais.
Seu objetivo é ajudar desenvolvedores na implementação de soluções personalizadas, levando
em consideração as características do domínio e do sistema em questão. Tais características
incluem Requisitos Não-funcionais, Requisitos funcionais, prioridades e carga de
trabalho. Esses fatores determinam a escolha de alternativas de desenvolvimento para um
determinado sistema (CHUNG et al., 2000).

## 2. Softgoals (Objetivos leves)

- Softgoals NFR
- Softgoals de Operacionalização
- Softgoals de Afirmação

## 3. Decomposições

- Decomposição de Softgoal NFR
- Decomposição de Operacionalização
- Decomposição de Afirmação (Claims)
- Priorização

## 4. Legenda

### Softgoals (Objetivos leves)

<img width="500" alt="nfr_guide" src="https://user-images.githubusercontent.com/51385738/157487932-c710441a-78a3-4dbb-ad17-9baf2fa7d2ea.png">
<center>
<figcaption> Figura 01 - Legendas Softgoals (Objetivos leves) </figcaption>
</center>

### Interdependecy (Interdependência)

<img width="500" alt="nfr_line_guide" src="https://user-images.githubusercontent.com/51385738/157487958-0f254ac9-1b3a-4ba8-b591-651f8ce27f60.png">
<center>
<figcaption> Figura 02 - Legendas Interdependecy (Interdependência) </a></figcaption>
</center>

## 5. Requisitos não funcionais

| ID    | Requisito                                                                                                                        | Técnica                                                                                                                                                                                                                                                                                  | Priorização |
| ----- | -------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| RNF01 | O aplicativo deve ter compatibilidade com qualquer sistema operacional                                                           | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md)                                                                                                                                                                        | MUST        |
| RNF02 | O aplicativo deve recusar o acesso de pessoas não autorizadas                                                                    | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md)                                                                                                                                                                        | MUST        |
| RNF03 | O aplicativo deve proteger os dados dos usuários                                                                                 | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md)                                                                                                               | MUST        |
| RNF04 | O aplicativo deve ser acessível para Pessoas com Deficiência (PcD)                                                               | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md)                                                                                                               | MUST        |
| RNF05 | O aplicativo deve consegui suportar uma grande quantidade de acessos simultâneos                                                 | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [EF](../elicitacao/tecnicas-elicitacao/entrevista.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md), [OF](../elicitacao/tecnicas-elicitacao/observacao.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md) | MUST        |
| RNF06 | O aplicativo deve ter baixo tempo de espera mesmo durante períodos de grande fluxo                                               | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md)                                                                                                                                                                        | MUST        |
| RNF07 | O aplicativo deve deve ter ter uma interface amigável na qual com no máximo 3 cliques o usuário consiga realizar a ação desejada | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md), [SF](../elicitacao/tecnicas-elicitacao/storyboard.md)                                                                                                                 | SHOULD      |
| RNF08 | O aplicativo deve deve se adaptar bem a dispositivos mobile                                                                      | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md)                                                                                                                                                                                                                                 | MUST        |
| RNF10 | O aplicativo deve possuir funcionalidades em modo offline                                                                        | [SF](../elicitacao/tecnicas-elicitacao/storyboard.md)                                                                                                                                                                                                                                    | COULD       |

## 6. Diagrama

### 6.1 Diagrama Geral sem propagação

![NFR_semPropagacao](https://user-images.githubusercontent.com/53023400/157520738-48cdb14e-9fb7-4a80-9fd5-e288c546089a.jpg)

<center>
<figcaption> Figura 03 - NFR Framework Geral sem propagação </figcaption>
</center>
<center>
<figcaption> <strong>Autor: </strong>Eduardo Gurgel e Jackes Fonseca</figcaption>
</center>

### 6.2 Diagrama Geral com propagação

![NFR_comPropagacao](https://user-images.githubusercontent.com/53023400/157521127-c901b744-d8e8-4aa7-8c8b-1d4d34d0a1e3.jpg)

<center>
<figcaption> Figura 04 - NFR Framework Geral com propagação </figcaption>
</center>
<center>
<figcaption> <strong>Autor: </strong>Eduardo Gurgel e Jackes Fonseca</figcaption>
</center>

## 7. Bibliografia

[1] CHUNG, L.; NIXON, B. A.; YU, E.; MYLOPOULOS, J. Non-functional requirements in software engineering. Springer Science & Business Media: [s.n.], 2000. v. 5. Disponível aqui. Acessado em 09/03/22.

[2] DA SILVA, Reinaldo Antônio. NFR4ES: Um Catálogo de Requisitos Não-Funcionais para Sistemas Embarcados. 2019. Dissertação (Mestrado em Ciência da Computação) - Universidade Federal de Pernambuco, Recife, 2019.

## 8. Histórico de versão

| Versão | Data  |             Descrição              |             Autor              |
| :----: | :---: | :--------------------------------: | :----------------------------: |
|  1.0   | 09/03 |        Criação do documento        |         Eduardo Gurgel         |
|  2.0   | 09/03 | Adição do documento de usabilidade | Eduardo Gurgel, Jackes Fonseca |
