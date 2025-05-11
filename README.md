# diagrama servico login

Fluxo:
- Usuário pede acesso ao login para compra do ingresso.
- Sistema adiciona o usuário numa fila(mutex queue).
- Quando for a vez do usuário o sistema retorna um token de acesso
- Usuário acessa página e realiza a compra do ingresso.
- Número de ingressos é atualizado, bem como de token permitidos para compra de ingresso do show.
