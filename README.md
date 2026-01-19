# Tchê Levo - Página de Redirecionamento

Esta página detecta Android ou iOS e redireciona para a loja correta do app
Tchê Levo. Também exibe uma tela mobile com o ícone e o destino.

## Como funciona
- Detecta o sistema operacional do dispositivo.
- Redireciona automaticamente para a App Store ou Google Play.
- Mostra botões para abrir manualmente as lojas.

## Onde editar os links das lojas
Os links ficam no início do script do `index.html`:

```html
<script>
  // Links de download (edite aqui se mudar).
  const APP_STORE_URL = "https://apps.apple.com/br/app/tch%C3%AA-levo/id1529677708";
  const PLAY_STORE_URL = "https://play.google.com/store/apps/details?id=br.com.tchelevo.passenger.drivermachine";
</script>
```

## Preview no WhatsApp (imagem acima do link)
Para o WhatsApp exibir a logo, edite as metas Open Graph em `index.html`
substituindo `SEU_DOMINIO` pelo endereço público desta página:

```html
<meta property="og:image" content="https://tchelevo.valedata.com.br/images/tchelevo.png" />
<meta property="og:url" content="https://tchelevo.valedata.com.br//" />
```

## Estrutura de arquivos
- `index.html`: página principal de redirecionamento.
- `images/tchelevo.png`: ícone do app.

## Como usar
1. Publique este diretório em um servidor web.
2. Acesse o link da página pelo celular.
3. O redirecionamento acontece automaticamente.

## Créditos
Desenvolvido por Almir Bolduan
