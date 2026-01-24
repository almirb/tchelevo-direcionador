# Tchê Levo - Website Oficial

Website oficial do Tchê Levo, seu aplicativo de mobilidade urbana. O site apresenta o app e oferece redirecionamento inteligente para download nas lojas iOS e Android.

## 🌐 Estrutura do Site

### Página Principal (`/`)

- Apresentação do aplicativo Tchê Levo
- Slogan: "Seu aplicativo de mobilidade urbana!"
- Características principais do serviço
- Botão para página de download
- Design moderno com glassmorphism e gradientes

### Página de Download (`/baixar/`)

- Detecção automática do sistema operacional (Android/iOS)
- Redirecionamento automático para a loja apropriada
- Botões manuais para App Store e Google Play
- Feedback visual do redirecionamento

## 📱 Como Funciona

### Página Principal

1. Apresenta o Tchê Levo com informações sobre o serviço
2. Exibe três características principais:
   - ⚡ Rápido e Prático
   - 🛡️ Seguro e Confiável
   - 💰 Preços Justos
3. Oferece botão para acessar a página de download

### Página de Download

1. Detecta automaticamente o sistema operacional do dispositivo
2. Redireciona para a App Store (iOS) ou Google Play (Android)
3. Exibe botões manuais caso o redirecionamento não funcione
4. Mostra visualmente o destino do redirecionamento

## ⚙️ Configuração

### Editar Links das Lojas

Os links das lojas ficam no arquivo `baixar/index.html`:

```javascript
const APP_STORE_URL = "https://apps.apple.com/br/app/tch%C3%AA-levo/id1529677708";
const PLAY_STORE_URL = "https://play.google.com/store/apps/details?id=br.com.tchelevo.passenger.drivermachine";
```

### Meta Tags Open Graph

As meta tags já estão configuradas para compartilhamento em redes sociais:

```html
<meta property="og:image" content="https://tchelevo.app.br/images/tchelevo.png" />
<meta property="og:url" content="https://tchelevo.app.br/" />
<meta property="og:title" content="Tchê Levo - Mobilidade Urbana" />
<meta property="og:description" content="Seu aplicativo de mobilidade urbana!" />
```

## 📁 Estrutura de Arquivos

```
tchelevo/
├── index.html              # Página principal do site
├── baixar/
│   └── index.html         # Página de redirecionamento
├── images/
│   ├── tchelevo.png       # Logo/ícone do app
│   ├── qrcode_valedata.png
│   └── qrcode_valedata.svg
└── README.md              # Este arquivo
```

## 🎨 Design

- **Fonte Display**: Bebas Neue
- **Fonte Corpo**: Sora
- **Cores Principais**:
  - Ink (Fundo escuro): `#0f2d2e`
  - Accent (Destaque): `#ffb13c`
  - Teal (Acento): `#10c8a8`
  - Paper (Texto): `#fff6e8`
- **Efeitos**: Glassmorphism, gradientes radiais, grid pattern

## 📱 Compatibilidade

- ✅ iOS (Safari)
- ✅ Android (Chrome)
- ✅ Responsivo para todos os tamanhos de tela
- ✅ PWA-ready (meta tags iOS configuradas)
- ✅ Open Graph para redes sociais

## 📄 Licença

© 2026 [Ezedy](https://ezedy.com) - Todos os direitos reservados
