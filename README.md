# INTEGRO Office WebView APK

Este projeto coloca o arquivo HTML dentro de um APK Android usando uma WebView nativa.

## O que está dentro
- `app/src/main/assets/www/index.html`: seu aplicativo HTML.
- `MainActivity.java`: abre o HTML dentro do Android.
- Permite abrir seletor de arquivos do Android.
- Permite abrir galeria pelo botão "Abrir Galeria".
- Permite abrir câmera pelo botão "Câmera".
- Mantém o gerenciador de arquivos, documento, planilha, apresentação e utilitários do HTML.

## Como gerar o APK pelo Android Studio
1. Instale o Android Studio.
2. Abra o Android Studio.
3. Clique em **Open** e escolha esta pasta: `INTEGRO_Office_WebView_APK_Project`.
4. Aguarde o Gradle sincronizar.
5. Conecte seu celular Android com Depuração USB ativada, ou gere direto o APK.
6. Vá em **Build > Build App Bundle(s) / APK(s) > Build APK(s)**.
7. O APK ficará em: `app/build/outputs/apk/debug/app-debug.apk`.

## Como instalar no celular
- Envie o `app-debug.apk` para o Android.
- Ative a permissão de instalar apps desconhecidos, se o Android solicitar.
- Instale o APK.

## Observação sobre acesso livre aos arquivos
O Android moderno limita acesso total ao armazenamento por segurança. O app usa:
- seletor de arquivo;
- seletor de galeria;
- câmera;
- importação de arquivos;
- armazenamento interno do HTML.

Para acesso real irrestrito tipo gerenciador de arquivos profissional, é necessário evoluir o projeto com módulo nativo usando Storage Access Framework, MediaStore ou permissão especial MANAGE_EXTERNAL_STORAGE.
