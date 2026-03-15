# 🚜 FarmTech Solutions - Fase 5 (Machine Learning & Cloud)

Este repositório contém as entregas da Fase 5 do projeto FarmTech Solutions, contemplando o desenvolvimento de modelos preditivos (Machine Learning) e a arquitetura de infraestrutura na nuvem (AWS).

## 📊 Entrega 1: Machine Learning (Previsão de Rendimento)
Foi realizada uma análise exploratória (EDA), clusterização (K-Means) para identificar tendências e outliers, e o treinamento de 5 modelos de regressão supervisionada para prever o rendimento agrícola com base nas condições climáticas.

* **Melhor Modelo:** Regressão Linear (R² de 0.995).
* **Notebook completo:** [Acesse o arquivo MateusPenteado_rm568518_pbl_fase5.ipynb aqui](./MateusPenteado_rm568518_pbl_fase5.ipynb)
* **Vídeo Demonstrativo (ML):** https://youtu.be/jnVNWj9T2p4

---

## ☁️ Entrega 2: Computação em Nuvem (Estimativa AWS)

Para hospedar a API que receberá os dados dos sensores e rodará o modelo de Machine Learning, configuramos uma instância **Amazon EC2** (Linux, t4g.micro com 2 vCPUs, 1 GiB de RAM e 50 GB de armazenamento gp3, 100% sob demanda).

Realizamos a cotação em duas regiões diferentes utilizando a AWS Pricing Calculator:

1. **US East (N. Virginia):** Custos estimados em **$10,13 USD/mês**.

<img width="1869" height="908" alt="aws_virginia" src="https://github.com/user-attachments/assets/bd6cdba7-ab60-4c9e-8389-0d1e52fad0be" />

2. **South America (São Paulo):** Custos estimados em **$17,38 USD/mês**.

<img width="1912" height="956" alt="aws_saopaulo" src="https://github.com/user-attachments/assets/679a5034-1812-4638-bd90-e7ea2e7fe0c0" />


### ⚖️ Justificativa de Escolha da Região
Apesar da região da Virgínia do Norte apresentar um custo financeiro menor, a solução técnica correta e escolhida para a FarmTech Solutions é a **South America (São Paulo)**. A escolha fundamenta-se em dois pilares essenciais do projeto:

1. **Baixa Latência (Acesso Rápido):** O projeto exige acesso rápido aos dados coletados pelos sensores espalhados pela fazenda. Manter o servidor geograficamente próximo (no Brasil) reduz drasticamente a latência de rede (ping), garantindo processamento em tempo real.
2. **Compliance Legal:** O enunciado destaca restrições legais para armazenamento de dados no exterior. Ao hospedar a aplicação na região de São Paulo, garantimos a conformidade com as leis locais de proteção e soberania de dados (como a LGPD), evitando multas e quebra de contratos.

* **Vídeo Demonstrativo (AWS):** https://youtu.be/kaJEX0Yj94U
