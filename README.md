
# Projeto de Detecção e Rastreamento de Carros de Fórmula E

---

## Desenvolvedores

- **Camila Feitosa** - RM: 558808
- **Gabriel Matiolli** - RM: 558963
- **Gustavo Berlanga** - RM: 555298
- **Leonardo Taschin** - RM: 554583
- **Vinicius Gardim** - RM: 556013

---

## Descrição do Projeto

Este projeto tem como objetivo realizar o rastreamento dos carros de Fórmula E utilizando o modelo de detecção YOLO (You Only Look Once). A partir da detecção dos carros, o objetivo final é estimar a velocidade dos veículos em tempo real para visualização dos telespectadores, proporcionando uma experiência mais imersiva e informativa durante as corridas.

## Instruções de Uso

1. **Clone o Repositório**: Clone o repositório do projeto em seu ambiente local.
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd <NOME_DO_REPOSITORIO>
   ```

2. **Instale as Dependências**: Utilize o gerenciador de pacotes `pip` para instalar as dependências necessárias.
   ```bash
   pip install ultralytics
   pip install supervision==0.1.0
   ```

3. **Prepare os Arquivos Necessários**:
   - Coloque o vídeo a ser analisado no diretório do projeto com o nome `formulaeexample.mp4`.
   - Certifique-se de ter o arquivo de pesos do modelo YOLO compactado em `weights.zip`.

4. **Execute o Script**: No terminal, execute o script Python para iniciar o processo de detecção e rastreamento.
   ```bash
   python detectar_objetos.py
   ```

## Requisitos

- **Sistema Operacional**: Windows, macOS ou Linux.
- **Python**: Versão 3.6 ou superior.
- **Pacotes**:
  - `ultralytics`
  - `supervision==0.1.0`
- **GPU**: Recomendado uma GPU NVIDIA para melhor desempenho na detecção e rastreamento em tempo real.

## Detalhes Técnicos

- **Modelo de Detecção**: Utiliza o modelo YOLO da biblioteca `ultralytics` para realizar a detecção dos carros.
- **Rastreamento**: O modelo faz a fusão dos resultados para otimizar a detecção contínua dos carros no vídeo.
- **Estimativa de Velocidade**: A estimativa de velocidade é feita com base na detecção dos carros em diferentes frames do vídeo, calculando a distância percorrida em um intervalo de tempo.

## Dependências

- `ultralytics`: Biblioteca que contém o modelo YOLO utilizado para detecção de objetos.
- `supervision`: Utilizado para gerenciar as versões e dependências do projeto.

## Informações Relevantes

- Certifique-se de que os caminhos para os arquivos de vídeo e pesos do modelo estejam corretos no script.
- O script verifica a disponibilidade de uma GPU NVIDIA para garantir que o processamento seja eficiente.
- Após a descompactação dos pesos e a verificação das versões, o script executa o modelo no vídeo especificado com um nível de confiança ajustável.

## Estrutura do Projeto

```
.
├── detectar_objetos.py
├── formulaeexample.mp4
└── weights.zip
```

## Equipe E-fficency



---
```

https://colab.research.google.com/drive/1XDqwvis_Reoua8H_EQg6yolizbnSer-8?usp=sharing
