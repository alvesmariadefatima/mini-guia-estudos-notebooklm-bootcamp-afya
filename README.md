# 📚 Mini Guia de Estudos com NotebookLM — Bootcamp Afya Automação de Dados com Python

![NotebookLM](https://img.shields.io/badge/Google-NotebookLM-orange)
![Status](https://img.shields.io/badge/Status-concluido-green)

Os resumos abaixo foram elaborados por mim a partir das fontes estudadas no NotebookLM e representam uma síntese autoral dos conceitos considerados mais relevantes para revisão.

## Transparência sobre o uso de IA

Este material foi desenvolvido com apoio do Google NotebookLM como ferramenta de estudo, organização de conhecimento e síntese de informações. Todas as fontes utilizadas estão listadas neste repositório e os conteúdos foram revisados e adaptados por mim.

## 📖 Sobre o Projeto

Este repositório reúne meu caderno temático produzido no Bootcamp Afya Automação de Dados com Python, utilizando o Google NotebookLM como ferramenta de apoio aos estudos.

Tema do caderno:
Fundamentos da Inteligência Artificial Moderna: Machine Learning, LLMs, IA Generativa e Agentes Inteligentes.

Como usei o NotebookLM:
- Organizei e resumi fontes abertas (texto/PDF)
- Criei glossários e mapas de conceitos
- Testei prompts e documentei “cicatrizes” (o que deu errado e como corrigi)
- Consolidei um miniguia reutilizável para revisões

---

## 🎯 Objetivos de Estudo

- Compreender os fundamentos da Inteligência Artificial Moderna
- Distinguir Machine Learning, Deep Learning e IA Generativa
- Entender como funcionam os Large Language Models (LLMs) e a arquitetura Transformer
- Explorar o conceito de agentes inteligentes e automação baseada em IA
- Desenvolver habilidades práticas de Engenharia de Prompt (critérios, iteração e troubleshooting)
- Criar material de consulta rápida para futuras revisões

Escopo: fundamentos conceituais e práticos; fora do escopo: implementação matemática aprofundada e treinamento de modelos em larga escala.

---

## 📚 Curadoria de Fontes (3–5) — usadas no NotebookLM

As fontes abaixo foram selecionadas, enviadas ao NotebookLM e serviram de base para respostas e resumos.

1) Deep Learning (Cap. 1–6) — Goodfellow, Bengio, Courville  
- Link: https://www.deeplearningbook.org/  
- Tipo: Livro online (texto)  
- Por que escolhi: base sólida em ML/DL com linguagem acessível  

2) Attention Is All You Need — Vaswani et al. (2017)  
- Link: https://arxiv.org/pdf/1706.03762.pdf  
- Tipo: Artigo científico (PDF)  
- Por que escolhi: marco da arquitetura Transformer, essencial para LLMs  

3) The Illustrated Transformer — Jay Alammar  
- Link: http://jalammar.github.io/illustrated-transformer/  
- Tipo: Artigo técnico ilustrado (texto)  
- Por que escolhi: visualizações claras da arquitetura e intuições práticas  

4) IBM — O que é Machine Learning? (pt-BR)  
- Link: https://www.ibm.com/br-pt/think/topics/machine-learning  
- Tipo: Artigo de referência (texto)  
- Por que escolhi: visão introdutória em português, útil para contextualização  

5) NIST AI Risk Management Framework (AI RMF 1.0)  
- Link: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf  
- Tipo: Framework oficial (PDF)  
- Por que escolhi: visão de riscos, governança e boas práticas em IA  

Observação importante: substituí as fontes anteriores que eram sobre investimentos/Benjamin Graham para manter coerência com o tema de IA. Se preferir manter o tema de investimentos, ajuste o “Tema” e os “Objetivos” para esse domínio.

---

## 🧠 Engenharia de Prompts e “Cicatrizes” (troubleshooting)

Abaixo, documento perguntas estratégicas, variações testadas, problemas encontrados e como corrigi. Também incluo critérios de qualidade exigidos antes de rodar cada prompt.

### Caso 1 — Marcos históricos da IA

- Objetivo: obter uma linha do tempo com marcos datados e referências
- Critérios de qualidade: datas verificáveis; citação da fonte; foco nos marcos mais influentes

Prompt v1 (genérico):
Quais são os principais marcos históricos da Inteligência Artificial?

Problema observado:
- Resposta ampla, sem ancoragem em datas precisas nem referências explícitas.

