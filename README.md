# Jose Eduardo Tirado Verbel · `jotive.dev`

**Backend Engineer** — Python · TypeScript · AI Integration

Backend engineer con 6+ años construyendo APIs y servicios que llegan a producción. Foco en diseño de API con trade-offs explícitos (cada decisión documentada como ADR), microservicios multi-tenant en Google Cloud, e integración real de LLMs en flujos de negocio.

Notas técnicas y proyectos en **[dev.jotive.com.co](https://dev.jotive.com.co)**.

---

## What I build

**Production APIs**
- REST con idempotency keys (Postgres unique + Redis lock), cursor pagination, rate limiting con token bucket Lua atómico, errores RFC 7807
- Microservicios multi-tenant en Cloud Run con signed URLs (GCS) y convención de keys por tenant
- Cada decisión técnica como Architecture Decision Record con alternativas rechazadas

**AI Integration (aplicado, no investigación)**
- Pipelines con Anthropic Claude Sonnet (incluyendo visión sobre URLs remotas) con manejo de quota y abort temprano en lugar de retry bobo
- Integración OpenAI Chat Completions dentro de pipelines FastAPI
- Clasificación de señales con LLM sobre datos scrapeados

**Infra**
- Bash idempotente para hardening de VPS (sshd, fail2ban, systemd user con CPU/RAM limits)
- Docker multi-stage + Compose como interfaz estándar
- CI/CD con GitHub Actions

---

## Featured engineering work

| Project | What it demonstrates | Stack |
|---|---|---|
| [order-processing-platform](https://github.com/jotive/order-processing-platform) | API design — idempotency dual-layer, cursor pagination, cache-aside, rate limit Lua, ADRs documentados | FastAPI · PostgreSQL 16 · Redis 7 · SQLAlchemy 2.0 · Alembic · Docker |
| [llm-rag-platform](https://github.com/GeosData/llm-rag-platform) | Pipeline RAG con citas a fuente, ADR sobre vector store (Qdrant vs pgvector) | FastAPI · Qdrant · OpenAI · SQLAlchemy 2.0 · Alembic |
| [smartshop](https://github.com/GeosData/smartshop) | Backend SaaS multi-tenant, JWT auth, ADRs sobre tenancy y autenticación | FastAPI · PostgreSQL · Redis · JWT |
| [coding-interviews-prep](https://github.com/jotive/coding-interviews-prep) | Algoritmos con análisis de complejidad O(t)/O(s) y pytest. Trade-offs explícitos sobre código clever | Python 3.11+ · pytest |
| [network-scanner](https://github.com/jotive/network-scanner) | CLI cross-platform sin dependencias para escanear red local | Python 3 |

> Más proyectos y notas técnicas en **[dev.jotive.com.co](https://dev.jotive.com.co)**.

---

## Tech stack

**Languages:** Python · TypeScript · JavaScript
**Backend frameworks:** FastAPI · Express · Pydantic v2 · SQLAlchemy 2.0 · Alembic
**Databases:** PostgreSQL · Azure SQL · Cosmos DB · Redis · SQLite
**AI / LLM:** Anthropic Claude API (incl. vision) · OpenAI API
**Cloud (Experience):**
- **Azure** — App Service · Container Apps · Storage (Blob, Queue, Table) · Service Bus · Event Grid · Event Hubs · Key Vault · Application Insights · Log Analytics · API Management · Entra ID · Azure DevOps
- **AWS** — Lambda · EC2 · S3 · API Gateway · SES · SNS · SQS

**Cloud (Familiarity):** Google Cloud (Cloud Run · GCS · signed URLs)
**DevOps:** Docker · GitHub Actions · Azure DevOps · Caddy · nginx · fail2ban · systemd
**Frontend (when needed):** React · Next.js 16 · Astro · Tailwind CSS · Zustand
**Auth & security:** JWT (`jose`) · Google OAuth · API key + bearer · multi-tenant patterns

**Knowledge / not yet evidenced in public code:** Kubernetes · Terraform · Prometheus · Grafana · vector DBs (pgvector, Qdrant) · LangChain / LangGraph · MongoDB.

---

## Connect

[dev.jotive.com.co](https://dev.jotive.com.co) · [LinkedIn](https://www.linkedin.com/in/jotive/) · jotive@gmail.com

---

*Systems Engineering BSc · Backend Engineer · Monteria, Colombia · Remote (UTC-5) · English B1-B2 (improving)*
