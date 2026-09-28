# Portfólio — Pedro Peretti Guimarães

Site estático (HTML puro, sem build, sem dependências de servidor). Pronto para publicar no **GitHub Pages**, de graça.

## Passo a passo (sem usar terminal)

1. **Crie uma conta no GitHub**, se ainda não tiver: https://github.com/join

2. **Crie um repositório novo**: https://github.com/new
   - Nome do repositório: `SEU-USUARIO.github.io` (troque `SEU-USUARIO` pelo seu nome de usuário do GitHub, exatamente igual). Esse nome especial faz o site sair direto em `https://SEU-USUARIO.github.io`, sem sufixo.
   - Deixe como **Public**.
   - Não marque nenhuma opção de "adicionar README" — deixe o repositório vazio.
   - Clique em **Create repository**.

3. **Suba os arquivos**: na página do repositório recém-criado, clique em **"uploading an existing file"** (ou "Add file" → "Upload files").
   - Arraste para dentro do navegador: `index.html`, `README.md`, e a pasta `projects` (arraste a pasta inteira, o GitHub aceita). Todas as fotos, vídeos e o currículo já estão embutidos dentro do próprio `index.html`, não precisa de mais nada.
   - Espere o upload terminar (o `index.html` é o arquivo mais pesado, pode demorar um pouco).
   - Escreva uma mensagem de commit qualquer (ex: "primeira versão") e clique em **Commit changes**.

4. **Ative o GitHub Pages**:
   - Vá em **Settings** (do repositório) → **Pages** (menu à esquerda).
   - Em "Build and deployment" → "Source", selecione **Deploy from a branch**.
   - Em "Branch", selecione `main` e a pasta `/ (root)`. Clique em **Save**.
   - Aguarde 1–2 minutos. O GitHub mostra o link do site no topo dessa mesma página quando terminar.

Pronto — o site está no ar, de graça, para sempre, em `https://SEU-USUARIO.github.io`.

## Quando tiver o domínio próprio (`.me` do GitHub Student Pack)

1. Em **Settings → Pages**, no campo **Custom domain**, digite o domínio (ex: `pedroperetti.me`) e salve. Isso cria um arquivo `CNAME` no repositório automaticamente.
2. No painel da Namecheap (onde o domínio foi registrado), configure os registros DNS apontando para o GitHub:
   - Um registro **A** apontando para cada um destes IPs: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`.
   - Um registro **CNAME** para `www` apontando para `SEU-USUARIO.github.io`.
3. Volte em Settings → Pages e marque **Enforce HTTPS** quando a opção ficar disponível (leva algumas horas para o certificado ser emitido).

## Atualizando o site depois

Sempre que eu (Claude) te mandar uma nova versão, é só repetir o passo 3 (Upload files) substituindo os arquivos — o GitHub Pages publica a atualização automaticamente em 1–2 minutos.

## Alternativa via terminal (opcional, para quem já usa git)

```bash
git clone https://github.com/SEU-USUARIO/SEU-USUARIO.github.io.git
cd SEU-USUARIO.github.io
# copie index.html, README.md e projects/ para dentro desta pasta
git add -A
git commit -m "primeira versão"
git push
```
