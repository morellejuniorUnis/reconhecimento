# Detecção de Faces com OpenCV e Dlib

## Descrição
Este projeto realiza a detecção de faces em imagens estáticas usando as bibliotecas **OpenCV** e **Dlib**. Ele também compara a eficiência entre os dois métodos e implementa a detecção de **landmarks faciais** para destacar as expressões (olhos, nariz, boca, etc.) nas faces detectadas.

O código é executado em **Google Colaboratory** e foi projetado para aceitar upload de imagens diretamente na plataforma. Após o upload, ele aplica a detecção de faces e landmarks utilizando dois métodos distintos:
1. **OpenCV**: Usando o classificador Haar Cascade.
2. **Dlib**: Usando o modelo baseado em HOG (Histogram of Oriented Gradients).

## Abordagem Utilizada
O código foi dividido em diferentes funções para garantir modularidade e clareza:
- `detect_faces_image_opencv`: Detecta faces usando o classificador Haar Cascade do OpenCV.
- `detect_faces_image_dlib`: Detecta faces usando o detector de faces HOG do Dlib.
- `detect_landmarks_dlib`: Detecta landmarks faciais (pontos dos olhos, nariz, boca) usando Dlib.
- `compare_face_detection`: Compara a performance entre OpenCV e Dlib em termos de tempo de execução.

Além disso, foi implementada uma comparação direta entre os dois métodos (OpenCV e Dlib), onde é possível visualizar as diferenças em termos de tempo de execução e a acurácia na detecção.

## Como Executar o Código no Google Colab

### Passos:
1. Acesse o Google Colab e crie um novo notebook.
2. Copie o código do arquivo Python e cole no notebook do Colab.
3. Execute o primeiro bloco para instalar as dependências necessárias:
   ```python
   !pip install opencv-python dlib
