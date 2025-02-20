# Portfólio de Reconhecimento de Texto

## Estrutura de Pastas
- **inputs**: Contém as imagens utilizadas para reconhecimento de texto.
- **output**: Contém os resultados de reconhecimento de texto das imagens.

## Processo
1. **Carregamento das Imagens:**
   - As imagens foram carregadas da pasta `inputs`.
2. **Reconhecimento de Texto:**
   - Utilizamos a biblioteca `OCR` para realizar o reconhecimento de texto nas imagens.
   - Os resultados foram salvos na pasta `output`.

## Exemplos de Código
```python
import ocr_library

# Carregar imagem
imagem = ocr_library.load_image('inputs/exemplo.png')

# Realizar reconhecimento de texto
texto = ocr_library.recognize_text(imagem)

# Salvar resultado
with open('output/resultado.txt', 'w') as f:
    f.write(texto)
