<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a3a2a,100:16a34a&height=200&section=header&text=Caio%20Wilker&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=Full%20Stack%20Developer%20%7C%20Java%20%26amp%3B%20Spring%20Boot%20%7C%20React%20%26amp%3B%20TypeScript&descSize=16&descAlignY=58&descColor=86efac" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](linkedin.com/in/caiowilker)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/caiowilker)
[![Margin Engine](https://img.shields.io/badge/Margin%20Engine-16a34a?style=for-the-badge&logo=rocket&logoColor=white)](https://marginengine.com.br)

<br/>

![Visitors](https://komarev.com/ghpvc/?username=caiowilker&color=16a34a&style=flat-square&label=visitas+ao+perfil)
![7º Semestre](https://img.shields.io/badge/7º%20Semestre-Engenharia%20da%20Computação-16a34a?style=flat-square)
![Minas Gerais](https://img.shields.io/badge/📍-Minas%20Gerais%2C%20Brasil-1a3a2a?style=flat-square&labelColor=0d1117&color=16a34a)

</div>

---

<img align="right" src="https://github-readme-stats.vercel.app/api/top-langs/?username=caiowilker&theme=tokyonight&layout=compact&langs_count=6&hide_border=true&count_private=true" width="300"/>

### Sobre mim

Desenvolvo software com foco em **arquitetura, segurança e produto**. Trabalho no ciclo completo — modelagem de banco, API REST, frontend e infraestrutura — com atenção real às decisões de engenharia por trás de cada escolha.

Atualmente construindo o **Margin Engine**, SaaS B2B em produção com clientes reais, arquitetura multi-tenant e pipeline de billing integrado.

> 🔥 **173 commits em abril de 2026** — backend, frontend e landing
> 📦 3 repositórios privados em produção ativa
> ⭐ 581 stars no projeto mais referenciado do perfil

<br clear="right"/>

---

## 🛠️ Stack

<div align="center">

#### Backend
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Hibernate](https://img.shields.io/badge/Hibernate-59666C?style=for-the-badge&logo=hibernate&logoColor=white)

#### Frontend
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

#### Infra & Tooling
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

</div>

---

## 🚀 Projeto principal

<div align="center">

[![Margin Engine](https://img.shields.io/badge/🥩%20Margin%20Engine-SaaS%20B2B%20em%20produção-16a34a?style=for-the-badge)](https://marginengine.com.br)

</div>

Software de controle de margem para açougues e supermercados. Calcula o custo real de cada corte a partir do preço da carcaça, monitora margem em tempo real e emite alertas antes de fechar no prejuízo.

```
margin-engine-back     → Java · Spring Boot · PostgreSQL · JWT · Multi-tenancy
margin-engine-front    → TypeScript · React · Vite · React Query · Tailwind
margin-engine-landing  → HTML · CSS · JS · GTM · Meta Pixel · LGPD
```

<details>
<summary><b>🔐 Decisões técnicas implementadas</b></summary>

<br/>

| Área | Decisão |
|------|---------|
| **Multi-tenancy** | Isolamento por `tenant_id` via Hibernate Filter — queries sempre escopadas, sem vazamento entre clientes |
| **Autenticação** | JWT + refresh token rotation, `sessionStorage` para mitigar XSS |
| **Segurança de banco** | RLS em 8 tabelas: `ENABLE ROW LEVEL SECURITY` + policies `USING (false)` + `REVOKE` para roles públicos. Backend com `BYPASSRLS` |
| **LGPD/GDPR** | Cookie de domínio pai `.marginengine.com.br` compartilhado entre landing e app — GTM e Meta Pixel bloqueados até aceite explícito |
| **Performance** | GTM lazy-loaded pós-interação, fontes com `media=print` swap, LCP < 2s |
| **Billing** | Planos, limites por feature, upgrade flow e webhooks |

</details>

> 🔒 Repositórios privados — código disponível para revisão sob solicitação

---

## 📂 Projetos públicos

<div align="center">

| Projeto | Stars | Stack | Descrição |
|---------|-------|-------|-----------|
| [desafio-consulta-vendas](https://github.com/caiowilker/desafio-consulta-vendas) | ⭐ **581** | ![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) Spring Boot | API REST de relatório de vendas. 581 devs salvaram como referência |
| [SIGE Automator 3.0](https://github.com/caiowilker/SIGE_Automator_3.0) | — | ![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white) | Automação de cadastramento em massa em sistema de gestão escolar |
| [DSCommerce](https://github.com/caiowilker/dscommerce-main) | — | ![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) Spring Boot | E-commerce com JWT, Spring Security e arquitetura em camadas |
| [rest-client](https://github.com/caiowilker/rest-client) | — | ![Java](https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) | Cliente HTTP para consumo de APIs REST externas |

</div>

---

## 📊 Estatísticas

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=caiowilker&show_icons=true&theme=tokyonight&include_all_commits=true&locale=pt-br&hide_border=true&count_private=true&ring_color=16a34a&icon_color=16a34a" height="170"/>
<img src="https://github-readme-streak-stats.herokuapp.com/?user=caiowilker&theme=tokyonight&hide_border=true&ring=16a34a&fire=16a34a&currStreakLabel=16a34a" height="170"/>

</div>

---

## 🎓 Formação

**Bacharelado em Engenharia da Computação** — 7º semestre

Fundamentos aplicados diretamente ao código de produção: estruturas de dados, algoritmos, sistemas operacionais, redes e engenharia de software.

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:16a34a,50:1a3a2a,100:0d1117&height=100&section=footer"/>

<sub>A maior parte do trabalho está em repositórios privados — o que importa está em produção.</sub>

</div>
