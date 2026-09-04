# VALE DESIGN SYSTEM

## Enterprise Digital Products
### Design System para aplicações corporativas, SharePoint, SPFx, React e Power Platform

**Versão:** 2.0

---

# 1. PROPÓSITO

Este documento define o padrão visual e de experiência para aplicações corporativas desenvolvidas neste projeto.

O objetivo é produzir interfaces:

- corporativas;
- modernas;
- premium;
- funcionais;
- consistentes;
- acessíveis;
- responsivas;
- fáceis de manter.

---

# 2. FONTE DE VERDADE

Este arquivo é a fonte de verdade para decisões de:

- UI;
- UX;
- cores;
- tokens;
- tipografia;
- espaçamento;
- componentes;
- densidade;
- responsividade;
- acessibilidade;
- hierarquia visual.

Quando houver conflito entre uma implementação visual e este documento, este documento prevalece.

Requisitos funcionais, segurança e limitações técnicas sempre têm prioridade.

---

# 3. PRINCÍPIO CENTRAL

> **VALE + Enterprise + Moderno + Funcional + Consistente + Acessível**

A identidade deve ser reconhecível sem transformar a interface em uma composição excessivamente verde ou amarela.

A sensação desejada é:

**corporativa, sofisticada, limpa, objetiva e confiável.**

---

# 4. PERSONALIDADE VISUAL

A interface deve transmitir:

- confiança;
- organização;
- eficiência;
- tecnologia;
- clareza;
- maturidade;
- simplicidade.

Evitar aparência:

- genérica;
- infantil;
- excessivamente colorida;
- experimental;
- "template pronto";
- dashboard cheio de cards;
- aplicativo de startup genérico.

---

# 5. REFERÊNCIAS

Use como referências conceituais:

- Microsoft Fluent UI;
- Microsoft 365;
- Power BI;
- Azure;
- aplicações corporativas modernas;
- princípios de design enterprise.

Não copie interfaces.

Use os princípios para construir uma identidade própria baseada neste sistema.

---

# 6. PALETA OFICIAL DO PROJETO

**Estas cores são a fonte de verdade da identidade visual deste projeto.**

## Primárias

| Token | Hex |
|---|---|
| Verde Vale | `#007E7A` |
| Amarelo Vale | `#EDB111` |
| Cinza Escuro | `#555555` |
| Branco | `#FFFFFF` |
| Verde Aqua | `#0ABB98` |
| Azul Vale | `#3CB5E5` |
| Cereja Vale | `#C0305E` |
| Laranja Vale | `#EE6F16` |

## Secundárias

| Token | Hex |
|---|---|
| Verde Escuro | `#034944` |
| Amarelo Claro | `#FFDD99` |
| Aqua Claro | `#9DE4D6` |
| Cereja Escuro | `#991310` |
| Azul Escuro | `#2626D1` |
| Cereja Claro | `#E191C5` |
| Cinza Claro | `#E6E7E8` |
| Cinza Médio | `#BCBEC0` |

## Status

| Token | Hex |
|---|---|
| Positivo | `#00B050` |
| Negativo | `#BB133E` |

**Nunca substitua essas cores por aproximações arbitrárias.**

---

# 7. REGRA DE HIERARQUIA DAS CORES

A regra principal é:

> **Neutros dominam. Verde identifica. Amarelo acentua. Cores secundárias diferenciam. Status comunicam.**

Não utilize todas as cores simultaneamente sem necessidade.

Evite:

- excesso de verde;
- excesso de amarelo;
- rainbow dashboards;
- fundos extremamente coloridos;
- gradientes decorativos.

---

# 8. DESIGN TOKENS

Centralize os valores visuais.

Exemplo:

```css
:root {
  --vale-verde: #007E7A;
  --vale-amarelo: #EDB111;
  --vale-cinza-escuro: #555555;
  --vale-branco: #FFFFFF;
  --vale-verde-aqua: #0ABB98;
  --vale-azul: #3CB5E5;
  --vale-cereja: #C0305E;
  --vale-laranja: #EE6F16;

  --vale-verde-escuro: #034944;
  --vale-amarelo-claro: #FFDD99;
  --vale-aqua-claro: #9DE4D6;
  --vale-cereja-escuro: #991310;
  --vale-azul-escuro: #2626D1;
  --vale-cereja-claro: #E191C5;
  --vale-cinza-claro: #E6E7E8;
  --vale-cinza-medio: #BCBEC0;

  --vale-status-positivo: #00B050;
  --vale-status-negativo: #BB133E;
}
```

