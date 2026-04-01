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

### Nome do iFlow
![Fluxo](imagens/Screenshot_9.png)
```
https://services.odata.org/V2/OData/OData.svc/
```

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_10.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_11.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_12.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_13.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_14.png)


<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_15.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_16.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_17.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_18.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_19.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_20.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_21.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_22.png)

<br>

### Nome do iFlow
![Fluxo](imagens/Screenshot_23.png)














