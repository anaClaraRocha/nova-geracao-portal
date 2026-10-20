# ⛪ Igreja Nova Geração — Portal Web

> Site institucional responsivo e dashboard administrativo para gestão de ministérios, eventos, batismos e relatórios de culto.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?logo=chartdotjs&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?logo=greensock&logoColor=black)

---

## 📌 Sobre o projeto

O **Portal Igreja Nova Geração** reúne duas frentes em um único repositório:

1. **Site institucional (landing page):** apresenta a igreja, os pastores, os horários de culto, os ministérios, os eventos e as localidades, com formulário de contato e links para as redes sociais.
2. **Dashboard administrativo:** área restrita, em estilo SaaS, para a liderança acompanhar e cadastrar ministérios, membros, eventos, batismos e a frequência dos cultos.

O projeto foi desenvolvido com **HTML, CSS e JavaScript puros**, sem back-end. Os dados do dashboard são persistidos no **LocalStorage** do navegador, e a estrutura está preparada para uma futura integração com uma API.

---

## ✨ Funcionalidades

### Site institucional

- Layout responsivo para celular, tablet e desktop
- Seções: hero, pastores, cultos, ministérios, online, eventos, localidades e rodapé
- Carrossel de eventos e modais de detalhes (evento e localidade)
- Formulário de contato com validação e proteção anti-spam (honeypot), enviado via [FormSubmit](https://formsubmit.co/)
- Animações de entrada com GSAP e revelação de seções com `IntersectionObserver`
- Botão flutuante de WhatsApp
- SEO básico com dados estruturados (JSON-LD, schema.org `Church`)
- Acessibilidade: `focus-visible`, skip-link e menu mobile navegável
- Acesso à área restrita pelo rodapé

### Dashboard administrativo

- **Login** com validação, opção "lembrar e-mail" e proteção de rotas por sessão
- **CockPit:** totalizadores (membros, ministérios, eventos, batismos e participantes do último culto), gráfico de frequência dos últimos cultos, próximos eventos e resumo geral
- **Ministérios:** CRUD de ministérios e de membros, com filtro por ministério
- **Eventos:** CRUD com upload de cartaz (convertido para Base64)
- **Batismo:** CRUD com listagem ordenada pela data do batismo
- **Relatório de Culto:** CRUD de registros de frequência por culto
- Tema **claro/escuro**
- Sidebar recolhível, header com notificações (eventos dos próximos 7 dias e aniversariantes do mês) e perfil editável
- Modais e toasts reutilizáveis em todas as telas
- Layout 100% responsivo

---
