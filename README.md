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
| `Row` | Linha | Valor correspondente à respetiva linha em questão e assim sucessivamente |
| `Season` | Temporada a que irá corresponder os dados seguintes | Temporada 1 a 6 |
| `No. in series` | Número do episódio contextualiza o resto da informação | Números de 1 a 29 |
| `Company` | Companhia que propõe o negócio | Nome da companhia |
| `Deal` | Feedback relativo ao negócio ter sido aceite ou não | Sim ou não (yes or no) |
| `Industry` | Enquadrar a companhia na indústria a que se destina | Nomes das indústrias, por exemplo de healthcare, business services etc |
| `Entrepreneur gender` | Referir o género de cada concorrente, ou mais concretamente o sexo feminino ou masculino | Feminino ou masculino (female or male) |
| `Amount` | Quantia proposta pelos concorrentes na apresentação do seu produto | Valores em doláres, como por exemplo $50,000 |
| `Equity` | Patrimônio líquido ou capital próprio, representa efetivamente os valores que os sharks têm na empresa no momento de investimento | Percentagem, como por exemplo 55% |
| `Valuation` | Avaliação do valor monetário da empresa, que consiste num cálculo, em que se multiplica o preço das ações da empresa pelo número total de ações em circulação |  Valores em doláres, como por exemplo $90,909 |
| `Corcoran` | Shark Barbara Corcoran | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `Cuban` | Shark Mark Cuban | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `Herjavec` | Shark Robert Herjavec | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `John` | Shark Daymond John | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `O'Leary` | Shark Kevin O'Leary | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `Guest` | Convidados do programa que investem, como é o exemplo do Ashton Kutcher | 1 que simboliza que investiu na empresa ou vazio significa que não investiu |
| `# Sharks` | Total de sharks que investiram | Valores de 1 a 5 |
| `$ per shark` | Quantia total do investimento | Valores em dólares, como por exemplo $50,000 |
| `Details/notes` | Detalhes/notas do acordo final para finalizar o negócio | Indicações, como por exemplo 2% royalty |
