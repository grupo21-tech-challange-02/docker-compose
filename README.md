Como Rodar o Projeto com Docker
Certifique-se de ter o Docker e o Docker Compose instalados.

* Primeiro Passo (Build)
Na primeira vez que executar o projeto, use o comando abaixo para construir as imagens e baixar as dependências:
    docker compose up --build
* Próximas Execuções -  Nas vezes seguintes, você pode subir o projeto de forma muito mais rápida utilizando o modo "detached" (em segundo plano):
    docker compose up -d
* Parar o Projeto - Para encerrar os serviços e remover os containers:
    docker compose down
* Caso necessite garantir que não reste containers orfãos:
    docker compose down --remove-orphans
Dica: Se você adicionar uma nova biblioteca ou alterar o arquivo de configuração do sistema, lembre-se de rodar o comando com --build novamente para atualizar a imagem.
