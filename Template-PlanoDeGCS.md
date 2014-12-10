<SCV - Sistema de Controle de Veículos>
=================
Plano de Gerenciamento de Configuração
======================================
Versão &lt;1.1&gt;
------------------

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|&lt;09/12/2014&gt;|&lt;1.0&gt;|&lt;Versão inicial - Definição do Plano GCS&gt;|&lt;Nelson Rodrigues&gt;|
|&lt;10/12/2014&gt;|&lt;1.1&gt;|&lt;Versão para Homologação&gt;|&lt;Nilderlan Fernandes Pereira&gt;|



1. Introdução
==============

O Plano de Gerenciamento de Configuração descreve todas as atividades do Gerenciamento de Controle de Configuração e Mudança que serão executadas durante o ciclo de vida do produto. Suas atividades envolvem identificar a configuração do software, manter sua integridade durante o projeto e controlar sistematicamente as mudanças.

1.1 Finalidade
---------------
Sua finalidade é criar um padrão a ser seguido por todos os membros da equipe para garantir o maior controle do produto no andamento do projeto.

1.2 Escopo
----------
Este Plano de Gerenciamento de Configuração destina-se a todos os membros da equipe responsáveis pelo desenvolvimento do sistema SCV e tem abrangência em todo o controle e gerenciamento da configuração do projeto.

1.3 Definições, Acrônimos e Abreviações
---------------------------------------
GC - Gerência de Configuração.
CCM - Comitê para o Controle de Mudanças.
GV - Gerência de Veículos
Baseline - Conjunto de itens de configuração que conseguiram um estado comprovado de estabilidade.
PGC - Plano de Gerência de Configuração.

1.4 Referências
---------------
- Template de Plano de Gerência de Configuração, Template-PlanoDeGCS.md
- CMMI for Development, Version 1.3

1.5 Visão Geral
---------------

&lt;Seção 2&gt; - São relacionados os papéis, as responsabilidades das atividades e as ferramentas dentro da GC. -
&lt;Seção 3&gt; - Descreve as identificações configuração, métodos, itens de configuração, baselines, estrutura do repositório e controle de mudanças. -
&lt;Seção 4&gt; - Descreve os padrões e procedimentos que deverão ser adotados e seguidos pela equipe. -
&lt;Seção 5&gt; - Descreve as ferramentas de software, o pessoal e o treinamento necessários para implementar as atividades de CM especificadas. -
&lt;Seção 6&gt; - Descreve as auditorias de configuração, os problemas encontrados e acompanhamento das correções.-

2. Gerenciamento de Configuração de Software
============================================

2.1 Organização, Responsabilidades e Interfaces
------------------------------------------------

|Papéis |Equipe |Responsabilidades|
|-------|-------|-----------------|
|Gerente de Configuração|Nelson Rodrigues|Estabelecer Politicas de GC / Escrever Plano de GC / Configurar Ambiente de GC / Criar Espaços de Trabalho de Integração / Criar Baselines / Promover Baselines |
|CCM|Nelson Rodrigues / Nilderlan Fernandes|Estabelecer Processo de Controle de Mudanças / Revisar Solicitação de Mudança|
|Desenvolvedor|Nelson Rodrigues / Nilderlan Fernandes|Segui os padrões e procedimentos definidos no PGC|

 
 
2.2 Ferramentas, Ambiente e Infra-estrutura
-------------------------------------------

GIT - Controle de Versão - Sistema de controle de versão


3. O Programa de Gerenciamento de Configuração
==============================================

3.1 Identificação da Configuração
---------------------------------
### 3.1.1 Métodos de Identificação
----------------------------------
Cada artefato deve ser nomeado com uma pequena sigla no inicio: H para hardware; SS para software do sistema; TP para produtos de terceiros; e AD para arterfatos de desenvolvimento. Seguido de um hífen e seu nome sem abreviações em caixa alta, logo em seguida deve ser declarado o número da versão do artefato levando em consideração o padrão XX.YY, onde XX significa que é uma versão aprovada e que está em produção e YY é uma versão alterada de XX, da qual ainda não foi aprovada, e sempre que for, incrementar 1 em XX.

### 3.1.2 Itens de Configuração
| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|&lt;Plano de Gerenciamento de Configuração&gt;|&lt;Nelson Rodrigues&gt;|&lt;11/12/2014&gt;|
|&lt;Código Fonte&gt;|&lt;Nilderlan Fernandes Pereira&gt;|&lt;11/12/2014&gt;|


### 3.1.3 Baselines do Projeto

Plano de Gerenciamento de Configurações: estabelecido na Elaboração do projeto, com o inituito de definir como será gerenciado o projeto. Autorizada por Nelson Rodrigues, contendo os padrões a serem seguidos e os planos de gerenciamento.

### 3.1.4 Estrutura do Repositório de Versões

O projeto terá um repositório raiz com um repositório filho para Documentação. Dentro desse haverá uma pasta para cada tipo de documento, onde ficarão os documentos e suas devidas versões. 
Cada release nova do projeto deve conter uma pasta dentro de uma pasta raiz Releases que fica dentro da pasta raiz do projeto. Dentro delas virão suas atividades e dentro dessa vem três subsequentes: trunk, tags, branches

3.2 Controle de Configuração e Mudança
--------------------------------------

### 3.2.1 Processamento e Aprovação de Solicitações de Mudança

As solicitações de mudanças são enviadas para o CCB, inicia uma analise, caso essa analise de mudança seja validada é dado inicio a execução da mudança, finalizando com o desenvolvimento, passa para fase de teste, os testes são analisados novamente e caso ocorra tudo certo a mudança é finalizada.

Status de Mudança.
Aberto - Criação da Solicitação
Em Analise - Analise da solicitação
Analisado - Aguardando Desenvolvimento
Em Desenvolvimento - Solicitação sendo desenvolvida
Desenvolvido - Aguardando Teste
Em testes - Solicitação em teste
Testado com erro - Aguardando Desenvolvimento
Testado sem erro - Solicitação esperando finalização
Finalizado - Solicitação finalizada.

### 3.2.2 Comitê de Controle de Mudança (CCB)

Fazem parte do CCB: Gerente de Projeto, Analista de Sistemas e Analista de Testes.


4. Padrões e Procedimentos
==========================
Deve se seguir um padrão de nomenclatura, como foi citado. A criação de repositórios deve ser levada em consideração com extrema cautela. Qualquer mudança deve ser encaminhada ao CCB. E as auditorias serão feitas ao fim de cada release a fim de verificar se há problemas e acompanhar suas resoluções.



5. Treinamento e Recursos
=========================
| Treinamento | Objetivo | Público Alvo |
|---------------|------------------------|------------------------|
|Repositório | Trinemento ensina como acessar o repositório através de uma máquina cliente, como dar os comandos mais importantes do repositório e como fazer a inclusao de novos itens.| Toda a equipe |



6. Auditorias de Configuração
=============================
A auditoria será feita ao fim de cada release, verificando se o que foi feito está seguindo os padrões definidos. Caso hajam problemas, eles serão documentados e colocados em um kanban virtual que permitirá o acompanhamento em tempo real.
