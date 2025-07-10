## Projeto de Análise e Transformação de Dados com Azure Data Factory e Data Flow


#### Status: ⏳ Em progresso

---

### 🚀 Visão Geral

Este projeto simula um ambiente corporativo de engenharia e análise de dados utilizando Microsoft Azure, com foco na construção de pipelines para ingestão, transformação e armazenamento de dados.

Utilizamos Azure Data Factory para orquestração e Azure Data Flow (Spark) para transformação dos dados, organizando os dados nas camadas Bronze, Silver e Gold.

---

### 🎯 Objetivos de aprendizagem

- Simular um ambiente de dados corporativo real
- Aprender o fluxo de ingestão e tratamento em camadas
- Aplicar boas práticas de arquitetura em nuvem
- Documentar e versionar o projeto para portfólio

---

### 🗂 Estrutura dos Dados

- **Camada Bronze:** dados brutos importados diretamente dos arquivos CSV originais.
- **Camada Silver:** dados limpos e estruturados, com tratamentos e ajustes.
- **Camada Gold:** dados transformados, agregados e prontos para análise e consumo, armazenados em arquivos CSV únicos.

---

## 📁 Dados Utilizados

Os dados utilizados são arquivos CSV simulando dados de pedidos, clientes, produtos, pagamentos, geolocalização e avaliações, com schemas interligados.

---

### ⚙️ Tecnologias e Ferramentas

- Microsoft Azure Data Factory (ADF)
- Azure Blob Storage (para armazenar arquivos CSV)
- Azure Portal para gerenciamento
-  Azure Data Flow (Spark)
- GitHub para versionamento e documentação

---

### 🔧 Passos para Reproduzir o Projeto

1. Criar Storage Account no Azure e configurar containers para Bronze, Silver e Gold.
2. Criar datasets no ADF apontando para os arquivos CSV em cada camada.
3. Criar pipelines no ADF com Data Flows para realizar joins e transformações.
4. Configurar parâmetros para flexibilizar caminhos e nomes de arquivos.
5. Executar pipelines e verificar arquivos transformados na camada Gold.
6. Opcional: conectar ferramentas de BI (ex: Power BI) para análise.

---

### 📝 Sobre a Transformação Principal

- Data Flow que realiza join entre as tabelas `orders` e `customers`.
- Produz um CSV único (`pedidos_com_clientes.csv`) na camada Gold.
- Parâmetros configurados para permitir reuso e escalabilidade.

---

### 💡 Observações

- O Data Flow foi configurado para usar “Single partition” para gerar um único arquivo CSV.
- O projeto pode ser expandido para incluir outras tabelas e transformações.
- Ideal para aprendizado prático de pipelines de dados no Azure.

---
## ✨ Autora

Thayla Oliveira  
[LinkedIn](https://linkedin.com/in/thayla-oliveira) | [Email](thaylathais1@gmail.com)

