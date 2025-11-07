# Mayabia — Calculadora Final
Este repositório contém uma **web app PWA** simples (demo) pronta para publicar no **GitHub Pages** e usar no **Median** para gerar uma app Android.

## Conteúdo
- `index.html` — Single-page app (login com localStorage, calculadora, estimativa do fim do mundo).
- `manifest.json` — Manifest PWA.
- `service-worker.js` — Service worker para cache offline simples.
- `icons/icon-192.png`, `icons/icon-512.png` — Ícones gerados.
- `README.md` — este ficheiro.

## Publicar no GitHub Pages
1. Crie um repositório no GitHub (p.ex. `mayabia-app`) e copie os ficheiros para a branch `main`.
2. No GitHub: `Settings` → `Pages` → escolha `main` branch e `/ (root)` e salve.
3. Aguarde alguns minutos e abra `https://<seuusuario>.github.io/<seurepo>/`.
4. Verifique se `manifest.json` e `service-worker.js` estão acessíveis via HTTPS (p.ex. `https://.../manifest.json`).

## Testar PWA
- Abra a URL no Chrome e abra DevTools → Lighthouse → PWA para ver sugestões.
- Tente `Adicionar à tela inicial` no Chrome (Android) para testar instalabilidade.

## Usar no Median
- No Median App Studio cole a URL pública do GitHub Pages (HTTPS).
- Configure ícones/splash se necessário (os ícones estão prontos em `icons/`).
- Gere o APK/AAB. Para publicação no Google Play será necessária uma conta de desenvolvedor e assinatura do app.

## Notas importantes
- Esta implementação usa **localStorage** para autenticação (apenas demo). Para produção, implemente um backend seguro.
- Recursos como Push Notifications e algumas APIs podem precisar de configurações adicionais.

