<img src='/img/logo.png' alt='logo da empresa' width='50px' heidth='50px'/>

# *IF posting*

# PROJETO DE SOFTWARE

## *Stakeholders*
|NOME|CARGO|E-MAIL|
|:Max costa cardoso|:Programador|: cardoso.max@estudante.ifro.edu.br|
|:Sebastião Regino Cezario Neto|:Programador|:sebasskins@hotmail.com|

# Sumário

* [RESUMO DO PROJETO](#resumo-do-projeto)
* [INTRODUÇÃO](#introdução)
  * [PROPÓSITO DESTE DOCUMENTO](#propósito-deste-documento)
  * [ESCOPO DO PROJETO](#escopo-do-projeto)
  * [CONCEPÇÃO DO SISTEMA](#concepção-do-sistema)
  * [CONVENÇÕES, TERMOS E ABRIVEAÇÕES](#convenções-termos-e-abreviações)
* [DESCRIÇÃO GERAL](#descrição-geral)
  * [USUÁRIOS DO SISTEMA](#usuários-do-sistema)
  * [ABRANGÊNCIA E SISTEMAS SIMILARES](#abrangência-e-sistemas-similares)
  * [SUPOSIÇÕES E DEPENDÊNCIAS](#suposições-e-dependências)
* [ESTUDO DE VIABILIDADE](#estudo-de-viabilidade)
  * [VIABILIDADE TÉCNICA](#viabilidade-técnica)
  * [VIABILIDADE ECONÔMICA](#viabilidade-econômica)
  * [VIABILIDADE ORGANIZACIONAL](#viabilidade-organizacional)
* [METODOLOGIA ADOTADA NO DESENVOLVIMENTO](#metodologia-adotada-no-desenvolvimento)
* [REQUISITOS DO SOFTWARE](#requisitos-do-software)
  * [REQUISITOS FUNCIONAIS](#requisitos-funcionais)
  * [REQUISITOS NÃO FUNCIONAIS](#requisitos-não-funcionais)
* [PROTOTIPAGEM](#prototipagem)
* [DIAGRAMA DE CASOS DE USO](#diagrama-de-casos-de-uso)
  * [ESPECIFICAÇÃO DOS CASOS DE USO](#descrição--especificação-dos-casos-de-uso)
* [DIAGRAMA DE CLASSES](#diagrama-de-classes)
* [DIAGRAMA DE SEQUÊNCIAS](#diagrama-de-sequências)
* [ DIAGRAMA DE ATIVIDADES](#diagrama-de-atividades)
* [REFERÊNCIAS](#referências)


# RESUMO DO PROJETO
| ITEM | DESCRIÇÃO|
|:---|:---|
| NOME DO PROJETO | IF posting|
| GERENTE DO PROJETO | Rafaela Soares Pereira|
| PRINCIPAL OBJETIVO | Auxiliar o desempenho academico e comunicativo de alunos, ex-alunos e futuros alunos dos IF's. |
| BENEFÍCIOS ESPERADOS |* Melhor acompanhamento pedagógico;<br/>* Redução da evasão escolar;<br/>* Aumento do número de matrículas;<br/>* Redução da inadimplência escolar;<br/>* Melhor comunicação de alunos ao redor do Brasil.|
| INÍCIO E TÉRMINO PREVISTOS | 14/03/2023 - 07/12/2023 |

[ [INÍCIO](#IF posting) ]

# INTRODUÇÃO

## PROPÓSITO DESTE DOCUMENTO

Este documento destina-se aos clientes, engenheiros, gerentes e demais stakeholders deste projeto. O propósito deste documento é apresentar a descrição dos serviços e funções que o sistema **_IF posting_** deve prover, bem como as suas restrições de operação e propriedades gerais, a fim de ilustrar uma descrição detalhada do sistema para um auxílio durante as etapas de análise, projeto e testes. O documento especifica todos os requisitos funcionais e não funcionais do sistema e contém a prototipagem, além de diagramas UML que foram construídos levando-se em conta as funcionalidades identificadas durante a fase de concepção do sistema.

## CONCEPÇÃO DO SISTEMA

Foram usados três métodos para que pudessem ser obtidos os requisitos do sistema:
  * Discussões individuais de um representante da equipe com Wagner Ferreira, Professor de fundamentos.


## CONVENÇÕES, TERMOS E ABREVIAÇÕES

Para evitar interpretações incorretas deste documento, algumas convenções e termos específicos. Tentamos ultilizar uma linguagem de facil compreensão

[ [INÍCIO](#fibonacci-management-system) ]

# DESCRIÇÃO GERAL

## ESCOPO DO PROJETO

### NO ESCOPO

O projeto consiste na construção de uma ferramenta para gerenciamento de aprendizado *(Learning Management System - LMS)*, que possa atender os alunos dos IF's em geral. O projeto visa auxiliar o sistema de ensino através de ferramentas síncronas e assíncronas que serão usadas por alunos, ex-alunos e futuros alunos da instituição de ensino.
O escopo do **produto** pode ser consultado nos [requisitos do software](#requisitos-do-software)

### FORA DO ESCOPO

Não fazem parte do escopo do projeto:
* Instalação e configuração do ambiente tecnológico do cliente;
* Treinamento de instalação, configuração, administração e  utilização do sistema;
* Integração com quaisquer sistemas ou base de dados do ambiente tecnológico do cliente.

## Usuários do sistema
|USUÁRIO|DESCRIÇÃO|
|:---|:---|
|**Usuário Padrão:**|Realizam as tarefas comuns a todos os usuários, tal como: logar e enviar mensagens. Todos demais usuários estendem as funcionalidades do UsuárioPadrão|
|**Administrador:**|Responsáveis pelo gerenciamento das entidades pertinentes à instituição e pela alocação de outros administradores|

## Abrangência e sistemas similares

### Abrangência:

O sistema terá ferramentas para a construção de uma comunidade acadêmica amigável e unida, na qual todos terão espaço para expressar opiniões, compartilhar interesses, relatar experiências cotidianas e, o mais importante, familiarizar-se com os Institutos Federais (IFs).

### Sistemas similares:

No cenário atual da universidade se encontra um sistema que é responsável por realizar tal tarefa, denominado Virtus, porém o sistema não atende todas as necessidades, não sendo considerado satisfatório pela maioria dos usuários.

No cenário nacional encontram-se quatro sistemas que se destacam:

**Sistema Acadêmico Integrado (SAI)**: É uma plataforma adotada por diversas instituições de ensino superior no Brasil, que oferece ferramentas de interação e comunicação entre estudantes, professores e funcionários. O SAI permite o compartilhamento de informações acadêmicas, notícias, eventos e fóruns de discussão.

**Rede Acadêmica Federada (RNP)**:bÉ uma infraestrutura nacional que interliga instituições de pesquisa e educação, possibilitando a colaboração e o compartilhamento de recursos. Além disso, a RNP oferece serviços de comunicação e colaboração entre os membros da rede, promovendo a troca de informações e o fortalecimento da comunidade acadêmica.

**Ambiente Virtual de Aprendizagem (AVA)**: Esses sistemas são adotados por várias instituições de ensino para oferecer suporte às atividades de ensino e aprendizagem online. Eles fornecem espaços para postagem de conteúdos, interação entre estudantes e professores, fóruns de discussão, entrega de tarefas, entre outras funcionalidades.

**Plataforma de Gestão Educacional**: São sistemas abrangentes que englobam não apenas a interação entre os membros da comunidade acadêmica, mas também a gestão administrativa e pedagógica da instituição. Essas plataformas oferecem recursos para comunicação, gerenciamento de turmas, controle de notas, agendamento de aulas, entre outros aspectos relacionados à vida acadêmica.

No cenário internacional os sistemas de maior porte são:

**Edmodo**: Uma plataforma educacional global que conecta estudantes, professores e pais, oferecendo recursos para colaboração, compartilhamento de recursos e interação.

**Moodle**: Um sistema de gerenciamento de aprendizado de código aberto que permite a criação de comunidades de aprendizado online. Oferece ferramentas para discussões, compartilhamento de arquivos, avaliações e interações entre os participantes.

**Canvas** Uma plataforma de aprendizado online amplamente utilizada em instituições educacionais em todo o mundo. Ela permite a criação de comunidades de aprendizado virtuais, oferecendo recursos para comunicação, colaboração e compartilhamento de conteúdo.

**Blackboard** Outra plataforma popular de aprendizado online que possibilita a criação de comunidades acadêmicas interativas. Oferece recursos como fóruns de discussão, blogs, mensagens instantâneas e compartilhamento de materiais didáticos.

Essas plataformas internacionais se assemelham ao "IF Posting" no sentido de proporcionar uma experiência colaborativa e interativa para os membros da comunidade acadêmica, permitindo a expressão de opiniões, compartilhamento de informações e interações significativas.
Os usuários devem utilizar um computador com a seguinte configuração mínima:

* Processador Dual Core 2GHz ou superior
* 2Gb de memória RAM
* acesso a internet

Os usuários devem utilizar um celular com a seguinte configuração mínima:
*Android 7.0


# ESTUDO DE VIABILIDADE

Uma vez definidos a necessidade para o sistema e seus requisitos de negócio, é possível compreender melhor o projeto do sistema proposto para elaborar o estudo de viabilidade com os seguintes destaques:

## Viabilidade Técnica
Os colaboradores da empresa contratante possuem bastante experiência com aplicações desta natureza, os analistas também estão familiarizados com esta área de aplicação comercial, porém o sistema utiliza uma tecnologia nova, com a qual os analistas e programadores não estão familiarizados. No que se refere ao tamanho do sistema, trata-se de um projeto de médio porte, com baixo nível de complexidade, que não será integrado a outros sistemas, limitando-se a atender a demanda da escola no que se refere à EaD, que, atualmente possui 1.000 alunos matriculados. Conclui-se que o projeto possui viabilidade técnica, em virtude dos baixos riscos identificados.

## Viabilidade Econômica

Foi realizada uma análise de custo-benefício, e, mesmo com estimativas conservadoras do retorno sobre o investimento e dos benefícios totais, este projeto é viável economicamente. Após a implantação, espera-se uma melhoria na qualidade dos serviços prestados e aumento da capacidade de vagas da unidade escolar.

## Viabilidade Organizacional

Do ponto de vista organizacional, este projeto apresenta baixo risco. Os diretores e coordenadores da instituição demonstram forte interesse no projeto. Espera-se que os professores e alunos aprovem a implantação do sistema, visto que atualmente a escola não possui uma ferramenta específica para o controle das informações, o que está provocando enormes transtornos para a instituição.


[ [INÍCIO](#fibonacci-management-system) ]

# Metodologia Adotada no Desenvolvimento


[ [INÍCIO](#fibonacci-management-system) ]

# Requisitos do Software

A especificação dos requisitos deste documento deve seguir as recomendações da norma IEEE Std-830-1998, levando em conta as recomentações do documento de [características dos requisitos](caracteristicas_requisitos.md).

## Requisitos Funcionais

A tabela a seguir contém a relação dos Requisitos Funcionais elicitados, com as colunas: identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
:---|:---|:---|
|RF-001|Fazer Login|Página separada dedicada a criação do login|
|RF-002|Fazer cadastro|Página dedicada a criação de conta|
|RF-003|Trocar senha|Página dedicada a troca de senha caso o usuário esqueça|
|RF-004|Adicionar postagem|Componente para adcionar pstagem|
|RF-005|Alternar entre câmera e a galeria do dispositivo|Subfunção dedicada a escolha do usuário entre fazer uma postagem cm a câmera do dispositivo ou a galeria|
|RF-006|Adcionar postagem de texto|Componente dedicado a escolha do usuário em fazer uma postagem de texto|
|RF-007|Alterar foto de perfil|Componente dedicado a alterar a foto de perfil|
|RF-008|Alterar nome|Componente para mudar o nome do perfil|
|RF-009|Adcionar amigos|Componente focado em adcionar amigos|
|RF-010|Conversar com amigos|Chat de conversa|
|RF-011|Fazer comentários de postagem|Componente focado em adcionar comentários|
|RF-012|Observar notícias dos outros campus|Componente que ficará no canto direito da tela mostrando as principais notícias dos outros campus|
|RF-013|Observar postagens de outros alunos|Comoponente que ficará na maior parte da página, mostrando as postagens dos alunos|
|RF-013|Botões mobile|Conjunto de botões e funções disponíveis apenas para mobile|
|RF-014|Definir preferências de postagens|Página focada em criar filtros para o tipo de conteúdo que o usuário gostaria de consumir|
|RF-015|Bloquear usuários|Componente para bloquear usuários e/ou amigos que o usuário não gostaria de receber postagens ou conversas|
|RF-016|Notificar usuário|Componente para notificações de postagens de usuários aos quais o usuário esteja seguindo|
|RF-017|Seguir usuário e/ou campus|Componente para seguir outros usuários ou campus|
|RF-018|Denunciar abuso|Botão para denunciar abusos ocorridos em conversas, ou postagens|
|RF-019|Tornar conta privada|Botão para tornar sua conta privada|
|RF-020|Tornar conta fantasma|Botão para tornar sua conta como conta fantasma|


## Requisitos Não Funcionais
A tabela a seguir contém a relação com os Requisitos Não Funcionais identificados, contendo identificador, nome, descrição e prioridade:

| IDENTIFICADOR | NOME | DESCRIÇÃO |
|:---|:---|:---|
|RNF-001|Desepenho|especificações relacionadas ao tempo de resposta, capacidade de processamento, uso de recursos (memória, armazenamento) e escalabilidade do sistema.|
|RNF-002|Usabilidade|requisitos relacionados à facilidade de uso, interface do usuário, experiência do usuário, acessibilidade e documentação.|
|RNF-003|Segurança|requisitos relacionados à proteção de dados, autenticação, autorização, criptografia e controle de acesso.|
|RNF-004|Confiabilidade|especificações relacionadas à disponibilidade do sistema, tolerância a falhas, recuperação de erros e manutenção.|
|RNF-005|Compatibilidade|requisitos relacionados à interoperabilidade do sistema com outras plataformas, sistemas operacionais, navegadores, dispositivos, etc.|
|RNF-006|Manutenibilidade|requisitos relacionados à facilidade de manutenção, extensibilidade, modularidade e documentação do código.|
|RNF-007|Legal e regulamentar|requisitos relacionados a conformidade com leis, regulamentos e padrões governamentais.|
|RNF-008|Escalabilidade|O sistema deve ser capaz de lidar com um aumento significativo no número de usuários, postagens e interações, mantendo um desempenho adequado e uma experiência do usuário satisfatória. Isso significa que o sistema deve ser dimensionável e capaz de lidar com o crescimento do volume de dados e do tráfego de usuários.|
|RNF-009|Acessibilidade|O sistema deve ser projetado e desenvolvido levando em consideração a acessibilidade para pessoas com deficiências, garantindo que todos os usuários possam utilizar as funcionalidades oferecidas. Isso inclui recursos como suporte a leitores de tela, teclado para navegação, contraste adequado nas cores, entre outros aspectos que tornam o sistema acessível a todos os usuários.
|RNF-010|Responsividade|O sistema deve ser responsivo, podendo ser acessado por usuários tanto do computador, quanto do celular e/ou demais dispositivos|



[ [INÍCIO](#fibonacci-management-system) ]


# Prototipagem

[Protótipo criado no FIGMA em 2022 por estudantes](https://www.figma.com/file/abDzdHjydjCid03IBaRrx5/Prot%C3%B3tipo?type=design&node-id=0-1&t=tyBiLb4EgdhlQyjr-0)

![Imagem do Protótipo](/img/home.png)

[ [INÍCIO](#fibonacci-management-system) ]


# Diagrama de Casos de Uso


![Diagrama de Casos de Uso](/img/UseCase Diagram1.png)

## Descrição / Especificação dos Casos de Uso

### UC-01 - Cadastrar Novo Usuario

|UC-01 - Cadastrar Usuario|           
|:---|
|**Descrição/Objetivo:** Permite a inclusão de novos usuarios no Sistema|
|**Atores: Administrador**|
|**Pré-condições:** O usuário precisa estar cadastrado e logado|
|**Pós-condições:** Será apresentada uma mensagem confirmando a realização do cadastro|
|**FLUXO PRINCIPAL / BÁSICO:**|
|1. O usuário seleciona a opção cadastrar professor|
|2. Os dados do usuario são inseridos|
|3. O usuário clica em salvar|
|4. Um novo ID é gerado |
|5. É apresentada uma mensagem confirmando a realização do cadastro|
|**FLUXOS ALTERNATIVOS / EXCESSÕES:** |
|**A1: Campo obrigatório não preenchido** |
|1. Uma mensagem será apresentada para o usuário, informando que existe(m) campos obrigatórios que não foram preenchidos |
|2. O cursor será posicionado no primeiro campo obrigatório que não foi preenchido |
|**A2: Data de nascimento inválida** |
|1. Uma mensagem será apresentada para o usuário, informando que a data informáda não é válida|
|2. O cursor será posicionado para o campo data|


## Matriz de Rastreabilidade


| REQUISITO |UC-01|UC-02|UC-03|UC-04|UC-05|UC-06|UC-07|UC-08|UC-09| UC-10|     
|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|:---|
|RF-001|X| | | | | | | | | |
|RF-002| |X| |X| | | | | | |

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Classes

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Sequências

[ [INÍCIO](#fibonacci-management-system) ]

# Diagrama de Atividades



# REFERÊNCIAS

Esta subseção apresenta as referências aos documentos que utilizamos no auxílio à construção deste documento.
* [UML](https://www.omg.org/spec/UML/2.5/About-UML/)
* [Práticas para Especificação de Requisitos IEEE-830](https://ieeexplore.ieee.org/document/720574)
