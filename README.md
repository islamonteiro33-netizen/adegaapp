# Chama Bebidas Adega

App da Adega em Expo/React Native, pronto para build Android no Codemagic.

## Rodar localmente

```bash
npm install
npx expo start
```

## Gerar APK no Codemagic

1. Suba essa pasta para um repositório no GitHub.
2. Conecte o repositório no Codemagic.
3. Escolha o workflow `android-apk`.
4. Rode o build.
5. O APK sairá em `android/app/build/outputs/apk/release/app-release.apk`.

## API usada

O app aponta para:

```txt
https://chamabebidas.com.br/api
```

Rotas esperadas:

```txt
GET   /api/stores
POST  /api/stores/login
GET   /api/stores/:storeId/orders
PATCH /api/orders/:orderId/status
```

Se a API ainda não tiver pedidos, o app abre mesmo assim e mostra uma lista de exemplo.
