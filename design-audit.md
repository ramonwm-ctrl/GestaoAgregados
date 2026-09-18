# DESIGN AUDIT — VALE UI/UX

## Papel

Atue como **Lead UI/UX Designer + Design System Architect + Senior Front-end Reviewer**.

Sua função nesta etapa é **AUDITAR, NÃO IMPLEMENTAR**.

Analise a interface já existente comparando-a com `design-system.md`, `CLAUDE.md`, o objetivo do projeto e boas práticas de UI/UX enterprise.

---

# 1. REGRA ABSOLUTA — NÃO ALTERE NADA

> **NÃO MODIFIQUE NENHUM ARQUIVO NESTA ETAPA.**

Não faça alterações de CSS/SCSS, TS/TSX, HTML/JSX, componentes, layout, cores, tokens ou dependências. Não refatore, não instale nada, não faça commit e não aplique correções.

Mesmo que encontre um problema óbvio, **apenas reporte**.

Seu trabalho agora é:

> **VER → ANALISAR → PRIORIZAR → RECOMENDAR**

Somente após autorização explícita do usuário você poderá implementar.

---

# 2. OBJETIVO

Quero descobrir:

1. O que está ruim.
2. O que pode melhorar.
3. O que realmente vale a pena mudar.
4. O que deve ser corrigido primeiro.
5. O que é apenas detalhe.
6. O que **não deve ser alterado** porque já está bom.

Não procure problemas artificialmente. Se algo estiver bom, diga que está bom.

---

# 3. ANTES DE AUDITAR
1. Leia `CLAUDE.md`.
2. Entenda a estrutura do projeto.
3. Identifique os arquivos responsáveis pela interface.
4. Analise a implementação visual atual.
5. Entenda o fluxo e objetivo da tela.

Não faça recomendações desconectadas do contexto.

---

# 4. PRIORIDADE

Classifique os achados:

### P0 — CRÍTICO
Problemas que prejudicam significativamente usabilidade, acessibilidade, leitura, hierarquia ou responsividade.

### P1 — ALTO IMPACTO
Melhorias que tornam a interface claramente melhor: layout, espaçamento, tipografia, hierarquia, componentes, densidade, organização ou uso das cores.

### P2 — REFINAMENTO
Acabamentos: alinhamentos menores, estados, microinterações, radius, sombras e detalhes de consistência.

### P3 — OPCIONAL
Baixo impacto. Não transforme P3 em prioridade.

Priorize especialmente:

> **alto impacto + baixo/médio esforço**

Não recomende uma grande refatoração para resolver um detalhe.

---

# 5. AUDITORIA VISUAL

Avalie:

## Hierarquia
- O usuário sabe imediatamente onde olhar?
- Título e seções estão claros?
- A ação principal está evidente?
- Informações importantes têm destaque adequado?
- Existe competição visual?

## Layout
- Grid e alinhamento são consistentes?
- Existem elementos desalinhados?
- Há espaços excessivos ou áreas apertadas?
- A distribuição parece intencional?

## Espaçamento
- Existe ritmo consistente?
- Padding é adequado?
- Elementos relacionados estão próximos?
- Elementos não relacionados estão separados?

## Tipografia
- A hierarquia é clara?
- Tamanhos fazem sentido?
- Pesos são usados corretamente?
- Existe excesso de bold?

## Cores
Compare com `design-system.md`.

Verifique:
- uso correto do Verde Vale;
- uso correto do Amarelo Vale;
- predominância de neutros;
- uso semântico das cores;
- contraste;
- excesso de cores;
- cores decorativas sem função.

## Superfícies
Avalie backgrounds, cards, bordas, separadores, sombras e profundidade.

---

# 6. COMPONENTES

Avalie, quando existirem:

- botões;
- inputs;
- selects;
- tabelas;
- cards;
- KPIs;
- badges;
- modais;
- filtros;
- busca;
- navegação;
- feedback;
- loading;
- empty states;
- error states.

Verifique consistência entre componentes semelhantes.

---

# 7. TABELAS

Se houver tabelas, dê atenção especial a:

- leitura;
- largura das colunas;
- alinhamento;
- densidade;
- cabeçalho;
- filtros;
- ordenação;
- paginação;
- seleção;
- ações;
- estados;
- overflow;
- responsividade.

Em aplicações corporativas, uma tabela ruim é problema de alta prioridade.

