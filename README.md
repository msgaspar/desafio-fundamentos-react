<h3>
  Desafio 07: GoFinances Web
</h3>

Nesse desafio, continuamos desenvolvendo a aplicação de gestão de transações, a GoFinances., dessa vez aplicando o que vimos até agora no React.js junto com TypeScript, utilizando rotas e envio de arquivos por formulário.

Essa aplicação irá se conectar backend do desafio anterior, exibir as transações criadas e permitir a importação de um arquivo CSV para gerar novos registros no banco de dados.


### Funcionalidades da aplicação

- **`Listar as transações da API`**: A página `Dashboard` deve ser capaz de exibir uma listagem através de uma tabela, com o campo `title`, `value`, `type` e `category` de todas as transações que estão cadastradas na sua API.

**Dica**: Utilizar a função [Intl](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/NumberFormat) para formatar os valores. Dentro da pasta `utils` no template você encontrará um código para te ajudar.

- **`Exibir o balance da API`**: A página `Dashboard` deve exibir o balance que é retornado do backend, contendo o total geral, junto ao total de entradas e saídas.

- **`Importar arquivos CSV`**: A página `Import` deve permitir o envio de um arquivo no formato `csv` para o backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte [modelo](https://github.com/Rocketseat/bootcamp-gostack-desafios/blob/master/desafio-database-upload/assets/file.csv).

**Dica**: Foi disponibilizado um componente chamado `Upload` na pasta `components` para você ter já preparado uma opção de drag-n-drop para o upload de arquivos. PS: Caso você esteja no windows e esteja sofrendo com algum erro ao tentar importar CSV, altere o tipo de arquivo dentro do arquivo `components/upload/index.ts` de `text/csv` para `.csv, application/vnd.ms-excel, text/csv`.

**Dica 2**: Utilize o [FormData()](https://developer.mozilla.org/pt-BR/docs/Web/API/FormData/FormData) para conseguir enviar o seu arquivo para o seu backend.

