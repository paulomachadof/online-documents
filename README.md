# radix-docs

Documentação técnica do projeto **RADIX** — Backend Foundation & Frontend Foundation.

Repositório mantido pela equipe de Product Management / Requirements Engineering.

---

## Conteúdo

### `azure_devops_hierarchy.html`

Fluxograma interativo da hierarquia de work items no Azure DevOps, gerado a partir da reunião de Backlog Review de 21/05/2026.

**Funcionalidades:**
- Visualização dos 5 níveis da hierarquia: Iniciativa → Épico → Feature → PBI → Task
- Toggle interativo entre as duas opções em discussão para o nível de Feature:
  - **Opção A** — Feature = componente individual
  - **Opção B** — Feature = grupo/categoria de componentes
- Clique em cada nó para ver detalhes, regras e status da decisão
- Indicação visual de itens ✅ definidos vs ⚠️ em aberto

**Como visualizar:**
Acesse via GitHub Pages: `https://<seu-usuario>.github.io/radix-docs/azure_devops_hierarchy.html`

---

## Hierarquia de Work Items — Resumo

| Nível | Tipo | Representa | Status |
|---|---|---|---|
| 1 | Iniciativa | Objetivo estratégico de longo prazo | ✅ Definido |
| 2 | Épico | Release / versão de entrega (ex: Release 1) | ✅ Definido |
| 3 | Feature | Componente individual **ou** grupo? | ⚠️ Em aberto |
| 4 | PBI | Incremento de valor entregável | ✅ Definido |
| 5 | Task | Atividade técnica efêmera (vive na sprint) | ✅ Definido |

> **Nível 3 em aberto:** aguardando lista de componentes do JP (prazo: 22/05) para definição final entre Opção A e Opção B.

---

## Decisões definidas na reunião (21/05/2026)

- Épicos representam **Releases/Versões** — não épicos de negócio genéricos
- Versionamento de componentes via novos Épicos: **v0 → v1 → v2**
- PBIs são incrementos fecháveis — evoluções futuras geram novos PBIs
- Tasks têm granularidade máxima de **1 dia** de trabalho
- Componentes de design são **predecessores** das features de implementação
- Carry-over de PBIs suportado via toggle no Azure DevOps
- Changelog será centralizado no ADO (formato a definir)

---

## Ponto em aberto — Feature vs Componente

### Opção A — Feature = componente individual
- Épico = release · Feature = componente (ex: Gauge Chart) · PBI = entregável técnico interno
- ✅ Rastreabilidade individual por componente
- ⚠️ Componentes simples ficam granulares demais como Feature

### Opção B — Feature = grupo de componentes
- Épico = release · Feature = categoria (ex: Charts, Inputs) · PBI = componente individual
- ✅ Alinha com estrutura da equipe de design; catálogo mais limpo
- ⚠️ Perde rastreabilidade do ciclo de vida por componente

**Decisão pendente** após recebimento da lista de componentes do JP.

---

## Ações definidas

- [ ] **JP** — Enviar lista de componentes (Backend + Frontend) até 22/05 EOD
- [ ] **Equipe** — Publicar lista na Wiki do Azure DevOps
- [ ] **JP** — Mapear dependências entre Foundation e projeto OE (nível de features)
- [ ] **Equipe** — Reestruturar features do Frontend agrupando componentes pequenos
- [ ] **Leandro / Design** — Vincular componentes de design como predecessores das features
- [ ] **João Paulo** — Alinhar processo de aprovação com Madir antes de compartilhar
- [ ] **Mari** — Finalizar dashboards de Power BI até fim do sprint atual

---

## Links

- 📋 [Página no Notion — Backlog Review Resumo](https://www.notion.so/367906c40ea3813e8d7dc852306d93d1)
- 📝 [Transcrição original da reunião](https://www.notion.so/367906c40ea380788404e523bec91a05)

---

*Documentação gerada por Claudia — AI Agent de Requirements Engineering · 21/05/2026*