---

# 9. TOKENS SEMÂNTICOS

Componentes devem preferencialmente consumir tokens semânticos.

```css
:root {
  --color-primary: var(--vale-verde);
  --color-primary-hover: var(--vale-verde-escuro);
  --color-primary-active: var(--vale-verde-escuro);
  --color-accent: var(--vale-amarelo);

  --color-background: var(--vale-cinza-claro);
  --color-surface: var(--vale-branco);
  --color-surface-secondary: #F8F9F9;
  --color-surface-hover: #F2F4F4;

  --color-text-primary: var(--vale-cinza-escuro);
  --color-text-secondary: #747474;
  --color-text-disabled: var(--vale-cinza-medio);

  --color-border: var(--vale-cinza-medio);
  --color-border-subtle: var(--vale-cinza-claro);

  --color-success: var(--vale-status-positivo);
  --color-error: var(--vale-status-negativo);
  --color-warning: var(--vale-laranja);
  --color-info: var(--vale-azul);
}
```

Os valores neutros adicionais acima são **tokens de interface derivados**, não novas cores de marca.

---

# 10. SUPERFÍCIES

Prioridade:

1. fundo neutro;
2. superfície branca;
3. superfície secundária;
4. elementos de destaque.

A interface deve ter profundidade principalmente por:

- contraste;
- espaçamento;
- bordas;
- hierarquia;
- posicionamento.

Não dependa de sombras pesadas.

---

# 11. TIPOGRAFIA

Priorize uma tipografia corporativa limpa e altamente legível.

Quando o ambiente permitir, utilize a tipografia definida pela plataforma/corporate standard.

Hierarquia clara entre:

- título;
- subtítulo;
- seção;
- label;
- conteúdo;
- informação auxiliar.

Evite excesso de pesos e tamanhos.

---

# 12. ESCALA TIPOGRÁFICA

Como referência:

- Display: 32–40px
- H1: 28–32px
- H2: 24–28px
- H3: 20–24px
- H4: 18–20px
- Body: 14–16px
- Small: 12–13px
- Caption: 11–12px

A escala deve ser ajustada ao contexto.

---

# 13. PESOS TIPOGRÁFICOS

Use principalmente:

- Regular;
- Medium;
- Semibold;
- Bold apenas para destaque real.

Evite interfaces onde tudo parece em negrito.

---

# 14. ESPAÇAMENTO

Use uma escala consistente baseada em múltiplos de 4px.

Referência:

- 4px;
- 8px;
- 12px;
- 16px;
- 20px;
- 24px;
- 32px;
- 40px;
- 48px;
- 64px.

Espaçamento deve criar hierarquia.

---

# 15. BORDER RADIUS

Use cantos modernos, mas discretos.

Referência:

- controles: 4–8px;
- cards: 8–12px;
- modais: 8–12px;
- elementos maiores: até 16px quando fizer sentido.

Evite exagero em elementos totalmente arredondados.

---

# 16. SOMBRAS

Sombras devem ser sutis.

Priorize:

- bordas;
- contraste;
- superfícies;
- espaçamento.

Evite:

- sombras pesadas;
- efeitos 3D;
- glow;
- neon.

---

# 17. LAYOUT

Priorize:

- alinhamento;
- grids consistentes;
- espaçamento previsível;
- leitura em blocos;
- áreas de respiro;
- conteúdo principal claramente identificado.

Evite centralizar tudo sem motivo.

---

# 18. CONTAINERS

Use containers para controlar:

- largura;
- alinhamento;
- densidade;
- leitura.

Evite conteúdo espalhado aleatoriamente pela tela.

---

# 19. CARDS

Cards devem existir quando ajudam a organizar informação.

Características:

- superfície clara;
- borda sutil;
- radius consistente;
- espaçamento adequado;
- hierarquia interna clara.

Evite transformar toda informação da aplicação em card.

