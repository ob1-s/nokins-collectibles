## 1. Visão Geral do Produto

* **Nokins Colecionáveis**

* **Resumo Executivo** (a ser preenchido)

* **O que é o produto?**

  * Plataforma web para colecionar, visualizar e comprar personagens digitais.

* **Qual problema/necessidade ele resolve?**

  * Facilita a experiência de colecionismo digital sem complexidade técnica, com pagamentos tradicionais.

* **Público‑alvo principal.**

  * Usuários interessados em colecionar personagens virtuais, fãs de cultura pop e jogos casuais.

---

## 2. Objetivos e Métricas de Sucesso

* **Objetivos de Negócio** (a ser preenchido)

  * Ex.: aumentar engajamento, aquisição de novos usuários, receita média por compra.

* **KPIs Principais**

  * Nº de usuários ativos diários (DAU)
  * Nº de compras concluídas por dia
  * Taxa de conversão no fluxo de checkout

---

## 3. Escopo do Produto

* **Funcionalidades Principais (v0)**

  1. Login/Registro de usuários (e-mail/senha ou OAuth)
  2. Lista de personagens disponíveis (banca)
  3. Inventário do usuário (coleção própria)
  4. Loja de personagens (catálogo e filtros)
  5. Página de detalhe de cada personagem
  6. Fluxo de compra e checkout (pagamento tradicional)

* **Funcionalidades Desejáveis (fora de v0)**

  * Filtros avançados (raridade, tema)
  * Wishlists e notificações de reposição
  * Sistema de pontos e recompensas

* **Não‑Funcionalidades (fora de escopo)**

  * Gamificação complexa (níveis, conquistas)
  * Integração blockchain ou criptomoedas

---

## 4. Personas e Jornada do Usuário

| Etapa        | Ação do Usuário                          | Emoção      | Possíveis Bloqueios           |
| ------------ | ---------------------------------------- | ----------- | ----------------------------- |
| Descoberta   | Vê anúncio e acessa landing page         | Curioso     | Falta de clareza no valor     |
| Onboarding   | Cria conta e faz login                   | Empolgado   | Formulário longo              |
| Exploração   | Navega pela banca de personagens         | Interessado | Catálogo extenso sem filtro   |
| Visualização | Entra na página de detalhe do personagem | Engajado    | Informações insuficientes     |
| Compra       | Adiciona ao carrinho e finaliza checkout | Satisfeito  | Falta de métodos de pagamento |
| Pós‑compra   | Confere inventário com novo personagem   | Realizado   | Latência na atualização       |

---

## 5. Requisitos Funcionais

| ID     | Requisito                                                       | Prioridade | Responsável  |
| ------ | --------------------------------------------------------------- | ---------- | ------------ |
| RF-001 | Usuário pode criar conta e fazer login/logout                   | Alta       | Frontend     |
| RF-002 | Exibir lista de personagens disponíveis com imagem e nome       | Alta       | Frontend     |
| RF-003 | Exibir inventário do usuário com seus personagens coletados     | Alta       | Frontend     |
| RF-004 | Exibir página de detalhe: atributos, lore e preço do personagem | Alta       | Frontend     |
| RF-005 | Fluxo de seleção, adição ao carrinho e resumo de compra         | Alta       | Frontend     |
| RF-006 | Integração com gateway de pagamento (checkout)                  | Alta       | Frontend/API |

---

## 6. Requisitos Não‑Funcionais

* **Segurança**: comunicação HTTPS, validação de formulários
* **Performance**: tempo de carregamento das páginas < 2s
* **Disponibilidade**: protótipo hospedado, sem SLA rígido
* **Usabilidade/UX**: design responsivo (mobile-first)

---

## 7. Arquitetura de Alto Nível (Front‑end)

* **Framework**: Vue.js ou React
* **Estilização**: Tailwind CSS
* **State Management**: Pinia/Vuex ou Redux
* **Autenticação**: JWT via API
* **Integração**:

  * API REST para personagens, inventário e checkout
  * Gateway de pagamento (Stripe, PayPal)

---

## 8. Fluxos e Wireframes

* **Fluxo de Login**: Tela de boas‑vindas → Formulário de login/registro → Redireciona para banca
* **Fluxo de Compra**: Banca → Página do personagem → Adicionar ao carrinho → Checkout → Confirmação
* **Wireframes**: links ou anexos pendentes (FIGMA)

---

## 9. Plano de Lançamento e Go‑to‑Market

* Protótipo interno para validação de UI/UX
* Teste com grupo controlado de usuários (beta)
* Feedback e ajustes
* Apresentação para stakeholders e definição de roadmap completo

---

## 10. Glossário

* **Personagem**: item colecionável digital com atributos e lore
* **Banca**: catálogo de personagens disponíveis para compra
* **Inventário**: coleção pessoal de personagens do usuário
* **Carrinho**: lista temporária para compra
* **Checkout**: processo de pagamento tradicional
