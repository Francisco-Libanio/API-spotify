# API-spotify
Explorando a API do Spotify.
## Objetivo:
Realizar captura de dados utilizando API do Spotify, relizar o precesso de ETL para construção de uma Databese contendo as seguintes informções:

- Nome do artista
- Nome da música 
- Genero
- Ano de Lançamento
- Tempo

OBS: O notebook API_Spotify_modelo1 mostra como realizar a consulta de dados no spotify sem o uso da biblioteca Spotipy.

### O código começa importando as bibliotecas necessárias:

- `dotenv` para carregar variáveis de ambiente a partir de um arquivo `.env`.
- `os` para interagir com o sistema operacional.
- `base64` para codificar as credenciais em Base64.
- `requests` para realizar solicitações HTTP.
- `pprint` para exibir os dados de forma mais legível.

## Descrição dos arquivos
Todos os scripts possuem um README interno com descrições de suas funcionalidades

### Usando_Spotipy
Neste arquivo é um exemplo de como coletar o top 50 músicas mais ouvidas no brasil desde os anos 2000, consturir um data frame com essas informações e por fim envialas ao Google planilhas.

### Capturando_dados_de_músicas
Em capturando_dados_de_musicas você pode capturar o dados de uma músicas especifica passando o nome do artista e nome da música dentro do dicionário, é importante lembrar que os nomes devem estar iguais aos nomes cadastrados dentro do spotify fique atento a expressões como "feat", "live" e "&" podem gerar confusão, como padrão é aconcelado utilizar aspas duplas na descrição dos nomes.

### Capturando dado de uma playlist
Para essa implementação em especial será necessario o ID da playlist pode ser encontrar no URL do spotify web localixado após "playlist/"

