
&nbsp;
&nbsp;
<p align="center">
  <img width="800" src="./figures/conecta_logo.png" />
</p> 

&nbsp;

# 🧠 TEDA Bootcamp — IEEE UFRN 2025

Este repositório contém o material prático do curso **Bootcamp TEDA** ministrado para o público de Engenharia Elétrica na **UFRN** durante o evento **IEEE 2025**.  
O objetivo é apresentar, de forma prática e didática, o uso do algoritmo **TEDA** para detecção de anomalias em séries temporais de consumo energético.

## 📂 Estrutura do Repositório

```
.
├── TEDA_Demo_Bootcamp.ipynb   # Notebook principal com explicações e código
├── teda.py                    # Implementação do algoritmo TEDA
├── lead1.0-small.csv          # Dataset de consumo energético
├── README.md                  # Este arquivo
└── figures/                   # Resultados gerados (gráficos, CSVs)
```

## 📋 Pré-requisitos

- Python 3.8+
- Pacotes listados em `requirements.txt`:
  ```bash
  pip install pandas numpy matplotlib scikit-learn
  ```

## 🚀 Como Executar Localmente

1. **Clone este repositório**:
   ```bash
   git clone https://github.com/conect2ai/TEDA-Bootcamp.git
   cd TEDA-Bootcamp
   ```

2. **Instale as dependências**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Abra o notebook no Jupyter**:
   ```bash
   jupyter notebook TEDA_Demo_Bootcamp.ipynb
   ```

4. **Execute as células sequencialmente** para:
   - Carregar e pré-processar os dados
   - Aplicar o TEDA
   - Visualizar as anomalias
   - Avaliar métricas e sensibilidade do parâmetro `m`

## ☁️ Executando no Google Colaboratory

1. Acesse: [Google Colaboratory](https://colab.research.google.com/)
2. Clique em **Arquivo → Carregar notebook**
3. Envie o arquivo `TEDA_Demo_Bootcamp.ipynb`
4. Também envie os arquivos `teda.py` e `lead1.0-small.csv` para a área de arquivos do Colab (painel à esquerda).
5. Execute as células na ordem.

💡 *Dica:* Você também pode abrir o notebook diretamente do GitHub no Colab clicando no link:
```
https://colab.research.google.com/github/conect2ai/TEDA-Bootcamp/blob/main/TEDA_Demo_Bootcamp.ipynb
```

## 📊 Dataset

O dataset `lead1.0-small.csv` contém leituras de consumo energético em kWh de diferentes edifícios, incluindo **rótulos de anomalias** para avaliação supervisionada do TEDA.

### Referência do dataset  
- **LEAD1.0: A Large-scale Annotated Dataset for Energy Anomaly Detection in Commercial Buildings**, Manoj Gulati & Pandarasamy Arjunan, arXiv preprint, 30 de março de 2022. Disponível em: [arXiv](https://arxiv.org/abs/2203.17256)

### Principais referências:

- Angelov, P. **"Anomaly detection based on eccentricity analysis"**, apresentação do framework TEDA em *IEEE Symposium on Evolving and Autonomous Learning Systems (EALS)*, Orlando, FL, EUA, dezembro de 2014. Introduz os conceitos de *typicality* e *eccentricity*, calculados de forma recursiva e sem assumir distribuições paramétricas.  [IEEE Xplore](https://ieeexplore.ieee.org/document/7009497) 

- Angelov também publicou o artigo **"Outside the Box: An Alternative Data Analytics Framework"**, *Journal of Automation, Mobile Robotics and Intelligent Systems*, vol. 8, n.º 2, 2014, p. 29-35, que fundamenta o TEDA como uma metodologia sistemática que dispensa suposições prévias sobre os dados e é adequada para processos reais complexos.  [JAMRIS](https://www.jamris.org/index.php/JAMRIS/article/view/299)


- **TEDA-RLS: A TinyML Incremental Learning Approach for Outlier Detection and Correction**, Pedro Andrade et al., *IEEE Sensors Journal*, novembro de 2024. Proposta de um algoritmo incremental baseado em RLS para detecção e correção de outliers em tempo real, implementado em um scanner OBD-II como prova de conceito. Disponível em: [IEEE Xplore](https://ieeexplore.ieee.org/abstract/document/10682534)

- **TEDA-Forecasting: An Unsupervised TinyML Incremental Learning Approach for Outlier Processing and Forecasting**, Pedro Andrade et al., *Computing*, vol. 107, artigo 162, publicado em 2 de julho de 2025, DOI: 10.1007/s00607-025-01490-3. Apresenta uma versão do TEDA adaptada para previsão de séries temporais e correção de outliers, com execução em dispositivo real de edge computing (TinyML)  [Springer Nature - Computing](https://link.springer.com/article/10.1007/s00607-025-01490-3)


## 🧩 Algoritmo TEDA

O TEDA (Typicality and Eccentricity Data Analytics) é um método incremental para detecção de anomalias que **não requer treinamento prévio** e é adequado para **execução em dispositivos embarcados** (TinyML).

## 🏆 Atividades

O notebook contém:
- Demonstrações passo a passo
- Exercícios práticos para explorar diferentes valores de `m`
- Comparação de desempenho entre prédios

## 📜 Licença

Este projeto é distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## 🌎 Sobre o Grupo Conect2AI

O grupo de pesquisa [**Conect2AI**](http://conect2ai.dca.ufrn.br) é composto por estudantes de graduação e pós-graduação da Universidade Federal do Rio Grande do Norte (UFRN). Nossa missão é aplicar Inteligência Artificial (IA) e Aprendizado de Máquina em áreas emergentes.

### 🎯 Nossas áreas de atuação incluem:

- **Inteligência Embarcada e IoT**: Otimização da gestão de recursos e eficiência energética para ambientes conectados.
- **Transição Energética e Mobilidade**: Uso de IA para otimizar o consumo energético de veículos conectados e promover uma mobilidade mais eficiente e sustentável.