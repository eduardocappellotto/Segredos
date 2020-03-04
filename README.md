
# Segredos
 Um projeto web onde busquei implantar diversos métodos de login bem como melhorar a segurança dos dados sensíveis, como senhas e seeds.
 
 ## A aplicação 

Na aplicação, cada usuário pode fazer login e realizar a postagem de um segredo. É possível visualizar o segredo de outras pessoas, mas sem nenhum tipo de identificação, ou seja, é o tipo de aplicação onde a segurança de dados é de extrema importância! 

Login page: ![enter image description here](https://i.imgur.com/neZceAq.png)

Secrets page:
![enter image description here](https://i.imgur.com/q2g5BF1.png)

Na Secrets page é possível verificar somente o segredo, e não qual usuário realizou cada postagem.
## Commits

Nos commits demonstro seis diferentes níveis de segurança de dados para uma aplicação:

## Level 1

O level 1 de segurança somente inclui uma checagem da dupla username:password inseridas pelo usuário com as duplas presentes no banco de dados.

## Level 2 

Adicionado encriptação nas senhas por meio do mongoose-encryption. No entanto, o seed "secret" ainda está disponível no código fonte.

(2.1). Adicionadas variáveis de environment para melhorar a segurança de código, deixando ocultas senhas, seeds e api keys.

## Level 3 

Foi realizado a troca de encrypt por seed por uma maneira ainda mais segura: Hashing. O hashing utilizado foi utilizando o pacote 'md5'.

## Level 4

Adicionado Salt á senha por meio da lib 'bcrypt', adicionando mais dificuldade á tentativa de um bruteforce hacking.

## Level 5

Utilizando a lib 'passport.js' foram adicionados cookies e controle de sessão de usuário.

## Level 6

No level 6 inseri autenticação por meio do Google OAuth 2.0, inserindo um botão para login via conta Google.
