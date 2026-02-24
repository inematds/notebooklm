# TODO — Curso NotebookLM Completo

> Gerenciamento do fluxo de criação do curso
> Padrão técnico: `ref/MASTER_COMPLETO.md` | QA: `ref/CHECKLIST_REVISAO.md`

---

## Estrutura do Curso

```
Trilha 1 (Emerald) — Fundamentos e Ferramentas  [Módulos 1.1 a 1.4]
Trilha 2 (Blue)    — Aplicação e Domínio         [Módulos 2.1 a 2.5 + Bônus]
```

---

## Status Geral

| Página | Arquivo | Status |
|--------|---------|--------|
| Landing Page | `index.html` | ✅ Criado |
| Trilha 1 — Index | `curso/trilha1/index.html` | ✅ Criado |
| Módulo 1.1 — Introdução | `curso/trilha1/modulo-1-1.html` | ✅ Criado |
| Módulo 1.2 — Fontes | `curso/trilha1/modulo-1-2.html` | ✅ Criado |
| Módulo 1.3 — Chat | `curso/trilha1/modulo-1-3.html` | ✅ Criado |
| Módulo 1.4 — Studio | `curso/trilha1/modulo-1-4.html` | ✅ Criado |
| Trilha 2 — Index | `curso/trilha2/index.html` | ✅ Criado |
| Módulo 2.1 — Casos de Uso | `curso/trilha2/modulo-2-1.html` | ✅ Criado |
| Módulo 2.2 — Colaboração | `curso/trilha2/modulo-2-2.html` | ✅ Criado |
| Módulo 2.3 — Hacks Avançados | `curso/trilha2/modulo-2-3.html` | ✅ Criado |
| Módulo 2.4 — Boas Práticas | `curso/trilha2/modulo-2-4.html` | ✅ Criado |
| Módulo Bônus — Projetos | `curso/trilha2/modulo-2-bonus.html` | ✅ Criado |

---

## TRILHA 1 — Fundamentos e Ferramentas (Emerald)

### ✅ index.html — Landing Page
- [x] Nav: Logo + INEMA.CLUB + Trilhas + Theme Toggle
- [x] Hero: título, descrição, stats (2 trilhas, 8+ módulos, 50+ tópicos, ~10h)
- [x] Cards das 2 trilhas com módulos listados
- [x] Seção "Por que aprender NotebookLM?"
- [x] Footer
- [x] Dark/light mode

### ✅ curso/trilha1/index.html — Índice da Trilha 1
- [x] Nav com trilha 1 ativa (emerald)
- [x] Header: gradiente emerald, stats (4 módulos, 27 tópicos, ~4h, Básico)
- [x] Seção 1: Navegação rápida (4 cards simples clicáveis — `<a>`, sem botões)
- [x] Seção 2: Cards detalhados com tópicos expansíveis
  - [x] Módulo 1.1 — 6 tópicos com 3 seções cada
  - [x] Módulo 1.2 — 7 tópicos com 3 seções cada
  - [x] Módulo 1.3 — 6 tópicos com 3 seções cada
  - [x] Módulo 1.4 — 6 tópicos com 3 seções cada
- [x] Modais com iframe para cada módulo
- [x] Botões ESQUERDA (justify-start)
- [x] Números em círculo (não setas)
- [x] Navegação: Voltar / Próxima Trilha

### ✅ curso/trilha1/modulo-1-1.html — Introdução e Contexto
- [x] Nav + Breadcrumb
- [x] Header: gradiente emerald, stats (6 tópicos, 30 min, Básico, Teoria)
- [x] Tópico 1: O que é o NotebookLM (Conceito + Dados + Dica)
- [x] Tópico 2: História e Evolução (Timeline)
- [x] Tópico 3: A Tecnologia RAG (Conceito + Grid fazer/evitar)
- [x] Tópico 4: NotebookLM vs Concorrentes (Comparação + Dica)
- [x] Tópico 5: Planos e Preços (Conceito + Dica prática)
- [x] Tópico 6: Primeiros Passos (Timeline de passos)
- [x] Resumo final com checklist + próximo módulo

### ⬜ curso/trilha1/modulo-1-2.html — Fontes: O Coração do NotebookLM
**Tópicos planejados (7):**
1. O que são fontes e por que importam
2. Tipos de arquivo suportados (PDF, YouTube, Drive, etc.)
3. Carregando fontes corretamente
4. "Cirurgia nos documentos" — preparando para melhores resultados
5. Selecionando fontes específicas (checkboxes)
6. Integração com Google Drive (sincronização)
7. Limites e restrições importantes

