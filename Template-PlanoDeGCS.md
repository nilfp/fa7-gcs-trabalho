<SCV - Sistema de Controle de Veículos>
=================
Plano de Gerenciamento de Configuração
======================================
Versão &lt;1.0&gt;
------------------

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP).  O texto exibido entre colchetes e em itálico foi incluído para orientar o autor e deve ser excluído antes da publicação do documento._

_Este documento utiliza a formatação da linguagem [Markdown] (http://daringfireball.net/projects/markdown/). Você pode encontrar um guia de referência rápido [aqui] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).]_

Histórico de Versões
--------------------

|Data                |Versão       |Descrição               |Autor          |
|--------------------|-------------|------------------------|---------------|
|_&lt;09/12/2014&gt;_|_&lt;1.0&gt;_|_&lt;Versão inicial - Definição do Plano GCS&gt;_|_&lt;Nelson Rodrigues&gt;_|
|_&lt;dd/mm/aaaa&gt;_|_&lt;1.1&gt;_|_&lt;Outra versão&gt;_  |_&lt;autor&gt;_|



1. Introdução
==============

O Pleno de Gerenciamento de Configuração descreve todas as atividades do Gerenciamento de Controle de Configuração e Mudança que serão executadas durante o ciclo de vida do produto. Suas atividades envolvem identificar a configuração do software, manter sua integridade durante o projeto e controlar sistematicamente as mudanças.

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
_[Descreva como os artefatos do projeto ou produto devem ser nomeados, marcados e numerados. O esquema de identificação deve abranger o hardware, o software do sistema, os produtos de terceiros (COTS) e todos os artefatos de desenvolvimento de aplicativos listados na estrutura de diretórios do produto; por exemplo, planos, modelos, componentes, software de teste, resultados e dados, executáveis e assim por diante.]_

### 3.1.2 Itens de Configuração
_[Relacionar os artefatos ou grupos de artefatos, separando por tipo, modulo ou subsistema, responsável ou momento em que deverão ser incluídos em baselines._
* _“Inclusão em Baseline” em branco significa que o grupo de artefatos não participará de baseline. Pode ser expresso como uma data ou identificador de uma baseline, fase ou ponto de controle_
* _“Responsável”: indicar nominalmente, sempre que possível]_

| Item (ou Tipo de Item)                 | Responsável na equipe	     | Inclusão em Baseline |
|----------------------------------------|-----------------------------|----------------------|
|_&lt;grupo de itens de configuração&gt;_|_&lt;nome do responsável&gt;_|_&lt;momento a partir do qual o conjunto de artefatos será incluído em baseline&gt;_|


### 3.1.3 Baselines do Projeto

_[As baselines funcionam como um padrão oficial no qual os trabalhos subseqüentes são baseados. Somente mudanças autorizadas podem ser efetuadas nas baselines._
_Descreva em que pontos do ciclo de vida do projeto ou produto as baselines devem ser estabelecidas. As baselines mais comuns devem ser definidas ao final de cada uma das fases de Iniciação, Elaboração, Construção e Transição. Elas também podem ser geradas no final de iterações ocorridas dentro das várias fases ou com freqüência ainda maior._
_Descreva quem autoriza uma baseline e o que ela contém.]_

### 3.1.4 Estrutura do Repositório de Versões
_[Descreva a organização de diretórios do seu repositório e que itens/arquivos devem ser armazenados em cada diretório.]_

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
_[Descreva os padrões e procedimentos que devem ser seguidos no projeto. Crie subseções se achar necessário, para organizá-los melhor.]_



5. Treinamento e Recursos
=========================
| Treinamento | Objetivo | Público Alvo |
|---------------|------------------------|------------------------|
|Repositório | Trinemento ensina como acessar o repositório através de uma máquina cliente, como dar os comandos mais importantes do repositório e como fazer a inclusao de novos itens.| Toda a equipe |



6. Auditorias de Configuração
=============================
_[Descreva o cronograma das auditorias de configuração e o que será verificado. Informe também como serão reportados os problemas encontrados e onde sera feito o acompanhamento dos itens corretivos.]_
