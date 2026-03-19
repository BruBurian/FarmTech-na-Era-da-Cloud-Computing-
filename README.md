# 🌾 Crop Yield Prediction - FarmTech Solutions

## 📌 Descrição do Projeto

Este projeto foi desenvolvido como parte da atividade acadêmica da FIAP, com o objetivo de aplicar técnicas de Inteligência Artificial e Machine Learning para análise de dados agrícolas.

A proposta consiste em analisar um conjunto de dados contendo informações climáticas e de solo, a fim de prever o rendimento de diferentes culturas agrícolas em uma fazenda de médio porte (aproximadamente 200 hectares).

---

## 🎯 Objetivo

* Realizar análise exploratória dos dados (EDA)
* Identificar padrões e tendências na produtividade agrícola
* Aplicar técnicas de clusterização para segmentação dos dados
* Desenvolver modelos preditivos capazes de estimar o rendimento das safras
* Avaliar o desempenho dos modelos utilizando métricas apropriadas

---

## 📊 Dataset

O conjunto de dados utilizado (`crop_yield.csv`) contém as seguintes variáveis:

* **Cultura**: tipo de cultura agrícola
* **Precipitação (mm/dia)**: volume de chuva diário
* **Umidade específica a 2m (g/kg)**: quantidade de vapor de água no ar
* **Umidade relativa a 2m (%)**: percentual de umidade no ar
* **Temperatura a 2m (°C)**: temperatura ambiente
* **Rendimento (ton/ha)**: produtividade da safra

---

## 🔍 Análise Exploratória (EDA)

Foram realizadas análises iniciais para entendimento dos dados, incluindo:

* Verificação de valores nulos
* Estatísticas descritivas
* Análise de distribuição das variáveis
* Matriz de correlação

Essas etapas permitiram identificar padrões iniciais e relações entre variáveis climáticas e o rendimento agrícola.

---

## 📌 Clusterização

Foi aplicada a técnica de **K-Means** para agrupar os dados em clusters, possibilitando:

* Identificação de padrões de produtividade
* Segmentação de cenários agrícolas
* Detecção de possíveis outliers

---

## 🤖 Modelos Preditivos

Foram implementados cinco algoritmos de regressão supervisionada:

* Regressão Linear
* Árvore de Decisão
* Random Forest
* K-Nearest Neighbors (KNN)
* Support Vector Regression (SVR)

---

## 📏 Métricas de Avaliação

Os modelos foram avaliados utilizando:

* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **R² (Coeficiente de Determinação)**

Essas métricas permitiram comparar a precisão e desempenho de cada modelo.

---

## 📈 Resultados

O modelo com melhor desempenho foi identificado com base nas métricas de erro e capacidade de explicação dos dados (R²).

Os resultados indicam que fatores como temperatura, umidade e precipitação possuem influência direta no rendimento das culturas.

---

## ⚠️ Limitações

* Dataset com quantidade limitada de variáveis
* Ausência de fatores importantes como tipo de solo, uso de fertilizantes e manejo agrícola
* Possível presença de outliers impactando os modelos

---

## 🚀 Melhorias Futuras

* Inclusão de novas variáveis relevantes
* Teste com modelos mais avançados (XGBoost, Redes Neurais)
* Otimização de hiperparâmetros
* Coleta de dados em maior escala

---

## 📁 Estrutura do Projeto

```
📦 projeto
 ┣ 📄 crop_yield.csv
 ┣ 📄 BrunoBurian_rm568025_pbl_fase5 .ipynb
 ┗ 📄 README.md
```

## 📌 Observações

Todo o desenvolvimento do projeto, incluindo código, análises e conclusões, está documentado no notebook Jupyter presente neste repositório.

---

# ☁️ Entrega 2 - Estimativa de Custos na AWS

## 🎯 Objetivo

Nesta etapa, foi realizada uma estimativa de custos utilizando a calculadora da AWS para hospedar a solução de Machine Learning desenvolvida na Entrega 1.

A infraestrutura será responsável por:

* Receber dados de sensores agrícolas via API
* Processar os dados
* Executar o modelo preditivo de rendimento de safra

---

## ⚙️ Configuração da Máquina

A simulação foi feita considerando uma instância com as seguintes características:

* **Sistema Operacional:** Linux
* **vCPUs:** 2
* **Memória:** 1 GiB
* **Rede:** até 5 Gigabit
* **Armazenamento:** 50 GB (EBS - HD)
* **Modelo de cobrança:** On-Demand (100%)

---

## 🌎 Comparação de Regiões

### 🇧🇷 Região: São Paulo (sa-east-1)

* Maior custo operacional
* Baixa latência para aplicações no Brasil
* Conformidade com leis de armazenamento de dados (LGPD)

💰 **Custo estimado mensal:** ~$15 - $20 USD

---

### 🇺🇸 Região: Virgínia do Norte (us-east-1)

* Infraestrutura mais barata
* Alta disponibilidade e escalabilidade
* Maior latência para usuários no Brasil

💰 **Custo estimado mensal:** ~$8 - $12 USD

---

## 📊 Análise Comparativa

| Critério          | São Paulo 🇧🇷 | Virgínia 🇺🇸 |
| ----------------- | -------------- | ------------- |
| Custo             | ❌ Maior        | ✅ Menor       |
| Latência          | ✅ Baixa        | ❌ Maior       |
| Conformidade      | ✅ Alta         | ❌ Restrita    |
| Performance local | ✅ Melhor       | ❌ Inferior    |

---

## 🧠 Escolha da Região

A escolha da região depende de dois fatores principais:

### 📌 Cenário com restrições legais (LGPD)

Devido à necessidade de manter os dados dentro do território nacional, a melhor escolha é:

👉 **Região de São Paulo (sa-east-1)**

### ✔️ Justificativa:

* Garantia de conformidade com a legislação brasileira (LGPD)
* Menor latência para envio e processamento dos dados dos sensores
* Maior confiabilidade na comunicação em tempo real

---

## ⚖️ Trade-off

Embora a região da Virgínia apresente menor custo, ela não atende aos requisitos legais e de desempenho do projeto.

Portanto, opta-se por um custo maior em troca de:

* Segurança jurídica
* Melhor performance
* Estabilidade operacional

---

## 🖼️ Simulação na Calculadora AWS

*(INSIRA AQUI PRINTS DA AWS CALCULATOR)*

Sugestões de imagens:

* Configuração da instância
* Comparação de preço entre regiões
* Resumo final da estimativa

---
## 🎥 Vídeo de Demonstração

🔗 (INSIRA AQUI O LINK DO SEU VÍDEO NO YOUTUBE - NÃO LISTADO)

---

## 👨‍💻 Integrantes do Grupo

* Bruno Nogueira Burian - RM568025

---

## 📌 Conclusão

A análise demonstrou que, apesar da diferença de custo entre regiões, a escolha da infraestrutura deve considerar não apenas o preço, mas também fatores como latência, conformidade legal e requisitos do negócio.

Para este projeto, a região de São Paulo se mostrou a opção mais adequada.
