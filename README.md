# Kanban por Épicos - Folha X

Dashboard Kanban em tempo real com dados do Azure DevOps para o projeto HCM - Senior / Folha X.

## Como acessar

Acesse o link: **[inserir URL do GitHub Pages aqui]**

> Exemplo: `https://seuusuario.github.io/kanban-folhax/`

## Primeiro acesso - Gerar sua PAT

Na primeira vez, a página pedirá sua **Personal Access Token (PAT)** do Azure DevOps.

### Passo a passo para gerar a PAT:

1. Acesse [Azure DevOps → Personal Access Tokens](https://dev.azure.com/senior-sistemas/_usersSettings/tokens)
2. Clique em **+ New Token**
3. Preencha:
   - **Name:** Kanban Folha X (ou o nome que preferir)
   - **Organization:** senior-sistemas
   - **Expiration:** escolha o prazo desejado (máx. 1 ano)
   - **Scopes:** clique em "Custom defined" e marque **Read** em "Work Items"
4. Clique em **Create**
5. **Copie o token gerado** (ele só aparece uma vez!)
6. Cole na página do Kanban e clique **Entrar**

### Após o primeiro acesso

- O token fica salvo no seu navegador (localStorage)
- Não será pedido novamente até expirar ou você clicar em "Trocar PAT"
- Se mudar de navegador ou limpar os dados, será pedido novamente

## Segurança

- ⚠️ **Cada pessoa deve gerar sua própria PAT** — não compartilhe tokens
- O token fica salvo apenas no SEU navegador, não é enviado a nenhum servidor
- Use o escopo mínimo: apenas **Read** em "Work Items"
- Defina uma data de expiração adequada

## Para desenvolvedores - Como publicar

### GitHub Pages

1. Crie um repositório no GitHub (pode ser público — a página só funciona com PAT válida)
2. Faça push dos arquivos (`index.html`)
3. Vá em **Settings > Pages**
4. Source: Deploy from branch `main` / `/ (root)`
5. Em ~1 min o site fica disponível

### Atualizar o dashboard

Basta fazer push de uma nova versão do `index.html` para a branch `main`.
