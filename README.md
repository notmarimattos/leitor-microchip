# Leitor de Microchip
Protótipo de leitor de código de barras (Code 128) das etiquetas de microchip, para a tela
*Realizar Microchipagem* da Central. Página única, sem servidor e sem login.

**Abrir:** https://notmarimattos.github.io/leitor-microchip/

## Modos

1. **Câmera deste computador** – webcam do PC lê a etiqueta, bipa e copia os 15 dígitos; cole na Central com Ctrl+V.
2. **Celular como leitor** – o PC mostra um QR; o celular abre o mesmo link, lê o QR e cada etiqueta lida no celular aparece no PC já copiada (canal via ntfy.sh, só o número do chip trafega).

## Observações

- No iPhone, abra o link acima no Safari (arquivo local não tem acesso à câmera).
- Se o Chrome pedir, permita a câmera no cadeado ao lado do endereço.
- Bibliotecas embutidas: `@zxing/library` 0.21.3 e `qrcode-generator` 1.4.4.

Versão 2.1 · prova de conceito e especificação para o botão "Ler código de barras" na Central.
