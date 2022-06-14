# Trabalho de Grupo
Trabalho final de programação

**Membros do grupo:** Mariana Pereira e Daniela Araújo.

**Contexto**

O nosso trabalho consiste num conjunto de perguntas relativas aos dados das primeiras 6 temporadas do reality show "Shark Tank". Este conjunto de dados é constituído pelo número correspondente às temporadas, episódios, companhias, negócio, indústria, género, o valor pedido de investimento, os "sharks" para determinar se participaram no negócio, o total do investimento, seis perguntas e as suas respetivas respostas. 

**Bibliografia**

* Fonte de Dados: Dados do Shark Tank para as temporadas 1-10 coletados por Halle Tecco, para consulta em: https://docs.google.com/spreadsheets/u/1/d/1Lr0gi_QJB_JU0lBMjJ7WiBRxA0loml1FlM-KlmKsaEY/htmlview?pli=1# 

* Fonte de Dados do CSV: Dados do Shark Tank para as temporadas 1-6 coletados por Halle Tecco, extraído em: https://gist.github.com/apurvadave/3afe546bc05e4e544b24


**Estrutura**

O repositório está organizado da seguinte forma:
+ `data.csv`: Conjunto de dados relativos às temporadas 1-6 do reality show "Shark Tank", extraído em (https://gist.github.com/apurvadave/3afe546bc05e4e544b24)
+ `vacinas_detalhe.csv`: contém dados detalhados semanais relativos à vacinação, extraídos do [dataset do relatório de vacinação](https://covid19.min-saude.pt/relatorio-de-vacinacao/) da DGS. Nota: até 17-03-2021 incluia apenas população residente no continente, vide nota de `vacinas.csv`. Nota: tal como todos os outros `csv`, a coluna `data` corresponde ao dia seguinte aos dados reportados (7 dias neste caso), enquanto o `Relatório PDF` refere o último dia desses 7 dias, e o `Dataset CSV` refere o primeiro dia desses 7 dias.
+ `data_concelhos.csv`: contém dados acumulados relativos aos confirmados por concelho, extraídos do [dashboard da DGS](https://covid19.min-saude.pt/ponto-de-situacao-atual-em-portugal/) (e por isso sujeito às mesmas limitações relativamente a abrangência e protecção de dados, nomeadamente concelhos com menos de 3 confirmados não são reportados). Esta série de dados tem início a 24-03-2020 e tem cadência diária até 04-07-2020, passando a cadência semanal a 14-07-2020, e terminando a 26-10-2020. Vide os próximos dados para o novo formato.
+ `data_concelhos_14dias.csv` e `data_concelhos_incidencia.csv` contém dados de confirmados do acumulado dos 14 dias anteriores à data do reporte, no primeiro ficheiro, e proporcional a 100k habitantes no segundo ficheiro. Inclui os dados calculados do `data_concelhos.csv` desde que os daddos são semanais, nomeadamente entre 27-07-2020 (correspondendo ao periodo de 13-07-2020 a 26-07-2020) até 26-10-2020, e será actualizado conforme seja disponibilizado pela DGS (semanalmente à segunda-feira).
+ `archive/`: arquivo de todos os relatórios de situação disponibilizados pela DGS, em formato `.pdf`. Os relatórios são disponibilizados diariamente, desde o dia 03-03-2020.
+ `notebooks/`: contém um _notebook_ Python com um exemplo simples de como carregar e visualizar os dados.
+ `extra/`: contém fontes de dados extras que podem ser usadas para complementar as análises dos restantes dados. As descrições dessas fontes de dados encontram-se dentro de um README nessa pasta.

**Dicionário de dados**

Uma explicação do conteúdo em `data.csv`.

* Shark Tank Data

| Nome da coluna        | Significado           | Possíveis valores  |
| ------------- |:-------------:| -----:|
| `row` | linha | valor correspondente à respetiva linha em questão e assim sucessivamente |
| `season` | temporada a que irá corresponder os dados seguintes | temporada 1 a 6 |
| `no. in series` | número do episódio contextualiza o resto da informação | números de 1 a 29 |
| `company` | companhia que propõe o negócio | nome da companhia |
| `deal` | é o feedback relativo ao negócio ter sido aceite ou não | sim ou não (yes or no) |
| `industry` | enquadrar a companhia na indústria a que se destina | nomes das inústrias, por exemplo de healthcare, business services etc |
| `entrepreneur gender` | referir o género de cada concorrente, ou mais concretamente o sexo feminino ou masculino | feminino ou masculino (female or male) |
| `amount` | quantia proposta pelos concorrentes na apresentação do seu produto | valores em doláres, como por exemplo $50,000 |
| `equity` | patrimônio líquido ou capital próprio, representa efetivamente os valores que os sharks têm na empresa no momento de investimento | percentagem, como por exemplo 55% |
| `valuation` | avaliação do valor monetário da empresa, que consiste num cálculo, em que se multiplica o preço das ações da empresa pelo número total de ações em circulação |  valores em doláres, como por exemplo $90,909 |
| `corcoran` | shark barbara corcoran | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `cuban` | shark mark cuban | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `herjavec` | shark robert herjavec | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `john` | shark daymond john | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `o'leary` | shark kevin o'leary | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `guest` | convidados do programa que investem, como é o exemplo do Ashton Kutcher | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `# sharks` | total de sharks que investiram | valores de 1 a 5 |
| `$ per shark` | quantia total do investimento | valores em dólares, como por exemplo $50,000 |
| `details/notes` | detalhes/notas do acordo final para finalizar o negócio | indicações, como por exemplo 2% royalty |
