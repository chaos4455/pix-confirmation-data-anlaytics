# 🚀 Projeto de Automação de Pagamento PIX 💸

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Flask](https://img.shields.io/badge/Flask-2.0%2B-black.svg)
![Mercado Pago API](https://img.shields.io/badge/MercadoPago-API-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-green.svg)
![Plotly](https://img.shields.io/badge/Plotly-Data%20Visualization-red.svg)
![Requests](https://img.shields.io/badge/Requests-API%20Calls-9cf.svg)
![Websocket](https://img.shields.io/badge/Websocket-Real--time%20Data-orange.svg)
![Webhook](https://img.shields.io/badge/Webhook-Automation%20Trigger-yellow.svg)

Este projeto é uma solução completa de automação para **emissão e confirmação de pagamentos via PIX** usando o **Mercado Pago API** integrado a um sistema de **PDV (Ponto de Venda)**. O sistema é projetado para gerar, processar e confirmar automaticamente pagamentos através de uma série de funcionalidades como webhooks, pooling e geração de relatórios analíticos com gráficos e heatmaps.

## 🎯 Propósito do Repositório

Este repositório tem como objetivo demonstrar na prática meus conhecimentos avançados na criação de **soluções de gráficos, relatórios, análises de dados (analytics) e dashboards interativos**. Através deste projeto, desenvolvi uma **automação completa** que processa eventos de pagamento via PIX, gera gráficos detalhados como heatmaps e envia esses relatórios automaticamente por **email**, **Telegram**, entre outros canais de comunicação.

A solução foi desenvolvida utilizando uma arquitetura de **micro serviços**, integrando APIs de pagamento, ferramentas de visualização de dados e modelos de linguagem (LLMs) para otimizar a entrega e análise dos dados. Isso permite uma gestão eficiente dos pagamentos e insights poderosos sobre as operações financeiras, levando a uma análise mais profunda dos padrões de transação e otimização de processos.


## 🔥 Funcionalidades Principais

- **Emissão de Pagamentos PIX**: Utilizando a API do Mercado Pago, o sistema gera automaticamente QR Codes para pagamentos PIX.
- **Confirmação de Pagamentos**: A confirmação de pagamentos é feita automaticamente via WebSocket ou webhook, garantindo que as transações sejam verificadas em tempo real.
- **Armazenamento de Eventos**: Cada evento de pagamento (geração, confirmação, falha) é registrado como um arquivo JSON, criando um log detalhado de todas as interações.
- **Transformação de Dados**: Os eventos registrados podem ser transformados em PDFs para fácil consulta e armazenamento.
- **Automação de Processamento**: O sistema possui uma automação que processa esses eventos, analisa os dados e gera insights a partir deles.
- **Análise e Visualização de Dados**: Gráficos e heatmaps foram criados para analisar o comportamento dos pagamentos e gerar relatórios detalhados sobre:
  - Volume de transações por hora, dia, cidade e loja.
  - Preços médios e ociosidade por período.
  - Tempo médio de processamento por transação.
  - Transações mínimas, máximas e médias ao longo do tempo.
  
## 🔧 Tecnologias Utilizadas

- **Flask**: Backend leve e eficiente para gerenciar a API e as requisições.
- **Requests**: Biblioteca usada para fazer chamadas para a API do Mercado Pago.
- **WebSocket**: Implementado para monitorar em tempo real o status dos pagamentos.
- **Webhook**: Automação para recebimento de notificações de pagamento.
- **Pandas**: Utilizado para manipulação e processamento dos dados coletados.
- **Plotly**: Ferramenta para visualização dos dados através de gráficos interativos e heatmaps.
- **Pillow (PIL)**: Usada para salvar as visualizações como imagens PNG.

## 📊 Processamento e Visualização dos Dados

Para entender melhor o comportamento dos pagamentos e identificar padrões de uso, foram criados diversos gráficos e heatmaps utilizando **Pandas** e **Plotly**. Esses gráficos incluem análises de:

- Volume de transações por dia e por hora, divididos por cidade e loja.
- Tempo médio de processamento dos pagamentos.
- Ociosidade e preços baixos registrados em determinados períodos.
- Heatmaps que indicam a densidade de transações ao longo da semana e do dia.
- Análises de transações mínimas, médias e máximas em diferentes intervalos de tempo.

Essas visualizações são geradas automaticamente e salvas no repositório, com arquivos no formato `.png` como, por exemplo:

Esses gráficos permitem visualizar as tendências de uso, ajudando a tomar decisões estratégicas e otimizar o processo de pagamentos.
![mapa_calor_dia_min](https://github.com/user-attachments/assets/02da8bce-8dff-4863-92f4-0e4f0c37347c)
![mapa_calor_semana_count](https://github.com/user-attachments/assets/4b4d78db-d0aa-40ed-914a-ff33259e4169)
![mapa_calor_semana_sum](https://github.com/user-attachments/assets/744b5e44-8adc-4f58-ac01-26af93008cbb)
![mapa_calor_semana_mean](https://github.com/user-attachments/assets/c220101b-15af-4e65-9899-15db6e11e981)
![mapa_calor_semana_max](https://github.com/user-attachments/assets/04391bbd-0b8e-45cf-b8de-0302817b1c9b)
![mapa_calor_semana_min](https://github.com/user-attachments/assets/a6b98c62-b291-42e3-9a0b-1c29eb1dbfa5)
![mapa_calor_ociosidade_por_hora_loja](https://github.com/user-attachments/assets/a3339eeb-74f2-45fb-9f7a-642caaea3e6b)
![mapa_calor_precos_baixos_por_hora_loja](https://github.com/user-attachments/assets/c34b3f9b-c93d-493a-b3da-74d0273cbccf)
![mapa_calor_media_transacoes_por_hora_loja](https://github.com/user-attachments/assets/a6fecb81-c875-459a-b89b-eabd944cd108)
![mapa_calor_minimos_por_hora_loja](https://github.com/user-attachments/assets/c89f4ea4-8cdb-4c91-8c48-a9d4076d0ad0)
![mapa_calor_tempo_medio_por_hora_cidade](https://github.com/user-attachments/assets/cd2474e3-d0da-4fd0-ace7-1a81ba8283a0)
![mapa_calor_volume_transacoes_por_hora_cidade](https://github.com/user-attachments/assets/a3c82427-5868-4114-8a4c-173fd0e167e6)
![mapa_calor_media_transacoes_por_hora_cidade](https://github.com/user-attachments/assets/816a010e-9609-453d-8f87-5f484b9514b7)
![mapa_calor_minimos_por_hora_cidade](https://github.com/user-attachments/assets/a2d554c3-11e4-4653-84aa-d26ebd820420)
![mapa_calor_pagamentos_por_dia](https://github.com/user-attachments/assets/39bbaedf-b474-4ad0-9875-1a49633b1f60)
![mapa_calor_precos_baixos_por_dia](https://github.com/user-attachments/assets/624c317a-e567-45fa-9425-6147009b0fce)
![mapa_calor_ociosidade_por_dia](https://github.com/user-attachments/assets/162f367e-a3cd-4949-8d8b-29cd88887c45)
![mapa_calor_tempo_medio_por_dia](https://github.com/user-attachments/assets/117792b6-d2d0-4f3a-8cc1-bf0bd44511e0)
![mapa_calor_volume_transacoes_por_dia](https://github.com/user-attachments/assets/432e5e6f-b7f7-44b5-9591-6bcc388783a7)
![mapa_calor_minimos_por_dia](https://github.com/user-attachments/assets/cad0bfd7-8943-4cf3-8419-a0d7431bfed7)
![mapa_calor_loja_count](https://github.com/user-attachments/assets/569c6d1b-9209-4672-be70-161f2ecb999c)
![mapa_calor_loja_sum](https://github.com/user-attachments/assets/dfded657-f942-48f7-bb1f-e9da5b42717f)
![mapa_calor_loja_mean](https://github.com/user-attachments/assets/7aabe4f4-5bca-4cf7-b3f6-3d965e23a166)
![mapa_calor_loja_max](https://github.com/user-attachments/assets/11eb38e4-6a4d-4da6-8bbd-6b9d932a68d1)
![mapa_calor_loja_min](https://github.com/user-attachments/assets/567bba69-5d1b-4b9a-b84c-d700f47d827c)
![mapa_calor_cidade_count](https://github.com/user-attachments/assets/454804c8-bc60-4c24-a104-95c97d6ee201)
![mapa_calor_cidade_sum](https://github.com/user-attachments/assets/29ee3201-50b9-40d4-aa70-e0cf5afaae66)
![mapa_calor_cidade_mean](https://github.com/user-attachments/assets/fe034207-a2af-41f5-8254-175c9d98dd87)
![mapa_calor_cidade_max](https://github.com/user-attachments/assets/9f0979ce-6971-40a8-af18-516cfd34ef69)
![mapa_calor_cidade_min](https://github.com/user-attachments/assets/34bf3d44-0c2a-4993-8551-99c402022b1e)
![mapa_calor_dia_count](https://github.com/user-attachments/assets/34a97ba8-0d4d-4ff4-b171-278c9a7092e6)
![mapa_calor_dia_sum](https://github.com/user-attachments/assets/ce89a887-764f-44ad-954b-47eb2a8cf22f)
![mapa_calor_dia_mean](https://github.com/user-attachments/assets/009f1079-bc4a-4595-95b7-493e1018cd47)
![mapa_calor_dia_max](https://github.com/user-attachments/assets/2b141403-dabf-400f-90c1-9f2c0492b854)
---
