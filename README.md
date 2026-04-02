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
- 
https://services.odata.org/V2/OData/OData.svc/


---

## 📁 Package Structure

### 📦 Package Name
```bash
ZPKG_CPI_ODATA_ENRICHMENT

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




































# 🚀 SAP CPI – Integração com Request-Reply & Content Enricher (OData)
## SAP BTP CPI - ODATA_ENRICHMENT

No dia a dia das empresas, é muito comum a necessidade de integrar diferentes sistemas para consolidar informações e apoiar processos de negócio.

Neste cenário, demonstro como utilizar os componentes Request-Reply e Content Enricher no SAP Cloud Integration para construir uma integração eficiente baseada em serviços OData.

🎯 Problema de Negócio

Imagine um cenário onde:

Um sistema fornece dados de produtos
Outro sistema contém informações de fornecedores
E uma aplicação precisa de tudo isso junto para exibir ou processar dados

👉 O desafio é:
Como consolidar essas informações em tempo real?

🧩 Solução Proposta

A solução utiliza dois padrões clássicos de integração:

🔹 Request-Reply

Responsável por buscar os dados principais (produtos) em um serviço externo.

🔹 Content Enricher

Responsável por complementar os dados com informações adicionais (fornecedores).


### Criando o Package
![Fluxo](imagens/Screenshot_1.png)

<br>

### Nome do Package
![Fluxo](imagens/Screenshot_2.png)
```
ZPKG_CPI_ODATA_ENRICHMENT
```
<br>

## 🧩 Criação do Integration Flow

### Adicionando o Artefato
![Fluxo](imagens/Screenshot_3.png)
```
CPI_ODATA_ENRICHMENT
```

<br>

## HTTPS
![Fluxo](imagens/Screenshot_4.png)


<br>

### Adicionando o Endpoint
![Fluxo](imagens/Screenshot_5.png)
```
/odata_enrichment
```

<br>

## Request Replay
Adicionando o Request Replay
![Fluxo](imagens/Screenshot_6.png)

<br>

### Adicionando o ODATA
![Fluxo](imagens/Screenshot_7.png)

<br>

### Selecionando o OData V2
![Fluxo](imagens/Screenshot_8.png)

<br>

### Configurando o Request Replay
![Fluxo](imagens/Screenshot_9.png)
```
https://services.odata.org/V2/OData/OData.svc/
```

<br>

### Configurando o Request Replay Connection
![Fluxo](imagens/Screenshot_10.png)

<br>

### Selecionando o proximo passo nas configurações do OData
![Fluxo](imagens/Screenshot_11.png)

<br>

### Selecionando as configurações e Definindo 
![Fluxo](imagens/Screenshot_12.png)

<br>

### Receiver
Adicionado um novo Receiver
![Fluxo](imagens/Screenshot_13.png)

<br>

### Content Enrichment
Adicionando o Content Enrichment
![Fluxo](imagens/Screenshot_14.png)


<br>

### Adicionando o OData
![Fluxo](imagens/Screenshot_15.png)

<br>

### Selecionando o OData V2
![Fluxo](imagens/Screenshot_16.png)

<br>

### Configurando o OData
Configurando o Connection
![Fluxo](imagens/Screenshot_17.png)
```
https://services.odata.org/V2/OData/OData.svc/
```

<br>

### Configurando o OData Processing
![Fluxo](imagens/Screenshot_18.png)

<br>

### Selecionando o proximo passo nas configurações do OData
![Fluxo](imagens/Screenshot_19.png)

<br>

### Configurando o Entidades e definindo as operations
![Fluxo](imagens/Screenshot_20.png)

<br>

### Content Enrichment
Configurando o Content Enrichment em Processing
![Fluxo](imagens/Screenshot_21.png)
```
ORIGINAL MESSAGE
Path to Node: /Products/Product
Key Element: ID

LOOKUP MESSAGE
Path to Node: /Suppliers/Supplier
Key Element: ID
```

<br>

### iFlow finalizado
Vamos salvar e fazer o Deploy
![Fluxo](imagens/Screenshot_22.png)

<br>

### POSTMAN
Resultado do Postman
![Fluxo](imagens/Screenshot_23.png)

<br>
<br>

---

## 📦 Exemplo prático – iFlow para baixar

📦 [Download do iFlow – CPI_ODATA_ENRICHMENT.zip](https://github.com/souzajean/CPI_ODATA_ENRICHMENT/raw/main/Package/CPI_ODATA_ENRICHMENT.zip)













