# 🚀 SAP CPI – OData Integration with Request-Reply & Content Enricher

## 📌 Overview

Este projeto demonstra a construção de um cenário de integração no **SAP Cloud Integration (SAP CPI)** utilizando serviços **OData V2**, aplicando padrões clássicos de integração para consolidação de dados em tempo real.

A solução combina os componentes **Request-Reply** e **Content Enricher** para orquestrar múltiplas fontes de dados em um único payload enriquecido.

---

## 🎯 Business Scenario

Em ambientes corporativos, é comum a necessidade de consolidar informações provenientes de diferentes sistemas.

### Cenário proposto:

- Um sistema fornece **dados de produtos**
- Outro sistema fornece **dados de fornecedores**
- Uma aplicação necessita dessas informações **de forma unificada**

### ❗ Desafio

Como integrar múltiplas fontes e entregar um payload consolidado em tempo real?

---

## 🧩 Solution Architecture

A solução implementa dois padrões fundamentais de integração:

### 🔹 Request-Reply
Responsável por consumir os dados principais (Products) via serviço OData.

### 🔹 Content Enricher
Responsável por enriquecer o payload com dados adicionais (Suppliers), com base em uma chave comum.

---

## 🏗️ Technical Architecture

- **Plataforma:** SAP BTP – Cloud Integration  
- **Protocolo:** HTTPS  
- **Formato:** XML (OData V2)  
- **Serviço de teste:**

https://services.odata.org/V2/OData/OData.svc/


---

## 📁 Package Structure

### 📦 Package Name
```bash
ZPKG_CPI_ODATA_ENRICHMENT
```
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

# :building_construction: Arquitetura do iFlow

## 🔄 Fluxo da Integração

---

### Criando o Package
Criação do package no SAP Cloud Integration, responsável por organizar e agrupar os artefatos de integração relacionados ao cenário.

![Fluxo](imagens/Screenshot_1.png)

<br>

### Nome do Package
Definição do nome técnico do package seguindo boas práticas de nomenclatura (prefixo Z para objetos customizados).

```bash
ZPKG_CPI_ODATA_ENRICHMENT
```
![Fluxo](imagens/Screenshot_2.png)

<br>

🧩 Criação do Integration Flow
Adicionando o Artefato

Criação do Integration Flow (iFlow), que será responsável por orquestrar todo o processo de integração entre os serviços OData.
```
CPI_ODATA_ENRICHMENT
```
![Fluxo](imagens/Screenshot_3.png)

<br>


















<br>
<br>

---

## 📦 Exemplo prático – iFlow para baixar

📦 [Download do iFlow – CPI_ODATA_ENRICHMENT.zip](https://github.com/souzajean/CPI_ODATA_ENRICHMENT/raw/main/Package/CPI_ODATA_ENRICHMENT.zip)













