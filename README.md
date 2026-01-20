Como Rodar o Projeto com Docker:

#### ℹ️ Certifique-se de ter o Docker e o Docker Compose instalados.

---

### Primeiramente

Crie um diretório chamado tc2;

Dentro desse diretório, clone cada um dos três projetos:
- ``` git clone https://github.com/grupo21-tech-challange-02/docker-compose.git ```
- ``` git clone https://github.com/grupo21-tech-challange-02/root-config.git ```
- ``` git clone https://github.com/grupo21-tech-challange-02/finance-app.git ```

---

#### Primeiro Passo (Build)
Na primeira vez que executar o projeto, use o comando abaixo para construir as imagens e baixar as dependências:<br />
``` docker compose up --build ```

#### Próximas Execuções -  Nas vezes seguintes, você pode subir o projeto de forma muito mais rápida utilizando o modo "detached" (em segundo plano):
```docker compose up -d```

#### Parar o Projeto - Para encerrar os serviços e remover os containers:
```docker compose down```

#### Caso necessite garantir que não reste containers orfãos:
```docker compose down --remove-orphans```

---

#### ℹ️ Dica:
- Se você adicionar uma nova biblioteca ou alterar o arquivo de configuração do sistema, lembre-se de rodar o comando com ```--build``` novamente para atualizar a imagem.
