# WAP Produção DelMORO v2

## Como rodar
Use um servidor local (recomendado):
- VSCode: Live Server
- Ou: `python -m http.server 5500`

## O que mudou nesta v2
- Cards de produtos no estilo “tile”: só imagem + nome + cod. balança.
- Removido “OK” bugado em cima do card antigo.
- Exemplo do Pão Caseiro já vem com imagem (./assets/pao-caseiro.png).

## Controle de acesso (Produção x Admin)
- Por padrão (sem login), o app abre em **modo Produção**: mostra apenas a aba **🍞 Produção**.
- Para liberar **🧾 Vendas / 📈 Histórico / ⚙️ Config**, faça login em **Acesso admin**.

### Como marcar um usuário como admin
No Firebase Realtime Database, crie o caminho:
`admins/<UID_DO_USUARIO> = true`

> Dica: você encontra o UID no Firebase Authentication.
