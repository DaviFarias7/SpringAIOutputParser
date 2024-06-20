## Projeto criado para consumir a api de chatbot do  com Spring AI

A interface OutputParser permite obter saída estruturada, por exemplo, mapeando a saída para uma classe Java ou um array de valores a partir da saída baseada em String dos modelos de IA.
Você pode pensar nisso em termos semelhantes ao conceito de RowMapper ou ResultSetExtractor do Spring JDBC. Os desenvolvedores querem converter rapidamente os resultados de um modelo de IA em tipos de dados que podem ser passados para outras funções e métodos em sua aplicação. O OutputParser ajuda a alcançar esse objetivo.
Construí este projeto utilizando a documentação do Spring AI. Nele, o resultado do prompt passado para IA segue os atributos da classe "ActorsFilms", que são "actor"(nome do ator) e "movies"(filmes do ator). 
Com isto, na classe OutputParserController eu defino o que a IA irá listar na resposta String userMessage = """ Generate the filmography for the actor {actor}. {format} """ (Gere para mim a filmografia do ator X).

### Documentação do Spring AI
A documentação do OutputParser foi removida pois a partir de 02.05.2024 as classes OutputParser, BeanOutputParser, ListOutputParser e MapOutputParser ficaram obsoletas e foram substituídas pelas classes StructuredOutputConverter, BeanOutputConverter, ListOutputConverter e MapOutputConverter. 

https://docs.spring.io/spring-ai/reference/api/structured-output-converter.html


### Endpoint listando os filmes do ator digitado

![image](https://github.com/DaviFarias7/SpringAIOutputParser/assets/86566715/3e425b5d-2eff-45c9-a691-9073a09f1e37)


