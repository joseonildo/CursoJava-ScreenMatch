# CursoJava-ScreenMatch
Conteúdo pratico do Curso feitos na Escola Alura - ScreenMatch - Atualizado e aperfeiçoado.

# APP - Busca de Filmes e Séries

Este aplicativo permite a busca de filmes e séries através da API OMDB, exibe uma lista dos resultados encontrados e oferece a opção de gerar arquivos de texto (.txt) ou JSON (.json) com as informações. Ele também permite que o usuário altere a chave de API e armazene a lista pesquisada.

## Funcionalidades

- **Busca de Filmes e Séries**: Realiza buscas de filmes e séries através da API OMDB com base em uma chave de API fornecida pelo usuário.
- **Armazenamento de Títulos**: Armazena os filmes e séries encontrados em uma lista para visualização posterior.
- **Geração de Arquivos**: Permite gerar um arquivo `.txt` ou `.json` com as informações dos títulos encontrados.
- **Alteração de Chave da API**: O usuário pode alterar a chave de acesso à API OMDB a qualquer momento.
- **Exibição de Lista de Títulos**: Exibe a lista de filmes e séries pesquisados no terminal.

## Como Usar

1. **Configuração da Chave da API**:
   Ao iniciar o aplicativo, você será solicitado a fornecer a chave da API OMDB (que deve ter 8 caracteres). Essa chave será usada para realizar as buscas de filmes e séries.

2. **Menu Principal**:
   Após configurar a chave da API, o aplicativo exibirá um menu com as seguintes opções:
   - **1**: Trocar a chave da API.
   - **2**: Buscar filmes ou séries e armazenar na lista.
   - **3**: Exibir a lista de títulos pesquisados.
   - **4**: Gravar a lista de títulos em um arquivo `.txt`.
   - **5**: Converter a lista para JSON e gravar em um arquivo `.json`.
   - **0**: Sair do aplicativo.

3. **Exemplo de Execução**:
   - O usuário começa fornecendo a chave da API OMDB.
   - Depois, o usuário pode realizar buscas, visualizar a lista e escolher gerar arquivos de saída.

4. **Saída**:
   - O aplicativo exibe a lista de filmes e séries pesquisados com detalhes como nome, lançamento, nota e duração.
   - Arquivos `.txt` e `.json` são gerados para armazenar os dados de pesquisa.

## Estrutura do Projeto

- **Pacotes**:
  - `br.com.alura.screenmatch.modelos`: Contém as classes `Filme`, `Serie`, `Titulo` e `TituloJson`, que representam os títulos de filmes e séries.
  - `br.com.alura.screenmatch.complementos`: Contém a classe `PesquisaTitulos`, que gerencia a busca de filmes e séries na API, e a classe `GeradorDeArquivo`, que grava a lista de títulos em arquivos.
  - `br.com.alura.screenmatch.excecao`: Contém a exceção personalizada `ErroDeConversaoDeAnoException`.
  - `br.com.alura.screenmatch.principal`: Contém a classe principal `AppBuscaFilmes`, que inicia o aplicativo e gerencia a interação com o usuário.

## Como Rodar

1. **Pré-requisitos**:
   - Java 11 ou superior instalado.
   - Conexão com a internet para acessar a API OMDB.

2. **Passos para execução**:
   - Compile e execute a classe `AppBuscaFilmes`.
   - Acompanhe o menu de opções e interaja com o sistema conforme necessário.

## Exceções e Erros:

- Se a chave da API fornecida for inválida (não contiver 8 caracteres), o sistema solicitará que o usuário insira uma chave válida.
- Em caso de falhas de rede ou problemas ao acessar a API OMDB, mensagens de erro serão exibidas.

## Desenvolvedor

Desenvolvido por **José Onildo**.