Ajuste — Prompt v2 (específico e com critérios):
Liste 12 marcos históricos da IA em ordem cronológica, com ano, evento e 1–2 linhas de contexto. Cite a fonte entre parênteses após cada marco (ex.: [Goodfellow cap.1], [Vaswani 2017], [IBM ML]). Não inclua marcos sem fonte.

Resultado resumido:
- Linha do tempo clara (dos anos 40 ao presente), incluindo Turing (1950), Dartmouth (1956), Perceptron (1957), invernos da IA, Deep Blue (1997), ressurgimento do DL (2006), Watson (2011), Transformer (2017) e popularização de LLMs.
- Referências apontadas para cada marco.

Aprendizado (cicatriz):
- Sem exigir referência inline, o modelo retorna generalidades. Ao solicitar citação por item, a cobertura e verificabilidade melhoraram.

### Caso 2 — O que é o Teste de Turing?

- Objetivo: descrição precisa do jogo da imitação, formato e critério
- Critérios de qualidade: definição sucinta; dinâmica do teste; limitações

Prompt v1:
O que foi o teste de Turing exatamente?

Problema:
- Texto explicativo correto, porém extenso e sem destacar os elementos operacionais do teste.

Ajuste — Prompt v2 (orientado a saída):
Explique o Teste de Turing em até 120 palavras. Estruture em: Objetivo, Dinâmica (interrogador, humano, máquina; comunicação por texto), Critério (indistinguibilidade pelo juiz). Finalize com “Limitações” (1 linha). Cite 1 fonte entre parênteses.

Resultado resumido:
- Definição objetiva com os 3 blocos pedidos e uma linha de limitações metodológicas.
- Referência à obra original e/ou fonte de apoio.

Aprendizado:
- Limitar palavras + pedir estrutura e fonte eleva a precisão e legibilidade.

### Caso 3 — Principais críticas ao Teste de Turing

- Objetivo: mapear objeções clássicas e modernas, sem depender de anedotas
- Critérios de qualidade: nome da crítica; ideia central; fonte

Prompt v1:
Quais são as principais críticas ao Teste de Turing?

Problema:
- Listas sem atribuição de fonte e com ênfase desbalanceada.

Ajuste — Prompt v2 (matricial e referenciado):
Liste 6 críticas ao Teste de Turing em formato: Nome da crítica — ideia central (máx. 20 palavras) — fonte entre colchetes. Inclua “Quarto Chinês (Searle)”, “Suficiente, não necessária”, “Fisicalidade/senso comum”, “Limitações metodológicas”. Não repita críticas.

Resultado resumido:
- Tabela enxuta cobrindo: Suficiência vs. necessidade; Quarto Chinês; memorização; fisicalidade; limitações metodológicas; criatividade/decidibilidade.
- Cada item com fonte indicada.

Aprendizado:
- Exigir formato fixo e citação por item reduziu redundâncias e melhorou rastreabilidade.

---

## 📘 Mini Guia de Estudos (Entrega Final)

### 1) Resumos Estruturados por Tópico

- Inteligência Artificial (IA)
  - O que é: campo que cria sistemas para executar tarefas que requerem inteligência humana
  - Por que importa: automação, produtividade, descoberta científica, serviços inteligentes
  - Subáreas: ML, DL, PLN, Visão, Planejamento, Robótica, Agentes
  - Riscos: viés, alucinações, privacidade, segurança, uso indevido
  - Boas práticas: dados de qualidade, avaliação contínua, governança

- Machine Learning (ML)
  - Ideia central: aprender padrões a partir de dados
  - Tipos: supervisionado, não supervisionado, por reforço
  - Pipeline: dados → features → modelo → validação → deploy → monitoramento
  - Métricas: accuracy, precisão, recall, F1, AUC; regressão: MAE, RMSE
  - Erros comuns: overfitting, leakage, dados desbalanceados

- Deep Learning (DL)
  - O que é: redes neurais profundas para tarefas complexas
  - Arquiteturas: CNNs (visão), RNN/LSTM (sequências), Transformers (PLN/multimodal)
  - Requisitos: muitos dados, GPU/TPU, regularização, early stopping
  - Riscos: interpretabilidade, custo, viés nos dados

- IA Generativa
  - Capacidade: gerar texto, imagem, áudio, código
  - Técnicas: auto-regressivos (LLMs), VAEs, GANs, Diffusion
  - Uso prático: assistência, prototipação, conteúdo, apoio a decisão
  - Cuidados: checagem de fatos, direitos autorais, políticas de uso

