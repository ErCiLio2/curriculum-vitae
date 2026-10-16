# Ercílio Teixeira Júlio
**Engenheiro de Software Full Stack**

**Email:** erciliociu@gmail.com · **Telefone:** +244 973 087 388
**LinkedIn:** linkedin.com/in/erciliojulio · **GitHub:** github.com/ErCiLio2
**Luanda, Angola** · Nascido em 14 de julho de 2003

---

## Perfil

Engenheiro de Software Full Stack, cofundador e COO da SOMATEC (Software Marketing e Tecnologia), em Luanda. Técnico de TI desde 2018 (8+ anos) e engenheiro de software profissional desde 2023. Desenvolve plataformas SaaS, fintech e ERP para o mercado angolano, cobrindo o sistema inteiro: hardware, rede, servidor, base de dados, API e interface. Colabora com a ChimGam em desenvolvimento web e consultoria em TI. Estudante da 42 Luanda (nível 5.13 / 21), com base em programação de sistemas, algoritmos e C/C++.

---

## Experiência Profissional

| Período | Organização | Função |
|---|---|---|
| Jan 2023 – presente | **SOMATEC** | Cofundador e COO |
| 2024 – 2026 | **Júlios AN — Comércio Geral e Transportes** *(em simultâneo com a AS)* | Técnico Sénior de TI, Desenvolvedor Full Stack e DevOps |
| Mar 2023 – Jan 2026 | **AS Consulting & Investments** | Técnico Sénior de TI, Desenvolvedor Full Stack e DevOps |
| Jul – Set 2024 | **Grupo ZonaLink** | Desenvolvimento de software (PHP/Laravel) |
| 2018 – 2023 | **Freelance** | Técnico de TI e consultoria |

**Na SOMATEC** lidera técnica e operacionalmente produtos SaaS, fintech e ERP para o mercado angolano. **Na AS Consulting & Investments e Júlios AN** foi responsável por todo o parque informático, desenvolvimento de software e implantação e manutenção dos sistemas em produção.

---

## Competências Técnicas

| Área | Competências |
|---|---|
| **Linguagens** | TypeScript, JavaScript, PHP, Python, Java, Go, C, C++, SQL, HTML5, CSS3, Bash |
| **Frontend** | React, Next.js (App Router), Svelte / SvelteKit, Vite, Tailwind CSS (v3 e v4), Zustand, PWA e offline-first, design tokens, i18n, conversão Figma→código, acessibilidade WCAG 2.2 |
| **Backend** | NestJS, Fastify, Laravel, Django, FastAPI, Node.js, APIs REST, microserviços, Kafka, Zod |
| **Mobile e Desktop** | Flutter, React Native (Expo), Electron (IPC, contextBridge, builds NSIS), Tauri |
| **Bases de dados** | PostgreSQL, MySQL, MongoDB, SQLite, Redis; Prisma, Drizzle, TypeORM, Mongoose; MinIO / S3, Vercel Blob |
| **DevOps e Infra** | Docker, Docker Compose, Dokploy, Traefik, gestão de VPS, domínios .ao, SSL, backups, monitorização, GitHub Actions |
| **Monorepos e Build** | pnpm workspaces, Turborepo, tsup, esbuild, Turbopack, Nixpacks |
| **Integrações** | WhatsApp Cloud API, OTP / verificação de telefone, geração de PDF (WeasyPrint, jsPDF), QR codes, OCR (PaddleOCR), vídeo em tempo real (LiveKit), streaming (Bunny Stream) |
| **Arquitectura** | SaaS multi-tenant, Clean Architecture, API-first, offline-first, RBAC, SAGA, documentação técnica |
| **Segurança** | JWT, RBAC, OTP, HMAC-SHA256, AES-256-GCM, auditorias de segurança, cibersegurança OT/SCADA, CSIRT/CERT |
| **Programação de sistemas** | Syscalls POSIX, sinais Unix, threads e mutexes, gestão de memória, parsers, listas ligadas, árvores, raycasting, fractais |
| **POO** | Classes, herança, polimorfismo, classes abstractas, templates (C++) |
| **Suporte de TI** | Parque informático empresarial, hardware, Linux, virtualização, redes TCP/IP, DNS, e-mail, servidores web; manutenção e instalação de sistemas operativos e software aplicacional; manuseio e configuração de impressoras; suporte remoto (AnyDesk) |
| **Ferramentas de escritório e negócio** | Pacote Office (Word, Excel, PowerPoint), Primavera (módulo de Marketing e Vendas), AnyDesk |

