# Classificador de Crédito

App em React (Vite) que lê o relatório do Salesforce ("Avaliações de crédito da minha equipe") e classifica os casos por status.

## Como publicar (GitHub + Vercel)

### 1. Criar o repositório no GitHub
1. Entre em https://github.com e clique em **New repository**.
2. Dê um nome (ex: `classificador-credito`), marque como **Private** se quiser, e clique em **Create repository**.
3. No seu computador, dentro desta pasta, rode:
   ```bash
   git init
   git add .
   git commit -m "primeiro commit"
   git branch -M main
   git remote add origin https://github.com/SEU-USUARIO/classificador-credito.git
   git push -u origin main
   ```
   (troque `SEU-USUARIO` pelo seu usuário do GitHub — o GitHub mostra esse comando exato na página do repositório recém-criado, em "...or push an existing repository from the command line").

### 2. Publicar no Vercel
1. Entre em https://vercel.com e faça login com sua conta do GitHub.
2. Clique em **Add New -> Project**.
3. Selecione o repositório `classificador-credito` que você acabou de subir.
4. O Vercel já detecta que é um projeto Vite automaticamente (Build Command: `npm run build`, Output: `dist`). Não precisa mudar nada.
5. Clique em **Deploy** e aguarde cerca de 1 minuto.
6. Pronto -- você recebe uma URL tipo `https://classificador-credito.vercel.app` que já pode usar e compartilhar.

Depois disso, qualquer novo `git push` para o `main` gera um novo deploy automático.

## Rodar localmente (opcional, para testar antes de subir)
```bash
npm install
npm run dev
```
Abre em http://localhost:5173
