# Processamento Digital de Imagens (Digital Image Processing)

Este repositório contém implementações de diversos algoritmos de processamento de imagens, desenvolvidos como parte da disciplina de **Processamento Digital de Imagens** do curso de **Sistemas de Informação** da **Universidade Federal de Viçosa - Campus Rio Paranaíba (UFV-CRP)**.

## Sobre o Projeto

O projeto visa demonstrar de forma prática os conceitos aprendidos em sala de aula, cobrindo tópicos fundamentais como transformações de intensidade, filtragem espacial, segmentação e detecção de bordas. Cada diretório contém o script Python do algoritmo e imagens de exemplo para teste.

**Professor:** Joao Mari

**Autores:**
- MatheusRV (3929)
- iguit0 (3902)
- ThiagoMunich (3628)

## Estrutura do Projeto

Abaixo está a estrutura de diretórios do projeto, organizada por tópicos da disciplina:

```
algorithms
├── 1 - Fundamentals of Digital Imaging
│   ├── aritm
│   │   ├── aritm.py
│   │   ├── img_1.tif
│   │   ├── img_2.tif
│   │   └── saida.tif
│   └── logic
│       ├── img_1.tif
│       ├── img_2.tif
│       ├── logic.py
│       └── saida.tif
├── 2 - Intensity Transformations
│   ├── 1 - Negative of An Image
│   │   ├── img_1.tif
│   │   ├── neg.py
│   │   └── saida.tif
│   ├── 2 - Gama Transformation
│   │   ├── gama.py
│   │   ├── img_1.tif
│   │   └── saida.tif
│   ├── 3 - Contrast Widening
│   │   ├── cont.py
│   │   ├── img_1.tif
│   │   └── saida.tif
│   ├── 4 - Histograms Building
│   │   ├── hist.py
│   │   ├── histograma.tif
│   │   └── img_1.tif
│   └── 5 - Histogram Equalization
│       ├── eq.py
│       ├── img_1.tif
│       └── saida.tif
├── 3 - Spatial filtering for smoothing
│   ├── 1 - Media Filter
│   │   ├── img_1.tif
│   │   ├── img_2.tif
│   │   └── media.py
│   ├── 2 - Gaussian Filter
│   │   ├── gaus.py
│   │   ├── img_1.tif
│   │   └── img_2.tif
│   ├── 3 - Median Filter
│   │   ├── img_1.tif
│   │   ├── img_2.tif
│   │   └── med.py
│   └── 4 - Max Min Filter
│       ├── img_1.tif
│       ├── img_2.tif
│       └── maxmin.py
├── 4 - Spatial filtering for sharpening
│   ├── 1 - Laplacian
│   │   ├── img_1.tif
│   │   ├── img_2.tif
│   │   └── lap.py
│   ├── 2 - Sharpness high-boost mask
│   │   ├── img_1.tif
│   │   ├── img_2.tif
│   │   └── nit.py
│   └── 3 - Gradient
│       ├── grad.py
│       ├── img_1.tif
│       └── img_2.tif
├── 5 - Segmentation Edge Detection
│   ├── 1 - Smoothing Edge Detection Effects
│   │   ├── bordas_s.py
│   │   ├── img_1.tif
│   │   └── saida.tif
│   └── 2 - Smoothing and Thresholding Effects on Edge Detection
│       ├── bordas_l.py
│       ├── img_1.tif
│       └── saida.tif
├── 6 - Segmentation Thresholding
│   ├── 1 - Iterative Threshold
│   │   ├── img_1.tif
│   │   ├── lim_it.py
│   │   └── saida.tif
│   ├── 2 - Otsu
│   │   ├── img_1.tif
│   │   ├── otsu.py
│   │   └── saida.tif
│   └── 3 - Effect of smoothing on thresholding
│       ├── img_1.tif
│       ├── lim_s.py
│       └── saida.tif
```

## Pré-requisitos

Para executar os scripts, você precisará de Python instalado e das seguintes bibliotecas:

- `numpy`
- `matplotlib`
- `scipy`
- `scikit-image`

Nota: Alguns scripts utilizam `scipy.misc.imread` e `imsave`, que foram depreciados em versões mais recentes do SciPy. Pode ser necessário ajustar o código para usar `imageio.imread` ou instalar uma versão compatível do SciPy/Pillow.

## Como Executar

Navegue até o diretório do algoritmo desejado e execute o script Python. A maioria dos scripts espera o nome da imagem de entrada e o nome do arquivo de saída como argumentos.

Exemplo para executar o "Negativo de uma Imagem":

```bash
cd "algorithms/2 - Intensity Transformations/1 - Negative of An Image"
python neg.py img_1.tif saida
```

Verifique o cabeçalho de cada arquivo `.py` para instruções específicas de uso.