---

## Portfolio de Projectos

### MESA Platform & Surface Manager · *SOMATEC · Em produção*

**Stack:** NestJS · SvelteKit · PostgreSQL · Redis · Prisma · Docker

ERP SaaS multi-tenant para farmácia, hotelaria, educação, restauração e retalho. Cada sector tem o seu *flavor* — tema visual, módulos activos e regras de negócio próprias — partilhando a mesma base de código e infraestrutura. O Surface Manager separa o plano de administração SaaS do espaço do cliente, com gestão de múltiplas subscrições num único painel.

- Isolamento por schema PostgreSQL por tenant; sistema de flavors sem fork de código
- Auditorias de UI periódicas para garantir paridade entre sectores

---

### Troco Seguro — Fintech e Mobilidade · *Em produção · Angola*

**Stack:** NestJS 11 · React/Vite · Tailwind CSS 4 · PostgreSQL · Redis · MinIO · Firebase · Docker · WhatsApp Cloud API

Plataforma completa de pagamentos e gestão de frotas para Angola: app mobile (motorista/passageiro), painel web (admin + gestor de frota) e API pública Troco Pay.

- Pagamentos QR em dois sentidos; anti-replay duplo (Redis + tabela de tokens usados); depósitos Multicaixa (webhook HMAC-SHA256)
- KYC via QR do BI; sistema de pânico/GPS; notificações multicanal (FCM, SMS, in-app)
- ~180 endpoints REST + Swagger; JWT + refresh silencioso; encriptação AES-256-GCM; locks pessimistas com retry em deadlock
- Testes: Jest (unitários) + Playwright E2E; CI com GitHub Actions

---

### FlyPort — SaaS B2B para Agências de Viagens · *flyport.tech · Em produção*

**Stack:** Django 6 · React 19 · Vite · Tailwind CSS 4 · PostgreSQL · Redis · Docker · Fabric.js · Travelport GDS

SaaS B2B para agências de viagens em Angola. Integra o GDS Travelport para extrair itinerários de PNRs e gera bilhetes em PDF com o branding de cada agência, através de editor visual em canvas. Modelo Trial / Starter / Professional.

- Backend Django 6 por domínios com fronteiras por import-linter; ~5 700 testes pytest em 8 fatias CI paralelas
- Migração progressiva Django → SPA React 19 — cada rota migrada remove o template no mesmo commit
- 9 tarefas Django-Q activas em produção; OpenAPI 3.1 gerado do código; Nginx + Cloudflare + SSL

---

### SaaS de Farmácia

**Stack:** NestJS · Kafka · Electron · PostgreSQL · Docker

Monorepo com microserviços NestJS e POS desktop offline em Electron. Kafka como bus de eventos; sincronização offline→online quando o terminal recupera ligação.

---

### WOL Commerce / WOL Loja

**Stack:** TypeScript · NestJS · React · MinIO · PostgreSQL

Comércio B2B e live commerce. Módulo de analytics construído de raiz; armazenamento centralizado de media em MinIO. Dashboard de gestão de vendas e inventário.

---

### iUConect — Plataforma de Serviços On-Demand · *SOMATEC*

**Stack:** TypeScript · NestJS · PostgreSQL · Redis · React Native · OTP · RBAC

Plataforma on-demand com quatro verticais de serviço. Arquitectura RBAC de dois planos — administração da plataforma separada do espaço do cliente. Autenticação OTP via SMS.

---

### Eduka — Plataforma de Explicações Online · *SOMATEC*

**Stack:** Fastify 5 · Prisma · PostgreSQL 16 · PgBouncer · Redis · MinIO · SvelteKit · Flutter

