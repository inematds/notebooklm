# Análise dos Arquivos ref/ — Padrão Técnico do Curso

> Gerado em: Fevereiro 2026

---

## O que foi encontrado

A pasta `ref/` contém um **sistema de design completo e padronizado** para construir cursos como páginas HTML estáticas com Tailwind CSS. São dois documentos técnicos de referência obrigatória.

---

## MASTER_COMPLETO.md (v2.0 — jan/2026)

O "livro de regras" definitivo. Cobre:

### Erros Críticos — Nunca Cometer
1. **Botões SEMPRE à esquerda** — `justify-start`, nunca `justify-center`
2. **Números em círculo nos tópicos** — não usar setas (▶)
3. **3 seções obrigatórias por tópico** expansível: "O que é", "Por que aprender", "Conceitos-chave"
4. **INEMA.CLUB em todas as páginas** — `text-sky-400`, ao lado do logo
5. **Light mode CSS obrigatório** — bloco de overrides em todas as páginas
6. **Título do módulo com `text-2xl`** — nunca menor

### Sistema de Cores por Trilha
| Trilha | Cor | Classe principal |
|--------|-----|-----------------|
| T1 | Emerald | `text-emerald-400` |
| T2 | Blue | `text-blue-400` |
| T3 | Purple | `text-purple-400` |
| T4 | Amber | `text-amber-400` |
| T5 | Teal | `text-teal-400` |
| T6 | Rose | `text-rose-400` |

- **Primary (Yellow)**: `#FACC15` — Logo, CTAs, destaques
- **Sky**: `text-sky-400` — Link INEMA.CLUB
- **Dark mode**: dark-900/800/700/600 customizados

### Estrutura de Projeto
```
projeto/
├── index.html
├── curso/
│   ├── trilha1/
│   │   ├── index.html
│   │   ├── modulo-1-1.html
│   │   └── ...
│   └── trilha2/
├── docs/
└── ref/
```

### Estrutura de Páginas

**Página de Trilha (index):**
- Nav global (logo + INEMA.CLUB + trilhas + theme toggle)
- Header com gradiente da cor da trilha
- Stats Grid (4 colunas: Módulos, Tópicos, Duração, Nível)
- Seção 1: Cards simples clicáveis (grid 2 cols) — `<a>` sem botões
- Seção 2: Cards detalhados com tópicos expansíveis (6-8 por módulo)
- Botões: "Ver em Modal" + "Ver Completo" (ESQUERDA - justify-start)
- Modal com `<iframe>` carregando a página completa do módulo

**Página de Módulo:**
- Nav idêntica + Breadcrumb
- Header com gradiente
- 6 tópicos ricos com seções variadas
- Resumo final com checklist + próximo módulo

### Componentes Disponíveis
- Box Conceito Principal (gradiente da trilha)
- Box Dados/Pesquisa (blue)
- Box Dica Prática (primary/yellow)
- Grid Fazer vs Evitar (emerald/red)
- Timeline de passos
- Box de Alerta (red)
- Número em círculo (pequeno w-6 e grande w-12)
- Tópico expansível com 3 seções
- Breadcrumb
- Resumo do módulo com navegação

### Tecnologias
- HTML5 + Tailwind CSS (CDN)
- Fonte Inter (Google Fonts)
- JavaScript vanilla (toggleTopic, theme toggle, modal com iframe)
- Dark/light mode via classe `dark` no `<html>`
- localStorage para persistir tema

---

## CHECKLIST_REVISAO.md (v1.5 — jan/2026)

Lista de verificação QA para cada página antes de publicar. Cobre:

### Erros Críticos (verificar primeiro)
- [ ] Botões à ESQUERDA (justify-start)
- [ ] Números em círculo (não setas)
- [ ] 3 seções por tópico
- [ ] INEMA.CLUB presente (sky-400)
- [ ] Light mode CSS incluído
- [ ] Título módulo text-2xl
- [ ] TODOS os módulos completos (não só header+botão)
- [ ] Modal com iframe (não conteúdo duplicado)
- [ ] Seção de cartões simples clicáveis no index

### Checklists Específicos
- Página de Trilha: Nav, Header, Cards de Módulo, Funcionalidade, Responsividade
- Página de Módulo: Nav, Breadcrumb, Header, Tópicos (6 sections ricas), Resumo Final
- Página de Slides: Estrutura, Layout, Conteúdo detalhado, Funcionalidade
- JavaScript: toggleTopic, theme toggle, modal (open/close/ESC)
- CSS: Inter, light mode overrides completo

### Erros Mais Comuns
| Erro | O que verificar |
|------|-----------------|
| Botões centralizados | Procurar `justify-center` nos botões de módulo |
| Setas em tópicos | Procurar `▶` ou `→` nos tópicos |
| Faltando INEMA.CLUB | Verificar navigation |
| Light mode quebrado | Testar alternando o tema |
| Título pequeno | Verificar `text-2xl` no h3 do módulo |
| Modal sem iframe | Modal DEVE usar `<iframe src="modulo-X-X.html">` |
| Cartões simples com botões | Seção 1 usa `<a>` clicável, SEM botões |

---

## Implicação para o Projeto

O curso NotebookLM deve ser construído como um **site web estático** seguindo este padrão. Cada página é um arquivo HTML independente que segue rigorosamente o design system definido no MASTER_COMPLETO.md e validado pelo CHECKLIST_REVISAO.md.