- LLMs e Transformers
  - Conceitos-chave: embeddings, atenção, máscara, positional encoding
  - Fluxo: tokenização → embeddings → camadas Transformer → geração
  - Limitações: alucinações, factualidade, sensibilidade ao prompt
  - Mitigações: boas instruções, contexto ancorado em fontes, verificação humana

- Agentes Inteligentes
  - Definição: sistemas que percebem, planejam e agem para atingir objetivos
  - Componentes: percepção, estado, política, plano, ação, feedback
  - Exemplos: automação de tarefas, RPA com IA, agentes de pesquisa/execução
  - Riscos: loops, ações inseguras, escalonamento sem supervisão
  - Boas práticas: objetivos claros, restrições, “human-in-the-loop”

### 2) Glossário Essencial (20 termos)

- IA — Inteligência Artificial
- ML — Aprendizado de Máquina
- DL — Aprendizado Profundo
- LLM — Large Language Model
- Prompt — Instrução passada ao modelo
- Context Window — Janela de contexto (tokens considerados na resposta)
- Token — Unidade mínima de texto processada pelo modelo
- Embedding — Vetor que representa significado de palavras/frases
- Atenção — Mecanismo que pondera relevância entre tokens
- Positional Encoding — Sinal que codifica posição na sequência
- Fine-tuning — Ajuste do modelo para um domínio específico
- Zero-shot/Few-shot — Uso com 0 ou poucos exemplos no prompt
- Alucinação — Resposta plausível porém falsa/inventada
- Overfitting — Modelo memorizando ruído do treino
- Regularização — Técnicas para reduzir overfitting
- Métricas de Classificação — Precisão, Recall, F1, AUC
- RL — Aprendizado por Reforço
- Risco em IA — Probabilidade x impacto de falhas/viés
- Governança de IA — Políticas e processos para uso responsável
- Human-in-the-loop — Humanos supervisionando/ajustando o sistema

[Opcional] Indique fontes de apoio no glossário, quando útil: (ex.: [Goodfellow cap.1], [NIST AI RMF]).

### 3) Prompts Reutilizáveis

- Revisão Rápida
Você é um(a) especialista em [TEMA] explicando para [PÚBLICO-ALVO], nível [NÍVEL]. Produza um resumo objetivo em até 10 tópicos, cobrindo: definição, por que importa, componentes-chave, fluxo/arquitetura (se houver), exemplos práticos no Brasil, erros comuns, métricas/indicadores, boas práticas e próximos passos. Cite fontes quando possível. Não invente dados.

- **Preparação para Certificação**
Você é um(a) instrutor(a) sênior de [TEMA] com foco na certificação [CERTIFICAÇÃO]. Público: [NÍVEL], experiência [EXPERIÊNCIA PRÉVIA], tempo [TEMPO DISPONÍVEL]. Entregue:
1) Domínios e objetivos (pesos se públicos)
2) 10–15 tópicos essenciais
3) Armadilhas de prova
4) Plano de estudo
5) Recursos oficiais
6) Glossário de 20 termos
7) Checklist pré-prova

- **Criação de Flashcards**
Gere 20 flashcards sobre [TEMA], nível [NÍVEL]. Misture: conceito/definição, cenários práticos, antipadrões. Para cada card: Pergunta, Resposta curta, Dica mnemônica (opcional), Dificuldade (1–5), Tags.

- **Simulado**
Crie 10 questões de múltipla escolha sobre [TEMA], nível [NÍVEL], estilo [ESTILO]. [NÚMERO_DE_OPÇÕES] alternativas, 1 correta. Balanceie dificuldade. Liste subtemas antes. Inclua Gabarito Comentado e Rubrica de Desempenho.

- **Mapa Mental**
Gere um mapa mental hierárquico de [TEMA] com profundidade [PROFUNDIDADE], cobrindo [FOCO]. Estruture com nó raiz, 5–7 pilares, sub-ramos (definições, exemplos BR, métricas, riscos). Entregue versão hierárquica e versão compacta por palavras-chave.

### 4) Como usar este miniguia (roteiro rápido de 7 dias)

- Dia 1: IA e ML (30–40 min) — leia resumos + 10 flashcards
- Dia 2: DL (30–40 min) — CNN/RNN/Transformer; revise 10 flashcards
- Dia 3: LLMs (40–50 min) — arquitetura e limitações; 1 simulado curto
- Dia 4: IA Generativa (30–40 min) — casos práticos + riscos
- Dia 5: Agentes (30–40 min) — percepção→ação; mini projeto mental
- Dia 6: Revisão guiada com “Revisão Rápida” + mapa mental
- Dia 7: Simulado completo + gabarito comentado e ajustes finais
---
