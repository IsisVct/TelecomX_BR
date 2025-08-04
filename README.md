# 📊 TelecomX BR - Análise de Evasão de Clientes

Este repositório contém uma análise de dados focada na evasão de clientes (churn) da empresa fictícia **TelecomX BR**, desenvolvida como parte do **Challenge de Data Science - ETL da Alura**.

---

## 🔍 Objetivo

O objetivo deste projeto é aplicar um processo de **ETL (Extração, Transformação e Carga)** para analisar os principais fatores associados à evasão de clientes e gerar **insights estratégicos** para retenção.

---

## 🛠️ Tecnologias e Bibliotecas Utilizadas

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly Express

---

## 📂 Estrutura do Projeto

telecomx_br.py # Código principal com etapas de ETL e análise exploratória


README.md # Documentação do projeto

df_telecomx.csv # Dataframe com os dados tratados em .csv

---

## 🧪 Etapas do Projeto

### 1. **📥 Extração de Dados**
- Fonte: JSON hospedado no GitHub.
- Normalização das colunas aninhadas: `customer`, `phone`, `internet`, `account`.

### 2. **🧹 Transformação**
- Tratamento de valores nulos (`Churn`, `Charges.Total`);
- Conversão de variáveis categóricas (`Yes`/`No` → `1`/`0`);
- Criação de colunas derivadas:
  - `Contas_Diarias` (valor estimado diário);
  - `TenureCategory` (segmentação por tempo de permanência);
  - `TotalServicos` (quantidade de serviços contratados).

### 3. **📊 Carga e Análise**
- Análises estatísticas descritivas;
- Visualizações com `matplotlib`, `seaborn` e `plotly`;
- Geração de insights e recomendações estratégicas.

---

## 📈 Principais Insights
<img width="4200" height="1800" alt="taxa_de_churn (1)" src="https://github.com/user-attachments/assets/4f87b9db-ecc2-478d-b418-98d80b285ffa" />

- **Taxa de evasão**: 26,5% dos clientes cancelaram os serviços.
- **Tenure ≤ 9 meses** → risco de churn quase 2x maior.
- **Contratos mensais** concentram maior evasão.
- **Cheque eletrônico** é o método de pagamento com maior churn.
- **Clientes jovens** tendem a evadir mais.
- **Faturas altas** também estão associadas ao cancelamento.

---

## 🎯 Recomendações

- **Oferecer incentivos** para contratos longos e pagamento automático;
- **Focar em retenção de clientes novos**, principalmente nos 9 primeiros meses;
- **Personalizar planos** para jovens e clientes com cobrança elevada;
- **Campanhas educativas** sobre os benefícios dos serviços da empresa.

---

## ▶️ Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/IsisVct/TelecomX_BR.git
   cd TelecomX_BR

2. Instale as dependências
   ```bash
   pip install pandas numpy matplotlib seaborn plotly

4. Execute o script:
   
   python telecomx_br.py

   
##📌 Observações
Este projeto foi desenvolvido em ambiente Colab, mas pode ser executado localmente.

Algumas visualizações requerem ambiente gráfico (como Jupyter ou Google Colab).

Os dados utilizados são públicos e disponibilizados pela Alura para fins educacionais.

##📚 Créditos
Desenvolvido por Isabelle Victoria de Souza 💻
Desafio proposto pela Alura — ONE | TECH FOUNDATION - Especialização Data Science.


