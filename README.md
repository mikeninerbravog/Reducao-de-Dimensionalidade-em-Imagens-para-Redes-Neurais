# Projeto de Prova de Conceito (POC) - Bootcamp DIO

## Aluno: Marcello S Bastos
### Bootcamp: Machine Learning Practitioner - Fevereiro de 2025
### Prova: Redução de Dimensionalidade em Imagens para Redes Neurais

Este projeto realiza a conversão de uma imagem colorida para escala de cinza e, em seguida, para preto e branco (binário). A redução de dimensionalidade facilita o treinamento de redes neurais, tornando o modelo mais eficiente.

## Requisitos:
- Google Colab
- Conta no Google Drive
- Biblioteca Pillow (PIL)

## Objetivos:
1. Carregar uma imagem a partir do Google Drive
2. Converter para escala de cinza
3. Converter para preto e branco (binarização)
4. Salvar as versões processadas no Google Drive

## Como Executar:
1. Faça upload da imagem (lenna2.jpg) no seu Google Drive, no caminho `/MyDrive/dio/`
2. Cole o código Python em uma célula do Google Colab
3. Execute a célula
4. Verifique os arquivos gerados no Google Drive (`escaladecinza.jpg` e `PB.jpg`)

## Explicação das Etapas:
- **Escala de Cinza:** Converte a imagem para tons de cinza usando a fórmula de luminância padrão:
  `gray = 0.299*R + 0.587*G + 0.114*B`
- **Preto e Branco:** Realiza binarização aplicando um limiar (threshold) fixo. 
  `bw = 255 if gray > 128 else 0`

## Impacto na Redução de Dimensionalidade:
- Reduz o número de canais (de 3 para 1)
- Diminui a complexidade computacional
- Facilita a detecção de padrões essenciais para redes neurais

## Resultados Esperados:
- `escaladecinza.jpg`: Imagem em tons de cinza
- `PB.jpg`: Imagem em preto e branco binária
