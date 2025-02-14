# Projeto de Prova de Conceito (POC) - Bootcamp DIO

## Aluno: Marcello S Bastos
### Bootcamp: Machine Learning Practitioner - Fevereiro de 2025
### Prova: Redução de Dimensionalidade em Imagens para Redes Neurais

Este projeto converte uma imagem colorida para escala de cinza e depois para preto e branco (binário). O objetivo é demonstrar a redução de dimensionalidade, facilitando o treinamento de redes neurais.

## Requisitos:
- Python 3
- Biblioteca Pillow (PIL)

## Objetivos:
1. Carregar a imagem `lenna2.jpg` (mesma pasta do script)
2. Converter para escala de cinza
3. Converter para preto e branco
4. Salvar as versões processadas no mesmo diretório

## Como Executar:
1. Coloque `lenna2.jpg` no mesmo diretório do script
2. Execute o script Python
3. Verifique os arquivos gerados (`escaladecinza.jpg` e `PB.jpg`)

## Explicação das Etapas:
- **Escala de Cinza:** Converte com a fórmula de luminância padrão:
  `gray = 0.299*R + 0.587*G + 0.114*B`
- **Preto e Branco:** Realiza binarização com limiar fixo:
  `bw = 255 if gray > 128 else 0`

## Impacto na Redução de Dimensionalidade:
- Reduz de 3 canais para 1 canal
- Diminui o custo computacional
- Facilita a extração de padrões para redes neurais

## Resultados Esperados:
- `escaladecinza.jpg`: Imagem em tons de cinza
- `PB.jpg`: Imagem binária (preto e branco)
