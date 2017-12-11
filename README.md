<!--
Exercícios de Introdução à Computação (c) by Nuno Fachada

Exercícios de Introdução à Computação is licensed under a Creative Commons
Attribution-NonCommercial-ShareAlike 4.0 International License.

You should have received a copy of the license along with this
work. If not, see <http://creativecommons.org/licenses/by-nc-sa/4.0/>.
-->

[![Exercícios: CC BY-NC-SA 4.0](https://img.shields.io/badge/Exercícios-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![Código: GPL v3](https://img.shields.io/badge/Código-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

# Exercícios de Introdução à Computação

Este repositório contém uma série de exercícios da disciplina de Introdução à
Computação da [Licenciatura em Aplicações Multimédia e Videojogos][lamv] da
[Universidade Lusófona de Humanidades e Tecnologias][ULHT] em Lisboa.

Os alunos podem e devem fazer _fork_ deste repositório, clonar o mesmo para o
seu PC e propor resoluções para os exercícios (e mesmo novos exercícios)
através de _pull requests_. A forma de colaboração está descrita em detalhe na
secção [Colaboração](#colab).

## Conteúdos

1. [Arquitectura de computadores](problemas/01_arquitectura.md)
2. [Bases de numeração](problemas/02_bases.md)
3. [Linha de comandos](problemas/03_cmd.md)
4. [Introdução ao C](problemas/04_introc.md)
5. [Operadores e operações](problemas/05_operacoes.md)
6. [Controlo de fluxo](problemas/06_controlofluxo.md)
7. [Funções](problemas/07_funcoes.md)
8. [Fluxogramas](problemas/08_fluxogramas.md)
9. [Markdown](problemas/09_markdown.md)
10. [Git](problemas/10_git.md)
11. [Arrays e apontadores](problemas/11_arrays.md)
12. [Strings](problemas/12_strings.md)
13. [Ficheiros](problemas/13_ficheiros.md)
<!--
14. [Estruturas e definição de tipos](problemas/14_structs.md)
15. [Organização de um programa](problemas/15_org.md)
16. [Documentação com Doxygen](problemas/16_doxy.md)
17. [Gestão dinâmica da memória](problemas/17_mem.md)
18. [Estruturas de dados](problemas/18_aed.md)
19. [Bibliotecas externas: G2](problemas/19_bibg2.md)
-->

<a name="colab" />

## Colaboração

Os alunos podem contribuir com soluções para os exercícios propostos, podendo
inclusive propor novos exercícios. Os seguintes passos descrevem uma forma
relativamente simples de contribuir para este repositório.

### Que ficheiros alterar?

Os exercícios estão na pasta [problemas](problemas). Cada ficheiro Markdown
corresponde aos exercícios de uma parte da matéria. Se o aluno adicionar um
exercício, deve seguir a numeração e formatação dos exercícios anteriores. Pode
opcionalmente adicionar a autoria do exercício através de um _link_ à sua
página do GitHub.

As soluções estão na pasta [solucoes](solucoes). Por sua vez, cada sub-pasta
contém uma série de ficheiros Markdown com as soluções dos exercícios de
determinada parte da matéria. Cada ficheiro corresponde a uma ou mais soluções
de apenas um dos exercícios. Se o aluno apresentar uma nova solução, pode
opcionalmente assinar a autoria da mesma através de um _link_ à sua página do
GitHub.

Em qualquer dos casos, o aluno pode também adicionar o seu nome/_link_ a
página do GitHub na secção Colaboradores desta página, mais abaixo.

São ainda aceites _pull requests_ com correções a esta página, às licenças, e
por ai fora.

### Obter/atualizar repositório local

#### Primeira colaboração

1. Cria uma cópia (*fork*) deste repositório (tipicamente denominado
_upstream_) na tua conta do GitHub (botão **Fork** no canto superior direito).
A cópia do repositório na tua conta é geralmente chamada _origin_.
2. Obtém uma cópia local (no teu PC) do repositório _origin_ com o comando
`git clone https://github.com/OTeuUserName/ic_exercicios.git` (substituir
`OTeuUserName` pelo teu nome de utilizador no GitHub).
3. Dar conhecimento ao teu repositório local da existência do repositório
remoto _upstream_ com o comando
`git remote add upstream https://github.com/VideojogosLusofona/ic_exercicios.git`.

<a name="colabseg" />

#### Colaborações seguintes

1. No teu repositório local, certifica-te que estás no ramo _master_:
    - `$ git checkout master`
2. Descarrega as novidades do repositório _upstream_ e junta-as (_merge_) ao
teu ramo _master_:
    - `$ git fetch upstream`
    - `$ git merge upstream/master`
3. Carrega (_push_) as novidades do _upstream_ para o repositório _origin_:
    - `$ git push origin master`

### Efetuar alterações e solicitar integração

1. Dentro da pasta dos exercícios, chamada *ic_exercicios*, cria um ramo
(_branch_) para inserires as tuas novas propostas:
    - `$ git branch meu_ramo`
    - `$ git checkout meu_ramo`
    - O nome `meu_ramo` pode ser substituído por qualquer outro nome.
    - O primeiro comando cria o ramo, o segundo comando muda o git para esse
      ramo. Os dois comandos podem ser compactados num só:
      `$ git checkout -b meu_ramo`.
2. Uma vez no novo ramo, faz as alterações/propostas às soluções e/ou aos
exercícios. Cada alteração/proposta deve ser especificada com pelo menos um
_commit_:
    - `$ git add nome_dos_ficheiros_alterados`
    - `$ git commit -m "Descrição das alterações efetuadas"`
3. O `novo_ramo` deve ser carregado (_pushed_) para o repositório _origin_ (ou
seja, para o *fork* que criaste no GitHub):
    - `$ git push -u origin meu_ramo`
    - A opção `-u` é necessária pois nesta fase o teu repositório no GitHub
      (_origin_) ainda não conhece o ramo chamado `meu_ramo`.
4. Uma vez confirmado que o _push_ foi realizado com sucesso, deve ser
solicitado um *pull request* (pedido de integração) na árvore original dos
exercícios (_upstream_). Para o efeito basta clicar no botão
**New pull request** e solicitar a seguinte integração:
    - _Base fork_ **VideojogosLusofona/ic_exercicios**, _base_ **master**
    (local onde queres integrar as tuas alterações).
    - _Head fork_ **OTeuUserName/ic_exercicios**, _compare_ **meu_ramo** (as
    tuas alterações que queres ver integradas).
    - Clica no botão verde **Create pull request**, e deixa uma pequena
    descrição da razão do pedido de integração, clicando depois novamente em
    **Create pull request**.
5. Caso o _pull request_ não tenha sido aceite, volta ao ponto 2.
6. Caso o _pull request_ tenha sido aceite, podes seguir os passos indicados
em [Colaborações seguintes](#colabseg), de modo a juntares as alterações que
propuseste ao teu ramo `master`. Posteriormente podes eliminar o `meu_ramo`
localmente e remotamente (_origin_) com os seguintes comandos:
    - `$ git branch -d meu_ramo`
    - `$ git push origin :meu_ramo`

## Licenças

Estes exercícios são disponibilizados através da licença [CC BY-NC-SA 4.0].
O código associado aos exercícios é disponibilizado através da licença [GPLv3].

## Metadados

* Autor: [Nuno Fachada]
* Colaboradores: [Tiago Ferreira Alves](https://github.com/synpse),
  [Rui Martins](https://github.com/rui-martins)
* Curso: [Licenciatura em Aplicações Multimédia e Videojogos][lamv]
* Instituição: [Universidade Lusófona de Humanidades e Tecnologias][ULHT]

[GPLv3]:https://www.gnu.org/licenses/gpl-3.0.en.html
[CC BY-NC-SA 4.0]:https://creativecommons.org/licenses/by-nc-sa/4.0/
[lamv]:https://www.ulusofona.pt/licenciatura/aplicacoes-multimedia-e-videojogos
[Nuno Fachada]:https://github.com/fakenmc
[ULHT ]:https://www.ulusofona.pt/
