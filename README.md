PlayAuth
========

Exemplo básico de uma aplicação play com autenticação e multiusuário.

> Resumo

Um aplicação multiusuário significa que a aplicação permitirá que um ou mais usuários possam estar conectados ao sistema simultaneamente sem haver conflito de informações.

O exemplo mostra como usar Session para ajudar a controlar esse tráfego de usuários.

Ao criar uma session no play pelo código 

```sh 
session("<chave>", <valor>);
```
Alocamos para a memória do servidor(de forma não permanete) o dito valor relacionado a dita chave, de forma que essa session esteja estritamente relacionada com o browser do cliente. Assim, mesmo que o cliente feche a aba ou browser ao reiniciar a aplicação a sessão ainda estará ativa. E se outro usuário em outro computador acessar a plicação terá também sua própria Session no servidor.

> Observações

- Uma Session ao contrário do Cookie só pode ser acessada no servidor
- Para limpar a Session usamos o comando 
```sh
session().clear();
```
- Para acessar um valor na Session usamos
```sh
session().get("<chave>")
```



