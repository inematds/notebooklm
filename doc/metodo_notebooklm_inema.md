# Método INEMA: NotebookLM como Research, Script e Prompt Engineer (Passo a passo completo)

> Objetivo: transformar o **Google NotebookLM** em uma “máquina” de criação com IA:  
> **(1) Pesquisa confiável**, **(2) Roteiros no seu estilo**, **(3) Prompts profissionais com sintaxe correta**.

---

## 0) O que você vai construir

Você vai criar **3 notebooks** (um para cada função):

1. **Research Engine (Pesquisador)**  
   Um notebook que recomenda ferramentas e estratégias **somente com base nas fontes que você forneceu** (zero achismo).

2. **Script Engine (Roteirista no seu estilo)**  
   Um notebook treinado com seus próprios vídeos/textos para gerar roteiros **com sua identidade** (natural para fala).

3. **Prompt Engineering Engine (Engenheiro de prompt)**  
   Um notebook alimentado com **documentação oficial** dos modelos (imagem/vídeo) para gerar prompts **com sintaxe e parâmetros corretos**.

> Regra de ouro do NotebookLM: ele é **forte quando você dá boas fontes**. Ele não “adivinha” nem “se atualiza sozinho”.

---

## 1) Research Engine — Motor de Pesquisa de Ferramentas (sem hype)

### 1.1 Criar o notebook
- Abra o NotebookLM
- Clique em **Create new**
- Nome sugerido: **INEMA — Research Engine**

### 1.2 Adicionar fontes (o “cérebro”)
Aqui você vai adicionar **URLs e/ou PDFs** de fontes confiáveis, por exemplo:
- Diretórios de ferramentas de IA
- Newsletters e páginas de novidades
- Páginas oficiais de ferramentas (docs, pricing, requisitos)
- Comparadores/leaderboards de modelos
- Blogs técnicos respeitados

**Boas práticas**
- Prefira **páginas oficiais** e diretórios curados.
- Mantenha uma lista pequena e forte: **10 a 30 fontes** já é suficiente.
- Atualize 1x por semana (adicione links novos). O NotebookLM é **estático**.

### 1.3 Custom Instructions (copiar e colar)
Cole algo assim em **Custom instructions**:

> **INSTRUÇÕES — Research Engine**  
> Você é um consultor de ferramentas de IA para criadores de conteúdo no Brasil.  
> Use **somente** as fontes carregadas neste notebook.  
> Sua missão é recomendar uma stack prática para o meu cenário, respeitando: orçamento, nível, hardware, idioma e objetivo.  
> Evite soluções caras/enterprise.  
> **Formato de resposta obrigatório:**  
> 1) Recomendações por etapa (Pesquisa / Roteiro / Voz / Thumb / Edição / Publicação)  
> 2) Por que serve para minhas restrições  
> 3) Prós e contras  
> 4) Alternativa gratuita quando existir  
> 5) Checklist final (passos)

### 1.4 Prompt template (use sempre)
Copie e preencha:

**PROMPT — Research Engine (Template)**
- Objetivo do canal/negócio:  
- Nicho:  
- Público:  
- Orçamento: (ex: R$ 0 / R$ 100/mês)  
- Nível: (iniciante/intermediário)  
- Hardware: (Windows/Mac, RAM, GPU se tiver)  
- Prioridade: (velocidade / qualidade / custo)  
- Entregas: (roteiro, voz, thumb, vídeo)  
- Responder **somente com base nas fontes do notebook**.

### 1.5 Saída ideal (o que esperar)
Uma boa resposta do Research Engine entrega:
- Uma stack enxuta (poucas ferramentas)
- Um motivo claro para cada escolha
- Um plano de execução (checklist)

---

## 2) Script Engine — Roteiros com sua identidade (fala natural)

### 2.1 Criar o notebook
- **Create new**
- Nome sugerido: **INEMA — Script Engine**

### 2.2 Alimentar com seu estilo (fontes)
Você precisa subir “amostras” suas. Opções:
- Links de **5 a 15 vídeos** seus (os melhores e mais representativos)
- **Transcrições** (você pode colar texto de transcrição)
- Roteiros antigos (Google Docs/PDF/Markdown)
- Posts seus (threads, captions, e-mails)

