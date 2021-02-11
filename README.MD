# Take_StringAnalyzer
Codigo feito para o processo seletivo da empresa Take.
O código é simples e contém a classe StringAnalysis.

Você passa uma stream em formato de string como argumento para a classe e ela armazena todas as palavras (pontuações são retiradas).
Através do método get_most_similar_word() você pode retornar a string da stream mais próxima de uma palavra do dicionário. É importante ressaltar que a comparação não é case-sensitive, ou seja, os caracteres 'A' e 'a' são considerados iguais.
A métrica de distãncia de strings usada aqui é conhecida como distância de edição ou distância de Levenshtein. Mais informações em: https://en.wikipedia.org/wiki/Levenshtein_distance

Abaixo um exemplo do funcionamento da classe:


- string_analyzer = StringAnalysis("Ola, esse codigo foi gerado como parte da avaliacao tecnica da take. Meu nome e gabriel resende goncalves e estou terminando o doutorado na UFMG. Minhas principais areas de pesquisa sao aprendizagem de maquina ou inteligencia artificial, reconhecimento de padroes visuais e visao computacional. Tenho 29 anos e moro em Belo Horizonte")

- print(string_analyzer.get_most_similar_word("Guilherme"))
- print(string_analyzer.get_most_similar_word("Took"))
- print(string_analyzer.get_most_similar_word("Ei"))
- print(string_analyzer.get_most_similar_word("programando"))
- print(string_analyzer.get_most_similar_word("50"))
- print(string_analyzer.get_most_similar_word("Feio"))
- print(string_analyzer.get_most_similar_word("artificial"))

Output:
- minhas
- ola
- ola
- e
- doutorado
- 29
- belo
- artificial
