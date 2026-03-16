# 🟦 FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
  <img src="src/assets/logo-fiap.png" width="80%" alt="FIAP">
</p>

# 🚜 FarmTech Solutions - Fase 5 (Machine Learning & Cloud)

Este repositório contém as entregas da **Fase 5 do projeto FarmTech Solutions**, contemplando o desenvolvimento de modelos preditivos (**Machine Learning**) e a arquitetura de infraestrutura na **nuvem (AWS)**.

---

## 📑 Sumário

1. Entrega 1: Machine Learning  
2. Entrega 2: Computação em Nuvem  
3. Justificativa de Arquitetura  
4. Estrutura do Projeto  
5. Tecnologias  
6. Integrantes  
7. Professores Responsáveis  

---

# 🎥 Vídeos Demonstrativos

## Machine Learning
👉 https://youtu.be/jnVNWj9T2p4

## Computação em Nuvem (AWS)
👉 https://youtu.be/kaJEX0Yj94U

---

# 🧠 Arquitetura da Solução

A arquitetura da solução proposta para o **FarmTech Solutions** segue o fluxo de coleta de dados agrícolas, processamento e análise preditiva utilizando Machine Learning, com hospedagem em infraestrutura de nuvem.

Pipeline da solução:

Sensores → Coleta de Dados → Machine Learning → API → Infraestrutura Cloud (AWS)

---

# 📘 Documentação do Projeto

O repositório contém todos os arquivos necessários para execução e análise da solução desenvolvida na Fase 5, incluindo:

- Notebook de Machine Learning  
- Dataset agrícola  
- Estrutura de diretórios  
- Evidências da estimativa de infraestrutura na AWS  

---

# 📊 Entrega 1 — Machine Learning (Previsão de Rendimento)

Foi realizada uma **análise exploratória de dados (EDA)**, seguida por **clusterização utilizando K-Means** para identificação de tendências e outliers.

Posteriormente foram treinados **5 modelos de regressão supervisionada** com o objetivo de prever o rendimento agrícola com base nas condições climáticas.

### Melhor Modelo

**Regressão Linear (R² de 0.995)**

### Notebook Completo

📄  
[MateusPenteado_rm568518_pbl_fase5.ipynb](./MateusPenteado_rm568518_pbl_fase5.ipynb)

---

# ☁️ Entrega 2 — Computação em Nuvem (Estimativa AWS)

Para hospedar a API responsável por receber os dados dos sensores e executar o modelo de Machine Learning, foi configurada uma instância **Amazon EC2** com a seguinte especificação:

- Sistema Operacional: Linux  
- Instância: **t4g.micro**  
- **2 vCPUs**  
- **1 GiB de RAM**  
- **50 GB de armazenamento gp3**  
- Cobrança **On-Demand**

A estimativa de custo foi realizada utilizando a **AWS Pricing Calculator** em duas regiões distintas.

---

## 🌎 Região 1 — US East (N. Virginia)

**Custo estimado:** $10,13 USD / mês

<p align="center">
  <img src="src/assets/aws_virginia.png" width="90%" alt="AWS Virginia Estimate">
</p>

---

## 🇧🇷 Região 2 — South America (São Paulo)

**Custo estimado:** $17,38 USD / mês

<p align="center">
  <img src="src/assets/aws_saopaulo.png" width="90%" alt="AWS Sao Paulo Estimate">
</p>

---

# ⚖️ Justificativa de Escolha da Região

Apesar da região da **Virgínia do Norte** apresentar um custo financeiro menor, a solução técnica escolhida para a FarmTech Solutions foi a **South America (São Paulo)**.

A escolha baseia-se em dois fatores principais.

## 1️⃣ Baixa Latência (Acesso Rápido)

O projeto exige acesso rápido aos dados coletados pelos sensores espalhados pela fazenda.

Manter o servidor geograficamente próximo (no Brasil) reduz drasticamente a latência de rede (ping), garantindo processamento em tempo real.

## 2️⃣ Compliance Legal

O enunciado destaca restrições legais para armazenamento de dados no exterior.

Ao hospedar a aplicação na região de São Paulo, garantimos a conformidade com as leis locais de proteção e soberania de dados (como a LGPD), evitando multas e quebra de contratos.

---

# 📂 Estrutura do Projeto

```bash
FIAP_FarmTech_Fase5/
├── src/
│   └── assets/
│       ├── aws_virginia.png
│       ├── aws_saopaulo.png
│       └── logo-fiap.png
├── MateusPenteado_rm568518_pbl_fase5.ipynb
├── crop_yield.csv
├── LICENSE
└── README.md
```
---
## 🧑‍💻 Tecnologias Utilizadas


Python

Pandas

Scikit-Learn

Jupyter Notebook

AWS EC2

AWS Pricing Calculator

---
## 👨‍🎓 Integrantes — Grupo S


<a href="https://www.linkedin.com/in/leno-siqueira-36789544?utm_source=share_via&utm_content=profile&utm_medium=member_ios">Leno Siqueira</a> — RM: 567893

<a href="https://www.linkedin.com/in/paulo-benfica-76057a7b">Paulo Benfica</a> — RM: 567648

<a href="https://www.linkedin.com/in/federico-villagra-97378838a">Fred Villagra</a> — RM: 567187

<a href="https://www.linkedin.com/in/math-penteado-1b4807200/">Mateus Lima</a> — RM: 568518

---
## 👩‍🏫 Professores Responsáveis


Tutor(a)

<a href="https://www.linkedin.com/in/sabrina-otoni-22525519b?utm_source=share_via&utm_content=profile&utm_medium=member_ios/">Sabrina Otoni FIAP</a>

Coordenador(a)

<a href="https://www.linkedin.com/company/inova-fusca/">André Godoi FIAP</a>

---
## 📜 Créditos e Licença

© 2025 — FIAP / PlantIA Agrodata

Licença MIT — uso livre para fins acadêmicos e de aprendizado.