**Dica prática**
- Comece com 5 vídeos TOP. Depois evolua para 10–15.
- Misture: vídeos “explicativos”, “vendas” e “conteúdo rápido”.

### 2.3 Custom Instructions (copiar e colar)
> **INSTRUÇÕES — Script Engine**  
> Você é meu roteirista e editor de roteiros.  
> Analise e imite meu tom: brasileiro, direto, com energia, didático e sem enrolar.  
> Escreva para ser falado (frases curtas, ritmo rápido, pausas).  
> Evite frases robóticas e clichês de IA.  
> Use: quebra de padrão, perguntas, curiosidade, micro-promessas, exemplos práticos.  
> **Estrutura padrão (Reels/TikTok 60s):**  
> - 0–2s: Hook (quebra de padrão)  
> - 2–6s: Promessa (o que vou ganhar)  
> - 6–40s: Passos (1–3 passos no máximo, bem visuais)  
> - 40–52s: Prova/Insight (por que funciona)  
> - 52–60s: CTA (curto e direto)  
> Mantenha minha personalidade.

### 2.4 Master Prompt (roteiro 60s pronto)
Copie e preencha:

**MASTER PROMPT — Script Engine (60s)**
- Tema do vídeo:  
- Objetivo: (reter / comentar / salvar / vender)  
- Público:  
- Tom: (mais agressivo / mais calmo / humor leve)  
- Conteúdo obrigatório (3 bullets):  
- CTA: (ex: “está no inema.club”)  
- Entregar: roteiro falado + versão curta (legenda).

### 2.5 Checklist de qualidade (roteiro viral)
Antes de publicar, confirme:
- Hook nos **2 primeiros segundos**
- 1 ideia principal (não 5)
- Frases curtas (fácil de falar no Heygen)
- Uma pergunta no meio
- Um “pattern interrupt” (ex: “para tudo”, “olha isso”)
- CTA simples e repetível

---

## 3) Prompt Engineering Engine — Prompts profissionais (sintaxe oficial)

> Este é o “motor” que mais muda resultado:  
> você para de escrever “prompt genérico” e começa a escrever **prompt que o modelo entende**.

### 3.1 Criar o notebook
- **Create new**
- Nome sugerido: **INEMA — Prompt Engineering Engine**

### 3.2 Coletar documentação oficial (PDF)
Para cada modelo (imagem/vídeo), busque:
- Documentação oficial (parâmetros, exemplos)
- Guia de boas práticas (quando oficial não existir)
- Restrições e formatos (aspect ratio, seed, negative prompt, etc.)

**Como salvar em PDF (recomendado)**
- Abra a página da doc
- **Ctrl+P (Windows) / Cmd+P (Mac)**
- Selecione **Salvar como PDF**
- Faça upload do PDF no NotebookLM

> Por que PDF? Links podem quebrar ou mudar; PDF “congela” a referência.

### 3.3 Custom Instructions (copiar e colar)
> **INSTRUÇÕES — Prompt Engineering Engine**  
> Aja como um engenheiro sênior de prompt.  
> Seu conhecimento é **estritamente limitado** às documentações carregadas neste notebook.  
> Use **apenas** parâmetros, sintaxe e recursos que existirem nas fontes.  
> Se eu pedir algo que não existe na doc, diga: “não encontrado na documentação” e proponha uma alternativa **dentro do que existe**.  
> **Formato de resposta obrigatório:**  
> 1) Prompt final (copiar e colar)  
> 2) Variação 1 (mais realista)  
> 3) Variação 2 (mais cinematográfica)  
> 4) Lista de parâmetros usados + por quê  
> 5) Checklist rápido de uso (onde colar, formato, proporção)

### 3.4 Prompt template (imagem)
Copie e preencha:

**PROMPT — Prompt Engineer (Imagem)**
- Modelo/ferramenta:  
- Objetivo: (thumbnail, capa, anúncio)  
- Assunto principal:  
- Estilo: (realista / cinematic / anime / etc.)  
- Ambiente:  
- Iluminação:  
- Câmera: (ângulo, lente, enquadramento)  
- Emoção:  
- Texto na imagem? (sim/não)  
- Restrições: (sem logos, sem marcas, sem gore, etc.)  
- Formato: (9:16 / 16:9 / 1:1)  
- Entregar **somente usando sintaxe da documentação carregada**.