### ⬜ curso/trilha1/modulo-1-3.html — Chat com Documentos
**Tópicos planejados (6):**
1. Interface de chat e citações clicáveis
2. Tipos de pergunta que funcionam melhor
3. Prompts básicos (resumo, explicação, comparação)
4. Prompts intermediários (análise crítica, contradições)
5. Super Prompts avançados da comunidade
6. O que o chat NÃO consegue fazer

### ⬜ curso/trilha1/modulo-1-4.html — Studio: Todas as Ferramentas
**Tópicos planejados (6):**
1. Notebook Guide (Study Guide, Briefing, FAQ, Glossário)
2. Audio Overview: geração e personalização
3. Audio Overview Interativo: entre na conversa
4. Mind Maps e visualizações interativas
5. Slide Decks e Infographics
6. Data Tables e Deep Research

---

## TRILHA 2 — Aplicação e Domínio (Blue)

### ⬜ curso/trilha2/index.html — Índice da Trilha 2
**Módulos (5):**
- 2.1 Casos de Uso Práticos
- 2.2 Colaboração e Compartilhamento
- 2.3 Hacks, Extensões e Fluxos Avançados
- 2.4 Boas Práticas, Limitações e Ética
- BÔNUS: Projetos Completos Guiados

### ⬜ curso/trilha2/modulo-2-1.html — Casos de Uso Práticos
**Tópicos planejados (7):**
1. NotebookLM para Estudantes
2. NotebookLM para Pesquisa Acadêmica
3. NotebookLM para Profissionais / Corporativo
4. NotebookLM para Criadores de Conteúdo
5. NotebookLM para Jornalistas
6. NotebookLM para Advogados e Compliance
7. NotebookLM para Educadores e Saúde

### ⬜ curso/trilha2/modulo-2-2.html — Colaboração e Compartilhamento
**Tópicos planejados (6):**
1. Permissões: Viewer vs Editor
2. Compartilhando via email e link público
3. Colaboração em tempo real
4. Analytics de uso (Plus)
5. NotebookLM Enterprise
6. Limites de compartilhamento por tipo de conta

### ⬜ curso/trilha2/modulo-2-3.html — Hacks, Extensões e Fluxos Avançados
**Tópicos planejados (7):**
1. Os 20+ hacks mais usados pela comunidade
2. Extensão Chrome: YouTube to NotebookLM
3. NotebookLM + Obsidian + Google Drive
4. Criando séries de podcasts multi-episódios
5. Análise de concorrentes com NotebookLM
6. Fluxo completo: pesquisa → análise → publicação
7. App mobile: recursos exclusivos

### ⬜ curso/trilha2/modulo-2-4.html — Boas Práticas, Limitações e Ética
**Tópicos planejados (6):**
1. Limitações reais descobertas pela comunidade
2. Taxa de alucinação: o que significa 13% vs 40%
3. Privacidade e segurança dos documentos
4. Uso ético em pesquisa e jornalismo
5. O que NÃO usar no NotebookLM
6. O futuro: o que esperar

### ⬜ curso/trilha2/modulo-2-bonus.html — Projetos Guiados
**Projetos planejados (4):**
1. Criar um curso com NotebookLM como base de pesquisa
2. Montar uma newsletter semanal automatizada
3. Revisão de literatura de 20 artigos em 2 horas
4. Criar um podcast de 5 episódios de um único livro

---

## Regras de Qualidade (ref/CHECKLIST_REVISAO.md)

Antes de marcar qualquer página como ✅, verificar:

- [ ] Botões à ESQUERDA (`justify-start`)
- [ ] Números em círculo (não setas)
- [ ] 3 seções por tópico
- [ ] INEMA.CLUB presente (`text-sky-400`)
- [ ] Light mode CSS incluído
- [ ] Título módulo `text-2xl`
- [ ] Dark/light mode funcionando
- [ ] Links corretos entre páginas
- [ ] Responsivo (mobile)

---

## Legenda

| Símbolo | Significado |
|---------|-------------|
| ✅ | Concluído e validado |
| 🔄 | Em progresso |
| ⬜ | Pendente |
| ⚠️ | Precisa revisão |