---

# 20. BOTÕES

### Primary
Use Verde Vale para a ação principal.

### Secondary
Use tratamento neutro.

### Tertiary / Ghost
Use para ações de menor prioridade.

### Destructive
Use status negativo.

Regra:

> Quanto mais importante a ação, maior deve ser sua evidência visual.

Não use múltiplos botões primários competindo na mesma área.

---

# 21. INPUTS

Inputs devem ter:

- label clara;
- estado normal;
- hover;
- focus;
- disabled;
- erro;
- ajuda quando necessário.

O estado de foco deve ser claramente perceptível.

---

# 22. TABELAS

Tabelas são componentes de alta prioridade em aplicações corporativas.

Priorize:

- leitura;
- alinhamento;
- densidade;
- cabeçalho claro;
- ordenação;
- filtros;
- seleção;
- estados;
- ações;
- paginação.

Evite linhas visualmente pesadas.

Use contraste e espaçamento para separar informações.

---

# 23. DASHBOARDS

Dashboard não deve ser uma coleção de cards coloridos.

Prioridade:

1. informação;
2. contexto;
3. comparação;
4. tendência;
5. ação.

Use cores para significado, não decoração.

---

# 24. KPIs

Um KPI deve possuir:

- label;
- valor principal;
- contexto;
- comparação ou tendência quando aplicável.

Evite colocar dez métricas competindo pela atenção.

---

# 25. STATUS E BADGES

Status devem possuir:

- cor;
- texto/ícone;
- significado explícito.

Nunca dependa exclusivamente de cor para comunicar informação.

---

# 26. ÍCONES

Ícones devem:

- ter função clara;
- manter estilo consistente;
- possuir tamanho coerente;
- não substituir texto quando o significado não for óbvio.

Evite excesso de ícones decorativos.

---

# 27. HEADER

O header deve:

- identificar o produto;
- facilitar navegação;
- manter hierarquia;
- não consumir espaço excessivo.

Priorize simplicidade.

---

# 28. NAVEGAÇÃO

A navegação deve deixar claro:

- onde estou;
- onde posso ir;
- qual é a seção atual;
- quais ações são principais.

Evite menus excessivamente profundos.

---

# 29. FILTROS

Filtros devem ser fáceis de:

- entender;
- aplicar;
- limpar;
- revisar.

Quando houver muitos filtros, organize-os progressivamente.

---

# 30. BUSCA

Busca deve apresentar:

- campo claramente identificável;
- feedback;
- estado vazio;
- loading quando necessário;
- resultados compreensíveis.

---

# 31. MODAIS

Use modal somente quando a ação exigir foco.

Evite transformar fluxos inteiros em modais dentro de modais.

Todo modal deve possuir:

- título;
- contexto;
- ação principal;
- ação secundária;
- fechamento claro.

---

# 32. FEEDBACK

Toda ação relevante deve fornecer feedback apropriado:

- sucesso;
- erro;
- aviso;
- carregamento;
- vazio.

Feedback deve ser claro e proporcional à importância da ação.

---

# 33. MICROINTERAÇÕES

Use animações discretas para:

- transições;
- loading;
- hover;
- confirmação;
- mudança de estado.

Evite animação apenas para "deixar bonito".

A animação deve comunicar.

---

# 34. RESPONSIVIDADE

A interface deve funcionar em:

- desktop;
- notebook;
- tablet;
- telas menores.

Componentes devem lidar corretamente com:

- overflow;
- tabelas;
- filtros;
- modais;
- navegação;
- conteúdo variável.

---

# 35. ACESSIBILIDADE

Acessibilidade é requisito estrutural.

Verifique:

- contraste;
- teclado;
- foco;
- labels;
- leitores de tela;
- aria;
- áreas clicáveis;
- mensagens;
- informação independente de cor.

---

# 36. SHAREPOINT / SPFX

Para SPFx:

- prefira CSS Modules/scoped styles;
- evite seletores globais;
- evite interferir no SharePoint;
- respeite Fluent UI quando utilizado;
- mantenha componentes isolados;
- evite hacks de DOM;
- considere diferentes contextos de Web Part.

Nunca utilize estilos globais como:

```css
button {}
input {}
table {}
div {}
```