### 3.5 Prompt template (vídeo)
Copie e preencha:

**PROMPT — Prompt Engineer (Vídeo)**
- Modelo/ferramenta:  
- Duração desejada:  
- Estilo:  
- Cena (o que acontece em 1 frase):  
- Movimento de câmera:  
- Movimento do personagem/objeto:  
- Ambiente / luz:  
- Qualidade desejada:  
- Formato: (9:16/16:9)  
- Restrições:  
- Explicar quais parâmetros foram usados e por quê.

---

## 4) Workflow completo (do zero ao post)

### 4.1 Fluxo recomendado (rápido)
1) **Research Engine** → escolhe stack e caminho  
2) **Script Engine** → gera roteiro 60s (fala natural)  
3) **Prompt Engineer** → cria prompt de thumb e/ou b-roll  
4) Produção (Heygen + editor)  
5) Publicação (título/legenda/CTA)

### 4.2 Checklist de publicação (Reels/TikTok)
- Gancho forte nos 2s iniciais
- Legendas grandes e curtas
- Cortes a cada 1–2s (se fizer sentido)
- Pergunta no final para comentários
- CTA em 1 frase: “Tá no inema.club”

---

## 5) Exemplos prontos (copiar e colar)

### 5.1 Prompt para o Script Engine (60s)
> Crie um roteiro falado de 60 segundos explicando o método de 3 motores no NotebookLM.  
> Use linguagem brasileira, direta, ritmo rápido.  
> Estrutura: Hook (0–2s), Promessa (2–6s), 3 passos (6–45s), Insight (45–55s), CTA (55–60s).  
> CTA: “tudo está no inema.club — você quer?”

### 5.2 Prompt para o Research Engine
> Quero montar um canal sobre IA para iniciantes no Brasil.  
> Orçamento: R$0–R$50/mês.  
> Hardware: Windows 8GB RAM.  
> Preciso: roteiro, voz, thumb, edição simples.  
> Recomende uma stack completa e explique por que serve para minhas restrições.  
> Responda somente com base nas fontes deste notebook.

### 5.3 Prompt para o Prompt Engineer (Thumbnail)
> Usando somente a documentação carregada, gere um prompt para uma thumbnail cinematográfica:  
> “cérebro de IA futurista brilhando, estilo high-end, contraste forte, foco no centro, fundo minimalista, sem texto, formato 16:9”.  
> Entregue prompt final + 2 variações + parâmetros usados.

---

## 6) Erros comuns e como corrigir

### 6.1 “O NotebookLM inventou coisa”
- Sua instrução está fraca. Reforce: **“use somente fontes carregadas”**.
- Suas fontes são vagas. Troque por docs oficiais/PDFs.
- Peça explicitamente: **“cite de qual fonte veio cada afirmação”** (quando aplicável).

### 6.2 “O roteiro ficou robótico”
- Adicione mais exemplos do seu estilo (mais vídeos/transcrições).
- Coloque nas instruções: “evite clichês e frases de IA”.
- Peça: “escreva para ser falado, com pausas e frases curtas”.

### 6.3 “O prompt não funciona no modelo”
- Você provavelmente usou parâmetros que **não existem** no modelo.
- Garanta que a documentação do modelo certo está no notebook.
- Exija: “use somente sintaxe da doc”.

---

## 7) Próximo passo (execução diária em 10 minutos)

**Rotina diária (10 min)**
1) Research Engine: “o que mudou no meu nicho?” (1–2 min)  
2) Script Engine: “roteiro 60s com hook + CTA” (3–4 min)  
3) Prompt Engineer: “thumb + b-roll” (3–4 min)  
4) Gravar/gerar e postar

---

## 8) CTA (para usar nos seus roteiros)
> “Se você quer montar essa máquina completa passo a passo, tá tudo no **inema.club**. Você quer?”

---

### Nota
Este documento descreve um **método**. As ferramentas específicas podem variar.  
O que não muda: **fontes confiáveis → estilo treinado → prompts com sintaxe oficial**.
