<div align="center">

<img src="./img/uendze-logo.png" alt="Uendze Logo" width="320" />

# 🇦🇴 Uendze

### Plataforma de Dados Financeiros do Mercado Angolano

**API e SDKs para acesso estruturado, simples e confiável aos dados financeiros de Angola.**

🚧 **Status:** MVP em desenvolvimento

</div>

---

## 📌 O que é o Uendze?

O **Uendze** é uma plataforma tecnológica criada para resolver um problema real: a **falta de acesso simples, padronizado e programável a dados financeiros do mercado angolano**.

O projeto nasce com uma abordagem **API First**, focada em desenvolvedores, analistas e startups que precisam consumir dados financeiros de forma confiável.

> 🎯 **Foco atual:** construir um MVP sólido, simples e bem estruturado.

---

## 🎯 Objetivo do Projeto

* Criar a **primeira base moderna de dados financeiros focada em Angola**
* Disponibilizar esses dados via **API REST clara e previsível**
* Facilitar análises, estudos e desenvolvimento de produtos financeiros

> ⚠️ O foco inicial **não é escala**, mas **qualidade e validação técnica**.

---

## 👥 Público-Alvo

O Uendze foi pensado para:

* 👨‍💻 **Desenvolvedores** que precisam integrar dados financeiros
* 📊 **Analistas e pesquisadores**
* 🚀 **Startups e fintechs locais**
* 🎓 **Estudantes de tecnologia e finanças**

---

## ✅ Benefícios

✨ **Por que usar o Uendze?**

* 📊 Dados financeiros organizados e centralizados
* 🔌 API simples e fácil de consumir
* 🧠 Modelo de dados pensado para histórico e análises
* ⏱️ Menos tempo coletando dados, mais tempo analisando
* 🚀 Base preparada para evolução futura

---

## 🚧 Status do Projeto (MVP)

> ⚠️ **Em desenvolvimento ativo**

Atualmente em construção:

* Estrutura base da API
* Modelagem de dados
* Endpoints principais
* Pipeline inicial de ingestão de dados

Ainda **não recomendado para uso em produção**.

---

## 🧱 Arquitetura (Visão Geral)

```
Fontes de Dados (Angola)
          ↓
   ETL / Processamento
          ↓
   Banco de Dados
          ↓
      API REST
          ↓
  Clientes / Integrações
```

Arquitetura pensada para:

* simplicidade
* evolução contínua
* fácil manutenção

---

## 🔌 API — Endpoints Planejados

```http
GET /api/v1/markets
GET /api/v1/markets/{symbol}
GET /api/v1/markets/{symbol}/history?start=YYYY-MM-DD&end=YYYY-MM-DD
```

> ⚠️ Os endpoints podem sofrer ajustes durante o desenvolvimento do MVP.

---

## 🧠 Organização dos Dados (Resumo)

* **Market** → ativo financeiro
* **MarketDay** → data de negociação
* **MarketSummary** → preços e volume (OHLCV)

Modelo simples, extensível e orientado a dados históricos.

---

## 🛠️ Tecnologias Utilizadas

* **Backend:** Python + FastAPI
* **ORM:** SQLAlchemy
* **Validação:** Pydantic
* **Banco de Dados:** PostgreSQL / MySQL
* **Infraestrutura:** Linux, Docker
* **Documentação:** OpenAPI (Swagger)

---

## 📦 SDKs (Planejado)

Além da API, o Uendze terá **SDKs oficiais** para facilitar ainda mais o consumo dos dados.

### 🎯 Objetivo dos SDKs

* Abstrair chamadas HTTP
* Reduzir complexidade de integração
* Aumentar produtividade do desenvolvedor

### 🐍 SDK Python (primeiro)

Planejado para:

```python
from uendze import Client

client = Client(api_key="SUA_API_KEY")

markets = client.markets.list()
history = client.markets.history(
    symbol="BODIVA:ABC",
    start="2024-01-01",
    end="2024-01-31"
)
```

> ⚠️ SDKs serão lançados **após a estabilização do MVP da API**.

---

## 🛣️ Próximos Passos

* Finalizar MVP da API
* Validar dados do mercado angolano
* Publicar documentação inicial
* Criar SDK Python (primeira versão)
* Evoluir arquitetura conforme feedback

---

<div align="center">

**Uendze**
*Construindo a base de dados financeiros de Angola.*

</div>
