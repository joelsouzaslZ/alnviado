# alnviado

Página simples para convidar usuários a um grupo do WhatsApp.

Descrição
- Página estática (único arquivo `index.html`) com botão para abrir o convite do WhatsApp, botão para copiar o link e comportamentos adaptativos para mobile/desktop.
- O site não pode forçar a entrada do usuário no grupo — apenas abre o link de convite; o usuário precisa confirmar no app.

Como testar localmente
1. Abrir `index.html` diretamente no navegador (funciona offline).
2. Ou executar um servidor local (recomendado) na pasta do projeto para simular hospedagem:

```pwsh
# no PowerShell
python -m http.server 8080
# e então abra http://localhost:8080
```

Notas importantes
- O link do convite está definido no próprio `index.html` (constante `INVITE`). Substitua-o se quiser outro grupo.
- Removido `grupowhatsapp.html`; todo o conteúdo foi consolidado em `index.html`.

Próximos passos possíveis
- Adicionar um workflow GitHub Actions para validação (HTML/CSS/JS) ou deploy automático (opcional).
- Incluir imagem/logo real em `assets/` e referenciar de forma relativa.

Licença
- Use livremente — este repositório contém apenas HTML estático.
