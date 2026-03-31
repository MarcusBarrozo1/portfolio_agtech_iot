*Read this in [English](README_en.md).*
# Análise e Tratamento de Dados: Sensores IoT Agrícolas 🚜

Este projeto apresenta um pipeline básico de limpeza e preparação de dados para séries temporais de sensores IoT em um contexto de AgTech. O foco principal foi garantir a integridade dos dados antes da aplicação de modelos de Machine Learning, simulando desafios reais de hardware e conectividade no campo.

## 🛠️ Tecnologias e Ferramentas
- **Python 3.x**
- **Pandas & NumPy**: Manipulação de dados e álgebra linear.
- **Matplotlib**: Visualização de tendências (Dataviz).
- **VS Code & Jupyter Notebooks**: Ambiente de desenvolvimento.

## 📈 Desafios Técnicos Superados

### 1. Gestão de Séries Temporais
- Conversão de tipos de dados (`object` para `datetime`) e estruturação de índices temporais para análises cronológicas precisas.

### 2. Imputação de Dados Faltantes (NaN)
- Identificação de lacunas causadas por falhas de conectividade.
- Aplicação de **Interpolação Linear** para reconstruir a continuidade física das variáveis de temperatura e umidade, preservando a coerência dos dados.

### 3. Detecção e Correção de Anomalias (Outliers)
- Implementação de lógica estatística baseada em **Z-Score** (3 Desvios Padrão).
- Identificação automática de picos de hardware irreais e substituição por valores estatisticamente aceitáveis através de técnicas de suavização.

### 4. Engenharia de Atributos (Feature Engineering)
- Implementação de **Médias Móveis (Rolling Window)** de 24h para redução de ruído e extração de tendências climáticas de longo prazo.

## 📊 Resultados
O projeto resultou em um dataset limpo (`iot_agricola_clean.csv`), pronto para modelagem preditiva, com visualizações que comprovam a remoção de ruídos e a identificação de padrões diários.

---
**Marcus Barrozo** *Geographic Data Scientist | Remote Sensing Specialist*