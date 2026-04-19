<div align="center">

# Caio Wilker

**Full Stack Developer · Java & Spring Boot · React & TypeScript**

7º semestre · Engenharia da Computação · Minas Gerais, Brasil

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/caio-wilker-107a9032a)
[![GitHub](https://img.shields.io/badge/github.com/caiowilker-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/caiowilker)

</div>

---

Desenvolvo software com foco em **arquitetura, segurança e produto**. Trabalho no ciclo completo — modelagem de banco, API REST, frontend e infraestrutura — com atenção real às decisões de engenharia por trás de cada escolha.

Atualmente construindo o **Margin Engine**, SaaS B2B em produção com clientes reais, arquitetura multi-tenant e pipeline de billing integrado. **173 commits em abril de 2026** distribuídos entre backend, frontend e landing.

---

## Stack

| | |
|---|---|
| **Backend** | Java · Spring Boot · Spring Security · JWT · JPA / Hibernate · PostgreSQL |
| **Frontend** | TypeScript · React · Vite · React Query · Tailwind CSS |
| **Infra & Tooling** | Supabase · RLS · Git · Linux · Docker · GTM · LGPD/GDPR |

---

## Projeto principal

### [Margin Engine](https://marginengine.com.br) — SaaS B2B em produção

Software de controle de margem para açougues e supermercados. Calcula o custo real de cada corte a partir do preço da carcaça, monitora margem em tempo real e emite alertas antes de fechar no prejuízo.

**3 repositórios privados · backend (Java) + frontend (TypeScript) + landing (HTML)**

Decisões técnicas implementadas:

- **Multi-tenancy** com isolamento por `tenant_id` via Hibernate Filter — queries sempre escopadas, sem vazamento entre clientes
- **Auth stateless** com JWT + refresh token rotation, armazenamento em `sessionStorage` para mitigar XSS
- **Segurança de banco** com RLS em 8 tabelas: `ENABLE ROW LEVEL SECURITY` + policies `USING (false)` para roles públicos + `REVOKE` de privilégios — API REST pública bloqueada, backend Java com `BYPASSRLS`
- **LGPD/GDPR** com cookie de domínio pai (`.marginengine.com.br`) compartilhado entre landing e app — GTM e Meta Pixel bloqueados até aceite explícito, sem dark patterns
- **Performance** na landing: GTM lazy-loaded pós-interação, fontes com `media=print` swap, LCP < 2s
- **Billing** com planos, limites por feature, upgrade flow e webhooks

> Repositórios privados — código disponível para revisão sob solicitação.

---

## Projetos públicos

### [desafio-consulta-vendas](https://github.com/caiowilker/desafio-consulta-vendas) · ⭐ 581 · Java · Spring Boot

API REST de consulta e relatório de vendas. O projeto mais referenciado do perfil — Spring Boot, JPA e arquitetura em camadas. 581 pessoas salvaram como referência.

### [SIGE Automator 3.0](https://github.com/caiowilker/SIGE_Automator_3.0) · Python

Automação de cadastramento em massa de alunos em sistema de gestão escolar. Eliminou processo manual repetitivo com script de alta confiabilidade.

### [DSCommerce](https://github.com/caiowilker/dscommerce-main) · Java · Spring Boot

E-commerce com API REST completa, autenticação JWT e controle de perfis de acesso. Base sólida em Spring Security e modelagem de domínio.

### [rest-client](https://github.com/caiowilker/rest-client) · Java

Cliente HTTP para consumo de APIs REST externas. Estudo aplicado de integração entre serviços.

---

## Formação

**Bacharelado em Engenharia da Computação** — 7º semestre

Fundamentos aplicados diretamente ao código: estruturas de dados, algoritmos, sistemas operacionais, redes e engenharia de software.

---

## Estatísticas

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=caiowilker&show_icons=true&theme=tokyonight&include_all_commits=true&locale=pt-br&hide_border=true&count_private=true" height="160"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=caiowilker&theme=tokyonight&layout=compact&langs_count=6&hide_border=true" height="160"/>

</div>

---

<div align="center">
<sub>A maior parte do trabalho está em repositórios privados — o que importa está em produção.</sub>
</div>
