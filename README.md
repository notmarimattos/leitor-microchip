# Leitor de Microchip (teste)

Protótipo de leitor do código de barras (Code 128) das etiquetas de microchip, para evitar a digitação
manual dos 15 dígitos. Página única, sem servidor e sem login.

**Abrir:** https://notmarimattos.github.io/leitor-microchip/

## Como usar

1. No PC, abra o link e clique na aba **Celular como leitor**: aparece um QR e um código de 6 letras.
2. No celular, abra o mesmo link (Chrome ou Safari). Ele já abre em **Enviar para o PC**: aponte a câmera
   para o QR da tela do PC (ou digite o código).
3. Quando aparecer **Conexão concluída** nos dois lados, cada etiqueta lida no celular chega ao PC já copiada —
   é só colar com Ctrl+V no campo do número do microchip.

Também dá para usar a webcam do próprio PC (aba **Câmera deste computador**) ou, no celular sem PC por perto,
o link discreto **Ler e copiar aqui**.

## Leitura

Três decodificadores, do melhor para o pior: o leitor nativo do navegador (BarcodeDetector, Chrome no Android),
o ZXing C++ em WebAssembly (embutido no arquivo) e o ZXing em JavaScript. A câmera é pedida em 1080p com foco
contínuo; quando o aparelho permite, o zoom começa em 2× (ajustável) e há botão de lanterna.

Dica: aproxime até as barras preencherem o quadro; se a imagem ficar tremida, afaste 1–2 cm para focar.

## Canal celular ↔ PC

Tópico aleatório no ntfy.sh (serviço público, sem conta), identificado só pelo código de 6 letras.
Só o número do chip trafega.

Versão 2.3.
