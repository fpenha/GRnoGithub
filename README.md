# Gerenciamento de Requisitos no Github

## Higeia - Sistema Hospitalar (Contexto Fictício)

### Uma Breve Descrição do Contexto / Problema

**Penha Corporation**, uma holding familiar com participação em grandes empresas espalhadas pelo mundo, nos contratou (esta turma, esta sala de aula) 
para desenvolvermos uma solução no qual pudéssemos tornar os processos relacionados aos serviços prestrados pelo **Hospital Penha** mais ágeis, gerenciáveis, 
eficazes e eficientes, evitando assim que uma decisão gerancial seja pautado sem embasamento. Então, após a discussão com os envolvidos/interessados, 
os seguintes requisitos foram brevemente capturados para projetarmos um sistema que permita acompanhar um paciente da acolhida/entrada até a sua alta/saída, 
registrando todos os dados e oferecendo informações para direcionarmos os procedimentos.

### Iteração-I: Controle da Estrutura Oferecida

Nesse primeiro momento, como uma prova de conceito e viabilidade, hospital precisa de um sistema que armazene os dados dos leitos em diferentes alas. 
O sistema deverá permitir o armazenamento de um número fixo, já que cada ala tem um número limitado de leitos.

## Nosso Processo 

<img src="https://github.com/user-attachments/assets/c31a7632-5f74-4282-a38d-1b265bf6cf75" width="600px" height="200px" />  

O Processo que será utilizado para o desenvolvimento do Sistema Hospitalar ( Higeia ), solicitado pela **Penha Corporation**, 
foi instanciado pela mescla dos seguintes modelos modelos de ciclo de vida de software: **iterativo** e **incremental**. 

<img src="https://github.com/user-attachments/assets/219e8a3d-2cb3-4914-85ad-a798849bdac1" width="500px" height="300px" />  

- **O DONO DO PRODUTO {ANALISA} A SOLICITAÇÃO**
  - **ENTRADA** : NESSECIDADE/CONDIÇÃO/CAPACIDADE/RESTRIÇÃO (ABSTRATO)
  - **SAÍDA** : ARTEFATO DE REQUISITOS ANALISADO  
- **O DONO DO PRODUTO [, _TESTADOR_,  _DESENVOLVEDOR_] {ESPECIFICA} O QUE REALIZAR**
  - **ENTRADA** : ARTEFATO DE REQUISITOS ANALISADO  
  - **SAÍDA** : ARTEFATO DE REQUISITOS DETALHADO   
- **O DONO DO PRODUTO [, _TESTADOR_, _DESENVOLVEDOR_] {PLANEJA} O ENTREGARÁ**
  - **ENTRADA** : ARTEFATO DE REQUISITOS DETALHADO
  - **SAÍDA** : TAREFAS
- **O DESENVOLVEDOR {CODIFICA} A TAREFA**
  - **ENTRADA** : TAREFA
  - **SAÍDA** : PRODUTO INCREMENTADO  
- **O TESTADOR [DONO DO PRODUTO, DESENVOLVEDOR] {REVISA} O REALIZADO**
  - **ENTRADA** : PRODUTO INCREMENTADO
  - **SAÍDA** : TAREFA ARQUIVADA OU REABERTA  
  
## Padrões Estabelecidos para o Desenvolvimento   

**Padrão de Desenvolvimento, Manutenção e Evolução do Produto**
    
 1. Estabeleça, criando ou selecionado, a Necessidade em um Artefato de Requisitos do Produto;  
 2. Se necessário, refina o Artefato de Requisitos em questão;  
 3. Especifique **O QUE** precisa ser feito em **ISSUEs** relacionadas ao Artefato estabelecido;   
 4. Realize o especificado por meio de **COMMITs** relacionados as **ISSUEs** criada;
 5. Valide o Produto, caso nao esteja satisfatório, siga para o PASSO 2.
 
**Padrão de Diretórios** - Artefatos só podem ser criados dentro dessa estrutura estabelecida. 

- [Requisistos](documentacao/requisitos/) : Artefatos que desencadeará a descrição das funcionalidades do programa.
- [Código Fonte](codigo-fonte/) : Artefatos de código/configuração do programa.

**Padrão para criar os Artefatos de Requisitos** - Os artefatos de requisitos deverão **representar apenas uma funcionalidade**, seguir **o padrão de nomenclatura estabelecido e descrito pelo ambiente** e **uma estrutura de diretório com nomes significativos** para organizar esses artefatos dentro do diretório padrão de [Requisitos](docs/requisitos/).

 - A estrutura de diretórios que armazenará esses artefatos de requisitos criados e mantidos no diretório [Requisitos](documentacao/requisitos/), deverá seguir esta classificação primária : (a) para as necessidades do domínio do problema, os artefatos de requisitos deverão ser organizados no diretório [Requisitos Funcionais](documentao/requisitos/funcionais); (b) para as necessidades determinadas por lei, os artefatos de requisitos deverão ser organizados no diretório [Requisitos Legais](documentacao/requisitos/legais) (c) para características de qualidade do produto, os artefatos de requisitos deverão ser organizados no diretório [Requisitos Não-Funcionais](documentacao/requisitos/n-funcionais);   
   
 - Padrão de nomenclatura
   - `REQ.` como prefixo para identificar os artefatos de requisitos que irão contextualizar as especificações de requisitos ;
   - Em seguida, uma identificação numérica de três dígitos (`REQ.000`) que consiga identificar o artefato de modo único e exclusivo.
   - Por fim, utilizaremos a extensão `.md` para permitir a utilização da [Linguagem de Marcação Markdown](https://www.markdownguide.org/) com intuito de formatar os artefatos de requisitos, possibilitando criar artefatos organizados e de estrutura fluida. (ex.: `REQ.000.md`)
 

