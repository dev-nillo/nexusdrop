# NexusDrop - Vitrine da Loja

Site estático (HTML) da loja, com o banco de dados no Supabase.

## Arquivos
- `index.html`  - vitrine (catálogo, busca, carrinho, checkout por WhatsApp)
- `produto.html` - página de detalhe do produto
- `Logo/`       - imagens da marca (opcional)

## Como publicar no GitHub Pages
1. Crie um repositório **público** no GitHub (ex.: `nexusdrop-loja`).
2. Envie estes arquivos para a branch `main`:
   ```
   git init
   git add .
   git commit -m "Vitrine NexusDrop"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/nexusdrop-loja.git
   git push -u origin main
   ```
3. No repositório: **Settings > Pages**.
4. Em *Source*, escolha **Deploy from a branch** > branch **main** > pasta **/(root)** > **Save**.
5. Em ~1 minuto o site fica em:
   `https://SEU-USUARIO.github.io/nexusdrop-loja/`

## Importante
- O painel de administração (**admin/**) e o código do servidor (**api/**)
  **não** fazem parte deste repositório, de propósito.
- A chave que aparece no HTML é a chave **pública** do Supabase
  (projetada para ser pública). A segurança dos dados é garantida pelas
  políticas de acesso (RLS) no banco.
