# EstacionaFácil — Sistema Inteligente de Análise de Satisfação

> **Aprendizagem por Projetos — 4º ADS/SI (2026-2)**[cite: 32]  
> **Desafio:** *Como interpretar automaticamente o que os clientes dizem sobre nossos serviços para melhorar a tomada de decisão em um estacionamento com portfólio amplo e crescente?*[cite: 32]

---

## Sobre o Projeto

O **EstacionaFácil** é um estacionamento tradicional com mais de 20 anos de história que expandiu seu portfólio para acompanhar a concorrência, passando a oferecer vagas cobertas, planos mensais e semanais, atendimento para motos e veículos de grande porte, pernoite, reservas via aplicativo, manobrista, lava-jato, estética automotiva e novos meios de pagamento (Pix e cartão)[cite: 32].

Com o crescimento do volume de atendimentos e canais de avaliação, a análise manual tornou-se inviável[cite: 32]. Este projeto especifica e modela uma solução computacional baseada em **Processamento de Linguagem Natural (NLP)** para extrair automaticamente os principais pontos de serviço dos feedbacks dos clientes, classificar sentimentos e apresentar indicadores gerenciais e alertas automáticos ao diretor operacional[cite: 32, 33].

---

## Estrutura do Repositório

A organização deste repositório segue boas práticas de **Gerenciamento de Configuração** para rastreabilidade dos artefatos produzidos[cite: 32, 35]:

* **`/docs`** — Documentação oficial do projeto:
  * `Documento_de_Visao_EstacionaFacil.pdf` *(Entrega 1 — 20/11)*
  * `desafio_estacionafacil_preenchido.docx` *(Ficha de Requisitos Cliente-Professor e Equipe)*[cite: 32, 35]
  * `Plano_de_Qualidade_e_Metricas.pdf`
* **`/modelagem/uml`** — Diagramas UML do sistema[cite: 35]:
  * Diagrama de Casos de Uso[cite: 35]
  * Diagrama de Atividades (Processo)[cite: 35]
  * Diagrama de Classes (Entidades de Negócio/Banco)[cite: 35]
  * Diagrama de Sequência[cite: 35]
* **`/modelagem/banco`** — Modelagem de dados[cite: 35]:
  * Modelo Entidade-Relacionamento (`DER_EstacionaFacil.mwb` — MySQL Workbench)[cite: 35]
  * Script SQL de criação das tabelas (`schema.sql`)
* **`/prototipo`** — Prototipação de interfaces[cite: 35]:
  * Link do Figma: `[Inserir link do protótipo no Figma aqui]`[cite: 35]
  * Telas exportadas do painel gerencial e configuração de alertas[cite: 33, 35]

---

## Escopo Principal (Resumo dos Requisitos)

* **Classificação Automática por Serviço:** Categorização dos feedbacks entre vaga avulsa, vaga coberta, lava-jato, estética, manobrista, app/reserva, pernoite e contrato mensal[cite: 32].
* **Análise de Sentimento e Indicadores:** Extração de polaridade e consolidação de métricas de satisfação no painel gerencial[cite: 32, 33].
* **Alertas Automáticos:** Notificação ao gestor sempre que o índice de satisfação de um serviço ficar abaixo do limiar configurado[cite: 33].
* **Filtros Analíticos:** Segmentação das análises por período, tipo de contrato (avulso, semanal, mensal) e categoria de veículo (carro pequeno, carro grande, moto)[cite: 33].
* **Desempenho:** Capacidade de processar lotes de até 1.000 avaliações em menos de 1 minuto[cite: 33].

---

## 🔄 Política de Controle de Versão (Gestão de Configuração)

Para garantir a integridade dos entregáveis e a qualidade do projeto, a equipe adota o seguinte fluxo de trabalho no GitHub[cite: 35]:

1. **Estrutura de Branches:**
   * `main`: Contém exclusivamente versões estáveis, revisadas e prontas para entrega[cite: 35].
   * `develop`: Branch de integração dos artefatos da equipe antes da revisão final.
   * `docs/*` e `feat/*`: Branches específicas por tarefa (ex: `docs/documento-visao`, `feat/der-mysql`, `feat/uml-classes`).
2. **Padrão de Commits:** Uso de prefixos semânticos (`docs:`, `feat:`, `fix:`, `refactor:`).
3. **Revisão por Pares:** Todo *Pull Request* destinado à `develop` ou `main` passa pela revisão de pelo menos um integrante da equipe antes do *merge*[cite: 22].

---

## Cronograma de Entregas

| Data | Marco / Entregável | Status |
| :--- | :--- | :---: |
| **24/08/2026** | Apresentação da proposta inicial pelo Cliente-Professor (v1.0)[cite: 33] | ✅ Concluído |
| **06/11/2026** | Definição de atributos de qualidade, métricas e gestão de configuração[cite: 35] | 🔄 Em andamento |
| **20/11/2026** | **1ª Entrega:** Documento de Visão (PDF), Requisitos, Protótipo e Modelagens (UML/DER)[cite: 35] | 🔄 Em andamento |

---

## 👥 Equipe

* **[Seu Nome Completo]** — `[Papel, ex: Requisitos / Documentação / Banco de Dados]`
* **[Nome do Integrante 2]** — `[Papel, ex: Modelagem UML / Protótipo Figma]`
* **[Nome do Integrante 3]** — `[Papel, ex: Qualidade / Métricas / GitHub]`
* **[Nome do Integrante 4]** — `[Papel]`
