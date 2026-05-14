# Como gerar o APK pelo celular usando GitHub

Este projeto já vem com GitHub Actions configurado para gerar o APK automaticamente.

## Pelo celular

1. Entre em https://github.com pelo navegador.
2. Crie uma conta ou faça login.
3. Crie um novo repositório, por exemplo: `integro-office-apk`.
4. Envie todos os arquivos deste projeto para o repositório.
   - Se o GitHub pelo celular dificultar enviar pasta inteira, use o app do GitHub ou faça pelo navegador em modo desktop.
5. Depois de enviar, toque na aba **Actions**.
6. Escolha **Gerar APK Android**.
7. Toque em **Run workflow**.
8. Aguarde alguns minutos.
9. Quando finalizar, abra a execução.
10. Baixe o arquivo em **Artifacts** chamado **INTEGRO-Office-APK**.
11. Extraia o ZIP baixado.
12. Instale o APK no Android.

## Onde fica o APK depois que o GitHub gerar

Dentro do artifact, procure por:

`app-debug.apk`

## Observação

Android Studio não roda oficialmente no Android comum. Este método usa os servidores do GitHub para compilar o APK.
