# Trabalho de Grupo
Trabalho final de programação

**Membros do grupo:** Mariana Pereira e Daniela Araújo.

**Contexto**

O nosso trabalho consiste num conjunto de perguntas relativas aos dados das primeiras 6 temporadas do reality show "Shark Tank". Este conjunto de dados é constituído pelo número correspondente às temporadas, episódios, companhias, negócio, indústria, género dos concorrentes, a quantia da proposta de investimento, o respetivo feedback se os sharks investiram ou não, o total do investimento, seis perguntas e as suas respetivas respostas. 

**Bibliografia**

* Fonte de Dados: Dados do Shark Tank para as temporadas 1-10 coletados por Halle Tecco, para consulta em: https://docs.google.com/spreadsheets/u/1/d/1Lr0gi_QJB_JU0lBMjJ7WiBRxA0loml1FlM-KlmKsaEY/htmlview?pli=1#

* Fonte de Dados do CSV: Dados do Shark Tank para as temporadas 1-6 coletados por Halle Tecco, extraído em: https://gist.github.com/apurvadave/3afe546bc05e4e544b24

**Estrutura**

O repositório está organizado da seguinte forma:
+ `data.csv`: Conjunto de dados relativos às temporadas 1-6 do reality show "Shark Tank", extraído em https://gist.github.com/apurvadave/3afe546bc05e4e544b24

+ `Shark Tank Investment Data (by @halletecco) - Google Drive.html`: contém dados detalhados relativos às temporadas 1-10, coletados por Halle Tecco, para consulta em: https://docs.google.com/spreadsheets/u/1/d/1Lr0gi_QJB_JU0lBMjJ7WiBRxA0loml1FlM-KlmKsaEY/htmlview?pli=1#

+ `Parte A.ipynb` contém os dados devidamente processados, analisados e com a respetiva visualização de informações extraídas.

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
