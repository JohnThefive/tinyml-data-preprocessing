# tinyml-data-preprocessing
Processamento e preparação do MRL Eye Dataset para aplicações de TinyML. O projeto realiza download via KaggleHub, classificação de imagens em olhos abertos e fechados, conversão para escala de cinza, redimensionamento para 96×96 pixels e processamento paralelo para otimizar a preparação do dataset.

## O que este projeto faz?

Este projeto realiza o pré-processamento do **MRL Eye Dataset**, disponibilizado no Kaggle, para preparação de imagens destinadas a aplicações de **TinyML**. O pipeline identifica e classifica imagens de olhos **abertos** e **fechados**, converte as imagens para escala de cinza e redimensiona todas para **96×96 pixels**, organizando-as automaticamente em diretórios por classe.

## Quais ferramentas foram usadas?

* **Python**
* **OpenCV (cv2)** para processamento e redimensionamento das imagens
* **KaggleHub** para download e gerenciamento do dataset
* **ProcessPoolExecutor** para processamento paralelo das imagens
* **Pathlib** para gerenciamento de arquivos e diretórios
* **TQDM** para acompanhamento do progresso do processamento

## Quais foram os resultados ou aprendizados?

O pipeline gera um dataset estruturado em duas classes, **abertos** e **fechados**, com imagens padronizadas em **96×96 pixels** e escala de cinza, facilitando sua utilização no treinamento de modelos de classificação para TinyML. O uso de processamento paralelo também permite otimizar a etapa de preparação de grandes volumes de imagens, reduzindo o tempo necessário para o pré-processamento do dataset.
