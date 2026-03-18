# Como publicar o app — Passo a passo completo

## ⚡ Mais rápido: GitHub Pages (10 minutos)

### 1. Criar conta no GitHub
Acesse github.com → "Sign up" → crie uma conta gratuita

### 2. Criar repositório
- Clique em "New repository"
- Nome: `osasco-express-app`
- Visibilidade: Public (para GitHub Pages gratuito)
- Clique "Create repository"

### 3. Subir os arquivos
**Opção A — Interface web (mais fácil):**
- Abra o repositório criado
- Arraste todos os arquivos do projeto para a tela
- Clique "Commit changes"

**Opção B — Terminal:**
```bash
cd osasco-express-app
git init
git add .
git commit -m "primeiro commit"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/osasco-express-app.git
git push -u origin main
```

### 4. Ativar GitHub Pages
- Vá em Settings → Pages
- Source: "Deploy from a branch"
- Branch: main / root
- Save

### 5. Acessar no celular
Após ~2 minutos: `https://SEU-USUARIO.github.io/osasco-express-app/src/`

**No iPhone:** Safari → compartilhar → "Adicionar à Tela de Início"
**No Android:** Chrome → menu (⋮) → "Adicionar à tela inicial"

---

## 📱 App Store e Play Store (leva mais tempo)

### Pré-requisitos de contas
- **Apple Developer Account**: USD 99/ano → developer.apple.com
- **Google Play Developer Account**: USD 25 único → play.google.com/console

### Processo resumido

1. Siga os passos do README para gerar o app nativo com Capacitor
2. No Xcode (iOS): Archive → Distribute App → App Store Connect
3. No Android Studio: Build → Generate Signed APK → Upload no Play Console
4. Preencher fichas das lojas (ícone, screenshots, descrição)
5. Aguardar revisão: iOS ~1-3 dias, Android ~1-7 dias

### Screenshots necessários
Tire prints das telas do app em:
- iPhone (6.5" e 5.5"): obrigatório para App Store
- Android (phone): obrigatório para Play Store

---

## 🔑 Domínio próprio (opcional)

Se quiser `app.osascoexpress.com.br` em vez do link do GitHub:

1. Configure DNS do seu domínio para apontar para GitHub Pages
2. Em Settings → Pages → Custom domain: `app.osascoexpress.com.br`
3. Marque "Enforce HTTPS"

---

## ✅ Checklist antes de publicar

- [ ] Ícones criados (192x192 e 512x512 px) em `public/icons/`
- [ ] README atualizado com informações corretas
- [ ] Testado no celular via GitHub Pages
- [ ] Tabela de preços atualizada (validade março/2026)
- [ ] CNPJ e dados do contrato corretos
