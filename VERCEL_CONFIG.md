# Configurar packpicante.online na Vercel (só você pode fazer)

O projeto já está pronto. Falta só isso **no site da Vercel** (você precisa estar logado):

---

## Passo 1 – Abrir o projeto
1. Acesse **https://vercel.com/dashboard**
2. Clique no projeto (ex.: **packpicana** ou o nome que aparecer)

---

## Passo 2 – Conferir o repositório
1. Clique em **Settings** (Configurações)
2. No menu da esquerda, clique em **Git**
3. Veja qual repositório está conectado (ex.: `seu-usuario/pack-r3d`)
4. **Importante:** no GitHub, a raiz desse repositório precisa ter **index.html** e a pasta **assets**.  
   Se no GitHub a raiz tiver uma pasta **extracted** e o index.html estiver dentro dela, vá no **Passo 3**.  
   Se o **index.html** já estiver na raiz do repositório, pule para o **Passo 4**.

---

## Passo 3 – Root Directory (só se o index.html estiver dentro de "extracted")
1. Ainda em **Settings**
2. No menu da esquerda, clique em **General**
3. **Role a página até o final**
4. Procure **"Root Directory"** ou **"Repository Root"**
5. Clique em **Edit** (se tiver)
6. Digite: **extracted**
7. Clique em **Save**

*(Se não achar "Root Directory", pode estar em **Settings → Git**, na parte de configuração do repositório.)*

---

## Passo 4 – Fazer um novo deploy
1. No menu do projeto, clique em **Deployments** (Implantações)
2. No último deployment da lista, clique nos **três pontinhos** (⋮)
3. Clique em **Redeploy**
4. Marque **Use existing Build Cache** (ou deixe como estiver) e confirme **Redeploy**
5. Espere terminar (alguns segundos)

---

## Passo 5 – Domínio packpicante.online
1. Vá em **Settings** → **Domains**
2. Se **packpicante.online** já estiver na lista, ótimo
3. Se não estiver, clique em **Add** e digite: **packpicante.online** → **Add**
4. Siga as instruções de DNS que a Vercel mostrar (no lugar onde você gerencia o domínio)

---

## Depois disso
Abra **https://packpicante.online** no navegador. Se ainda der 404, espere 1–2 minutos e teste de novo (cache/DNS).