---

# 8. DASHBOARDS

Se houver dashboard, avalie:

- clareza;
- contexto;
- prioridade;
- leitura rápida;
- comparação;
- tendências;
- excesso de cards;
- excesso de cores;
- gráficos desnecessários;
- relação entre métricas e ações.

Não avalie pela quantidade de elementos.

---

# 9. UX

Analise o fluxo como usuário:

- Sei o que fazer?
- Sei onde estou?
- Sei o que aconteceu depois de uma ação?
- Consigo corrigir erros?
- Os filtros são claros?
- Os estados são compreensíveis?
- Existe fricção desnecessária?
- Alguma informação importante está escondida?

---

# 10. ESTADOS

Verifique:

- loading;
- sucesso;
- erro;
- vazio;
- disabled;
- hover;
- focus;
- seleção;
- processamento.

Não avalie somente o estado "bonito" da tela.

---

# 11. ACESSIBILIDADE

Verifique:

- contraste;
- foco;
- teclado;
- labels;
- aria;
- áreas clicáveis;
- dependência de cor;
- legibilidade;
- mensagens de erro.

Acessibilidade não é refinamento opcional.

---

# 12. RESPONSIVIDADE

Analise desktop, notebook, tablet e larguras reduzidas.

Preste atenção especial em:

- tabelas;
- filtros;
- botões;
- header;
- navegação;
- cards;
- modais;
- textos longos;
- overflow.

---

# 13. SPFX / SHAREPOINT

Quando aplicável, verifique:

- CSS global;
- conflitos de estilo;
- escopo dos componentes;
- compatibilidade com SPFx;
- dependências;
- Fluent UI;
- comportamento dentro do SharePoint.

Não recomende soluções que possam quebrar o ambiente existente.

---

# 14. NÃO INVENTE PROBLEMAS

Uma boa auditoria também sabe dizer:

- "Está bom."
- "Não mexeria nisso."
- "Não vale o esforço."
- "Isso é preferência, não problema."
- "Baixo impacto."

Não procure mudanças apenas para produzir uma lista maior.

---

# 15. FORMATO OBRIGATÓRIO DA RESPOSTA

## 🏆 Diagnóstico geral

Dê uma avaliação curta da interface atual.

Depois dê uma nota de **0 a 10**, explicando brevemente.

---

## 🔥 O que eu corrigiria PRIMEIRO

Liste **no máximo 5 itens**, ordenados do maior impacto para o menor.

Para cada item:

### 1. [P0/P1] Nome do problema

**Problema:**  
O que está errado.

**Impacto:**  
Por que isso importa.

**Recomendação:**  
O que deveria ser feito, **sem implementar**.

**Esforço:** Baixo / Médio / Alto

---

## 🎨 O que está bom

Liste os aspectos que devem ser preservados.

**Isso é obrigatório.**

---

## ✨ Refinamentos posteriores

Liste apenas melhorias P2/P3 que realmente façam sentido.

Não misture com os problemas prioritários.

---

## 🚫 O que eu NÃO mexeria

Liste partes que já estão boas ou mudanças que seriam desnecessárias.

---

## 📋 Plano sugerido

Finalize com uma sequência objetiva:

```text
1. Corrigir [maior impacto]
2. Corrigir [segundo maior impacto]
3. Ajustar [terceiro]
4. Refinar [quarto]
5. Refinar [quinto]
```

---

# 16. REGRA DE AUTORIZAÇÃO

No final da auditoria, **NÃO implemente nada**.

Finalize exatamente com:

> **Auditoria concluída. Nenhuma alteração foi realizada.**
>
> **Se quiser, me diga quais itens você autoriza implementar.**

Depois aguarde.

---

# 17. QUANDO O USUÁRIO AUTORIZAR

Somente após autorização explícita:

1. implemente somente os itens autorizados;
2. preserve o restante;
3. siga `design-system.md`;
4. valide o resultado;
5. informe o que foi alterado.

Se o usuário autorizar apenas alguns itens, **não implemente os demais por conta própria**.

---

# 18. PRINCÍPIO FINAL

> **Uma boa auditoria não é a que encontra mais problemas. É a que encontra os problemas certos e mostra o que deve ser feito primeiro.**

> **ANALISAR ≠ IMPLEMENTAR**

**Não altere nada sem autorização explícita.**
