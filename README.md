# Curso
# API de Musica
Esta Api é utilizada para...

## Endpoints 
Colocar todas as rotas aqui:

### GET /games
Esse endpoint é responsavel por retornar todos os games
#### Parametros que recebe
Nenhum
#### Respostas
##### ok! 200
Caso essa resposta aconteça voce vai receber a listagem de todos os games

Exemplo de resposta:
```
[
    {
        "id: 23, 
        "title": "call of duty",
        "year": 2019,
        "price": 60
    },

    etc
]
```
##### Falha de autenticaçao! 401
Caso essa resposta aconteça, isso significa que aconteceu alguma falha durante o processo de autenticação da requisicao. Motivos: Token invalido, token expirado.

Exemplo de resposta:
```
{
    "err": "Token INvalido"
}
```


### POST /auth
Esse endpoint é responsavel pelo processo de login
#### Parametros que recebe
email: E-mail registado no sistema

password: Senha do utilizador registado no sistema, com determinado email. 

Exemplo:
```
{
    "email": "dsjkdsj@jfdks",
    "password": "fjejl
}
```

#### Respostas
##### ok! 200
Vai receber o token JWT para conseguir aceder endpoints protegidos na API.

Exemplo de resposta:
```
    {
        "token":
        "adjakldjaljaldajldasjlkjal" 
    }

    etc

```
##### Falha de autenticaçao! 401
Caso essa resposta aconteça, isso significa que aconteceu alguma falha durante o processo de autenticação da requisicao. Motivos:  Senha ou email invalidos. 

Exemplo de resposta:
```
{
    "err": "Credenciais invalidas"
}
```







