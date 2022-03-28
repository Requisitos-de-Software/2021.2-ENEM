# Especificação suplementar

## 1. Introdução
A especificação suplementar é um documento com o objetivo de explicitar os requisitos do aplicativo, tendo em vista os requisitos de usabilidade, confiabilidade, suportatibilidade e desempenho, além de outros requisitos, como: sistemas operacionais e ambientes, requisitos de compatibilidade e restrições de design.

### 1.1 Finalidade
A finalidade é  especificar os requisitos não-funcionais do aplicativo ENEM, descrevendo seu comportamento a partir do modelo de casos de usos e com isso capturando um conjunto completo de requisitos do sistema.

## 2. Escopo
Com o aplicativo Enem, é possível ver notícias sobre o exame, conferir informações de situação da inscrição, ver o cronograma de provas com datas e locais e ter acesso ao cartão de confirmação, trazer o gabarito das provas, o resultado individual após o exame ser realizado e o espelho da redação.

## 3. Requisitos Não-Funcionais

|  ID  |  Requisito  |  Técnica  |   Priorização  |
|------|-------------|-----------|----------------|
| RNF01 |  O aplicativo deve ter compatibilidade com qualquer sistema operacional | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md)  | MUST  |
| RNF02 |  O aplicativo deve recusar o acesso de pessoas não autorizadas | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md)  | MUST  |
| RNF03 |  O aplicativo deve proteger os dados dos usuários | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md)  | MUST  |
| RNF04 |  O aplicativo deve ser acessível para Pessoas com Deficiência (PcD) | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md)  | MUST  |
| RNF05 |  O aplicativo deve consegui suportar uma grande quantidade de acessos simultâneos | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [EF](tecnicas-elicitacao/entrevista.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md), [OF](../elicitacao/tecnicas-elicitacao/observacao.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md)  | MUST  |
| RNF06 |  O aplicativo deve ter baixo tempo de espera mesmo durante períodos de grande fluxo | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [IF](../elicitacao/tecnicas-elicitacao/introspeccao.md)  | MUST  |
| RNF07 |  O aplicativo deve deve ter ter uma interface amigável na qual com no máximo 3 cliques o usuário consiga realizar a ação desejada | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md), [QF](../elicitacao/tecnicas-elicitacao/questionario.md), [SF](../elicitacao/tecnicas-elicitacao/storyboard.md)  | SHOULD |
| RNF08 |  O aplicativo deve deve se adaptar bem a dispositivos mobile | [BF](../elicitacao/tecnicas-elicitacao/brainstorming.md)  | MUST  |
| RNF10 |  O aplicativo deve possuir funcionalidades em modo offline | [SF](../elicitacao/tecnicas-elicitacao/storyboard.md)  | COULD  |

### 3.1 Usabilidade
A interface deve ser intuitiva apresentando o conteúdo e os recursos de uma forma simples, direta e fornecer o mínimo de distração. Sendo assim, o usuário deve consegui realizar a ação desejada com o mínimo de esforço possível.

### 3.2 Confiabilidade

<h4 class="header-light">3.2.1 Disponibilidade</h4>
O serviço tem que está diponível 24/7 tendo que suportar uma grande quantidade de acesso simultâneos de usuários principalmente após a divulgação do local da prova e ao ser liberado a nota das provas.

<h4 class="header-light">3.2.2 Privacidade dos Dados</h4>
O aplicativo tem que seguir a Lei Geral de Proteção de Dados (LGPD).

### 3.3 Desempenho
A aplicação tem que ter um tamanho e um desempenho compativo com dispositivos mais fracos, visto que ENEM é um prova que engloba jovens de diferentes classes sociais.

### 3.4 Suportabilidade
O aplicativo deve ter compatibilidade com qualquer sistema operacional suportando a versão do Android 4.4 ou superior ou a versão do IOS 10.0 ou superior.

### 3.5 Requisito Físico
Os dispositivos deverão ter acesso a internet para acessar o aplicativo.

## 4. Bibliografia
<p>KADER, Saleh; Especificação Suplementar; Disponível em: <https://requisitos-habitica.netlify.com/EspecificacaoSuplementar>. Acesso em: 04/03/2022.</p>
<p>Play Store, Inep - ENEM, Disponível em: <https://play.google.com/store/apps/details?id=br.gov.inep.inepenem&hl=pt_BR&gl=US>. Acesso em: 04/03/2022.</p>
<p>Apple Store, Inep - ENEM, Disponível em: <https://apps.apple.com/br/app/enem-inep/id1114622953>. Acesso em: 04/03/2022.</p>

## 5. Versionamento

| Versão | Data | Modificação | Autor |
|--|--|--|--|
| 1.0 | 04/03/2022 | Criação da página | Pedro Henrique e Vitor Diniz |
| 1.1 | 04/03/2022  | Elaboração do documento | Pedro Henrique e Vitor Diniz |
| 1.2 | 04/03/2022  | Revisando e padronizando índice do documento | Pedro Henrique e Vitor Diniz |