Ligação alunos ↔ tutores. Segurança reforçada: menores, documentos sensíveis (registo criminal, passaporte) e pagamentos.

- Módulos com fronteiras ESLint; contrato OpenAPI gerado do código; tipos TypeScript derivados automaticamente
- PostgreSQL 16 + PgBouncer; bus de eventos interno entre módulos

---

### FIP — Financial Intelligence Platform

**Stack:** FastAPI · Celery · SvelteKit 2 · Svelte 5 · PostgreSQL · Redis · MinIO · Alembic

Inteligência financeira com backend Python assíncrono (FastAPI + Celery) e frontend SvelteKit totalmente desacoplado — landing pública e dashboard autenticado.

---

### SeaOPEX — Sistema de Ship Chandling · *FreteMar / GOUV ESTÚDIO*

**Stack:** NestJS 10 · Next.js 14 · Prisma · PostgreSQL · TypeScript

Sistema operacional interno para empresa de Ship Chandling. JWT com refresh token httpOnly; proxy Next.js → NestJS.

---

### Outros projectos

**Uright · angoleva-transportes · guia turístico · catálogo de livros (PWA)** — Gestão associativa multi-tenant, transportes com QR e PDF, turismo e aplicação offline-first.

**Websites institucionais** — Ondas Marítimas e outros clientes, com optimização de performance e canvas animado.

**Infraestruturas críticas** — Proposta de cibersegurança OT/SCADA, CSIRT/CERT e protecção física no sector energético angolano.

**Go API** — API REST em Go (Gin) com PostgreSQL, MongoDB e protocolo QUIC/HTTP3.

---

## Formação

### 42 Luanda — Escola de Engenharia de Software
**Setembro 2024 – presente** · ISPTEC, Talatona, Luanda, Angola
**Nível actual:** 5.13 / 21 · **Tronco Comum concluído:** 57%

Formação por aprendizagem entre pares (peer-to-peer), sem professores nem aulas tradicionais. Modelo baseado em projectos práticos com avaliação pelos pares.

| Projecto | Horas | Resultado |
|---|---|---|
| cub3d — raycasting, motor 3D estilo Wolfenstein | 280H | Pass |
| minishell — shell completa com GNU Readline | 210H | Pass |
| Philosophers — concorrência: threads e processos | 70H | Pass |
| Libft — biblioteca C de raiz | 70H | Pass |
| fract-ol — gráficos 2D, fractais, miniLibX | 60H | Pass + bónus |
| NetPractice — redes TCP/IP, sub-redes, routing | 50H | Pass |
| minitalk — comunicação por sinais UNIX | 50H | Pass + bónus |
| Born2beroot — virtualização e administração de sistemas | 50H | Pass |
| push_swap — algoritmos de ordenação em pilha | 50H | Pass |
| get_next_line | 55H | Pass + bónus |
| ft_printf — funções variádicas | 55H | Pass |
| CPP Módulos 00–04 — POO em C++ | 70H | Pass |
| Exam Rank 02, 03, 04 | — | Pass |
| CPP Módulo 05 | 25H | Em progresso |

### Técnico Médio em Informática de Gestão
**IPAS Zango Zero** · 2021 – 2025

### Certificações e Cursos
Programação Web — MundoTec (mundotec.ao) · Informática na Óptica do Utilizador — Centro de Formação Profissional Nelpalma · Hardware e Software — Centro de Formação Profissional Nelpalma · Administração de Sistemas Linux — Udemy · Next.js App Router Fundamentals · React Foundations for Next.js · LinkedIn para Busca de Oportunidades

---

## Eventos e Participações

| Data | Evento | Representação |
|---|---|---|
| 16–18 Mai 2024 | **Unitel Startup Summit** — by Unitel | SOMATEC |
| 31 Ago 2024 | **Hackathon Academia BAI** | SOMATEC |

---

## Idiomas

Português (nativo) · Inglês (elementar)

## Em exploração

Kotlin · Armazenamento distribuído (SeaweedFS)
