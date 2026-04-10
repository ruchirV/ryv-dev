---
title: "StockTracker"
date: 2026-04-01
featured: true
description: "A full-stack, real-time stock price dashboard with AI chatbot."
tags: ["TypeScript","React","D3","NodeJS","AWS"]
link: "https://github.com/ruchirV/StockTracker"
weight: 100
type: "projects"
---
A full-stack, real-time stock price dashboard. Live WebSocket price feeds, D3 visualisations, price threshold alerts, and an AI portfolio chatbot for premium users.

Built as a portfolio project demonstrating real-time architecture, modern React patterns, type-safe full-stack TypeScript, and production-grade engineering practices.

---

### Features & Live Demo

The application is deployed on AWS cloud. Here are some of the features of the applications. 

- User registration with option to integrate using **Google** or **Github** accounts.
- Live tracking of stocks using [Finnhub API](https://finnhub.io/docs/api/websocket-trades) connected via websocket.
- Show Candle chart using **D3** by fetching data from [Yahoo Finance API](https://query1.finance.yahoo.com/v8/finance/chart/).
- AI Chat integration with LLM model **llama-3.1-8b-instant** using [Groq API](https://console.groq.com/docs/api-reference#chat-create).


[Click here](https://stocktracker.ruchirv.dev) for live demo.

---

### Tech Stack

#### Frontend

|                |                                             |
| -------------- | ------------------------------------------- |
| Framework      | React 18 + TypeScript (strict)              |
| Data fetching  | TanStack Query v5 (React Query)             |
| UI state       | Zustand                                     |
| Visualisations | D3.js                                       |
| Styling        | Tailwind CSS                                |
| Forms          | React Hook Form + Zod                       |
| Real-time      | Native WebSocket client                     |
| Performance    | TanStack Virtual (virtualised lists)        |
| Testing        | Vitest + React Testing Library + Playwright |
| Bundler        | Vite                                        |

#### Backend

|               |                                                |
| ------------- | ---------------------------------------------- |
| Runtime       | Node.js + TypeScript (strict)                  |
| Framework     | NestJS                                         |
| Database      | PostgreSQL (via Prisma ORM)                    |
| Cache + queue | Redis (ElastiCache) + BullMQ                   |
| Auth          | JWT (access + refresh rotation) + Passport.js  |
| Social auth   | OAuth 2.0 — Google, GitHub                     |
| Real-time     | NestJS WebSocket Gateway                       |
| Email         | Nodemailer + SendGrid                          |
| LLM           | Provider-agnostic adapter (OpenAI / Anthropic) |
| Testing       | Jest + Supertest                               |

#### Infrastructure

|                   |                           |
| ----------------- | ------------------------- |
| Cloud             | AWS                       |
| Frontend hosting  | S3 + CloudFront           |
| Backend compute   | ECS Fargate               |
| Database          | RDS PostgreSQL            |
| Cache             | ElastiCache Redis         |
| Load balancer     | Application Load Balancer |
| IaC               | Terraform                 |
| CI/CD             | GitHub Actions            |
| SAST              | CodeQL + SonarCloud       |
| Secret management | AWS Secrets Manager       |

---