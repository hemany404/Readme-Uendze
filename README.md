<div align="center">

<img src="./assets/uendze-logo.png" alt="Uendze Logo" width="260" />

# **Uendze.**

### Plataforma de Dados Financeiros do Mercado Angolano

<br />

![Status](https://img.shields.io/badge/Status-MVP%20em%20desenvolvimento-yellow)
![Foco](https://img.shields.io/badge/Foco-Mercado%20Angolano-red)
![Produto](https://img.shields.io/badge/Tipo-API%20%26%20SDK-blue)

</div>

---

## **O que é o Uendze? (Visão Geral)**

O **Uendze** é uma plataforma de **dados financeiros** focada exclusivamente no **mercado angolano**, criada para resolver um problema central:

>  A inexistência de **dados financeiros estruturados, padronizados e acessíveis via API** em Angola.

O projeto nasce com uma abordagem **API-first**, servindo como infraestrutura base para desenvolvedores, analistas, startups e fintechs.

> 🎯 **Missão:** tornar dados financeiros angolanos acessíveis, utilizáveis e confiáveis.

<br />

<p align="center">
 <img src="./assets/uendze-logo.png" width="90%" alt="Uendze"/>
</p>

<br />

> ### **Do 0 ao MVP: o Uendze em construção**
>
> O Uendze está a ser desenvolvido do zero, com foco em arquitetura limpa, modelo de dados correto e crescimento sustentável.

---

## **Público-Alvo**

O Uendze foi desenhado para:

*  **Desenvolvedores** que precisam consumir dados financeiros via API
*  **Analistas de dados e pesquisadores**
*  **Startups e fintechs angolanas**
*  **Estudantes** de tecnologia, economia e finanças

---

## **✅ Benefícios Principais**

> Simples, direto e útil.

*  Dados financeiros **centralizados** do mercado angolano
*  API REST **simples e previsível**
*  Modelo de dados preparado para **histórico e análises**
*  Menos tempo a coletar dados manualmente
*  Base sólida para produtos financeiros futuros

---

## **🧠 O Problema**

Atualmente em Angola:

1.  Não existem APIs públicas financeiras modernas
2.  Dados estão dispersos, manuais ou em PDF
3.  Desenvolvedores precisam “raspar” dados
4.  Falta histórico estruturado

---

## **A Solução Uendze**

O Uendze resolve isso criando:

>  Uma **camada única de dados financeiros**
>  Um **modelo de dados consistente**
>  Uma **API REST clara**
>  **SDKs** para facilitar integrações

Começamos por **Angola**, com profundidade e qualidade, antes de qualquer expansão.

---

## **Arquitetura (Visão Simplificada)**

```
Fontes de Dados (Mercado Angolano)
            ↓
     Ingestão / ETL
            ↓
      Banco de Dados
            ↓
        API REST
            ↓
        SDKs
            ↓
     Aplicações / Análises
```

Arquitetura pensada para:

* simplicidade
* evolução contínua
* escalabilidade futura

---

## **API – Endpoints (exemplos)**

```http
GET /api/v1/markets
GET /api/v1/markets/{symbol}
GET /api/v1/markets/{symbol}/history?start=YYYY-MM-DD&end=YYYY-MM-DD
```

>  Endpoints serão evoluidos durante o MVP.

---

## **SDKs Oficiais (em desenvolvimento)**

Além da API REST, o Uendze disponibilizará **SDKs oficiais** para facilitar o consumo dos dados.

###  Objetivo dos SDKs

* Eliminar chamadas HTTP manuais
* Reduzir erros de integração
* Aumentar produtividade

### Exemplo — SDK Python (planeado)

```python
from uendze import Client

client = Client(api_key="SUA_API_KEY")

markets = client.markets.list()

history = client.markets.history(
    symbol="BFAAA",
    start="2024-01-01",
    end="2024-01-31"
)
```

>  SDKs serão lançados após estabilização do MVP da API.

---

## **Tecnologias Utilizadas (MVP)**

| Camada         | Tecnologia         |
| -------------- | ------------------ |
| Backend        | Python, FastAPI    |
| ORM            | SQLAlchemy         |
| Validação      | Pydantic           |
| Banco de Dados | SQLite inicialmente/PostgreSQL(depois)  |
| Infra          |  ainda sem infra   |
| Docs           | OpenAPI (Swagger)  |



---

<div align="center">

**Uendze.**

</div>