sem uma justificativa excepcional.

---

# 37. REUTILIZAÇÃO

Se um padrão aparecer várias vezes, avalie transformá-lo em componente.

Exemplos:

- PageHeader;
- FilterBar;
- DataTable;
- EmptyState;
- LoadingState;
- StatusBadge;
- KpiCard;
- Modal;
- ConfirmationDialog;
- SearchBox.

Não crie abstrações apenas por antecipação.

---

# 38. DENSIDADE

Aplicações corporativas normalmente precisam apresentar bastante informação.

Busque:

> **alta densidade informacional + excelente legibilidade**

Não transforme uma aplicação de trabalho em uma interface excessivamente espaçada.

---

# 39. LESS BUT BETTER

Evite:

- gradientes sem função;
- sombras exageradas;
- animações excessivas;
- excesso de cards;
- excesso de cores;
- bordas desnecessárias;
- elementos decorativos;
- efeitos visuais sem significado.

---

# 40. PRINCÍPIO DE CONSISTÊNCIA

Se dois componentes executam funções semelhantes, eles devem parecer semelhantes.

Consistência deve existir em:

- cores;
- espaçamento;
- radius;
- tipografia;
- estados;
- ícones;
- comportamento.

---

# 41. PROJETOS NOVOS

Em projetos novos:

1. leia este documento;
2. estabeleça os tokens;
3. estabeleça componentes base;
4. estabeleça layout;
5. implemente funcionalidades;
6. revise visualmente;
7. valide acessibilidade;
8. valide responsividade.

---

# 42. PROJETOS EXISTENTES

Não faça redesign destrutivo.

Primeiro:

1. preserve funcionamento;
2. identifique padrões existentes;
3. introduza tokens;
4. normalize componentes;
5. corrija inconsistências;
6. melhore hierarquia;
7. refine visualmente.

---

# 43. ESTRATÉGIA DE MIGRAÇÃO

Quando aplicável:

```text
Tokens
  ↓
Base visual
  ↓
Componentes fundamentais
  ↓
Estrutura
  ↓
Componentes de dados
  ↓
Componentes avançados
  ↓
Refinamento
```

Faça migração progressiva.

---

# 44. MIGRAÇÃO VISUAL

Ao modernizar uma interface existente, não altere tudo simultaneamente.

Priorize:

1. tipografia;
2. espaçamento;
3. cores;
4. superfícies;
5. componentes;
6. layout;
7. estados;
8. responsividade;
9. microinterações.

---

# 45. AUDITORIA VISUAL

Antes de considerar uma interface pronta, pergunte:

- A hierarquia está clara?
- Sei imediatamente o que é importante?
- Os elementos estão alinhados?
- Há excesso de informação visual?
- As cores têm função?
- Os espaços são consistentes?
- A interface parece corporativa e premium?
- Parece um produto projetado ou um CRUD genérico?
- Funciona em telas menores?
- É acessível?
- Há algo visualmente desnecessário?

---

# 46. REFINAMENTO PREMIUM

Depois que estiver funcional, procure oportunidades de melhoria em:

- alinhamento;
- ritmo visual;
- espaçamento;
- tipografia;
- densidade;
- estados;
- feedback;
- consistência;
- detalhes de interação.

O objetivo não é adicionar efeitos.

O objetivo é remover imperfeições.

---

# 47. REGRA DE OURO

> **A interface deve parecer simples porque foi bem projetada, não porque foi simplificada demais.**

---

# 48. PRIORIDADE

Quando houver conflito:

1. segurança;
2. funcionalidade;
3. acessibilidade;
4. performance;
5. usabilidade;
6. consistência;
7. estética.

Estética nunca deve quebrar os itens acima.

---

# 49. RESULTADO ESPERADO

Uma aplicação que:

- pareça profissional;
- pareça moderna;
- seja reconhecível como produto corporativo;
- tenha identidade Vale;
- seja confortável para uso diário;
- seja consistente;
- seja acessível;
- seja tecnicamente sustentável.

---

# 50. REGRA FINAL

> **Não faça apenas uma interface bonita. Faça uma interface que pareça ter sido projetada por uma equipe profissional de produto, design e engenharia.**
