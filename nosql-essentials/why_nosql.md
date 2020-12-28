# Why NoSQL

## Nesse rascunho irei descrever sobre a dominância do SQL e afirmar que o 'boom' do NoSQL não é momentâneo.

### O valor dos banco de dados Relacionais:

- Dados persistidos: 
Essa vantagem está relacionado a forma como os dados das aplicações ficam salvos. Com o uso de SGBD's pode-se guardar os dados no disco (*backing store*),
em vez de salvar em arquivos que ficavam no S.O. Com isso, ganha-se produtividade pela facilidade de conseguir salvar rapidamente grande quantidade de dados e a capacidade
de buscar parte dos dados de forma mais rápida do que em arquivos.

- Concorrência:
Quando dois processos tentam acessar/modificar o mesmo dado (duas pessoas tentando comprar um mesmo acento em um concerto). Nesse cenário deve ser implementado uma
coordenação de acessos, para que evite-se erros e informações incosistentes. **Bancos relacionais** resolvem isso usando o conceito de **transações**.

- Integração:
Várias aplicações podem juntas formar uma grande aplicação, que dependem dos dados de uma das outras. Uma possível solução para isso, usando bancos relacionais,
é criar uma arquitetura de *shared database integration*, em que todas as aplicações acessam um mesmo repositório de dados. Assim, graças ao conceito de transação descrito anteriormente, as aplicações conseguem escrever/ler dados com garantia de estarem íntegros.

- Um modelo Padronizado:
