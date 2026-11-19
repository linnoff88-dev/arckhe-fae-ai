# BUILD SPEC — fae-ai (uso interno dos construtores)

Curso: **Formação em Automação Estratégica com IA** · Emoji do curso: ⚙️ · Nome curto no logo: "Automação com IA"

Leia também: `/home/nmaldaner/.claude/skills/formato-curso/references/MASTER_COMPLETO.md`,
`/home/nmaldaner/.claude/skills/formato-curso/references/SVG-FUTURISTA.md`,
`/home/nmaldaner/.claude/skills/formato-curso/references/CHECKLIST_REVISAO.md`.

## Trilhas (cor / pasta / nome / emoji)
- T1 Emerald · `curso/trilha1/` · Fundamentos · 🧭
- T2 Blue · `curso/trilha2/` · Auditoria & Mapeamento · 🔍
- T3 Purple · `curso/trilha3/` · Desenho de Soluções · 📐
- T4 Amber · `curso/trilha4/` · Construção · 🛠️
- T5 Teal · `curso/trilha5/` · Comercialização · 💰
- T6 Rose · `curso/trilha6/` · Prática · 🧪

## NAV CANÔNICO para páginas dentro de `curso/trilhaX/` (index da trilha E módulos — mesma profundidade)

Copie verbatim; em cada página marque a trilha ATIVA trocando suas classes para `text-COR-400 bg-COR-500/10` e removendo `hover:` dela; as demais ficam `text-neutral-400 hover:text-COR-400 hover:bg-COR-500/10 transition-colors`.

```html
<nav class="sticky top-0 z-50 bg-dark-900/95 backdrop-blur-sm border-b border-dark-600">
  <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="flex justify-between items-center h-14">
      <div class="flex items-center space-x-4">
        <a href="../../index.html" class="flex items-center space-x-2 text-yellow-400 hover:text-yellow-300">
          <span class="text-2xl">⚙️</span>
          <span class="font-bold text-lg hidden sm:inline">Automação com IA</span>
        </a>
        <span class="text-neutral-600">|</span>
        <a href="https://inema.club" target="_blank" class="text-sky-400 hover:text-sky-300 text-sm font-medium">INEMA.CLUB</a>
      </div>
      <div class="flex items-center space-x-1 sm:space-x-2">
        <a href="../trilha1/index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-neutral-400 hover:text-emerald-400 hover:bg-emerald-500/10 transition-colors"><span class="sm:hidden">T1</span><span class="hidden sm:inline">Fundamentos</span></a>
        <a href="../trilha2/index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-neutral-400 hover:text-blue-400 hover:bg-blue-500/10 transition-colors"><span class="sm:hidden">T2</span><span class="hidden sm:inline">Auditoria</span></a>
        <a href="../trilha3/index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-neutral-400 hover:text-purple-400 hover:bg-purple-500/10 transition-colors"><span class="sm:hidden">T3</span><span class="hidden sm:inline">Desenho</span></a>
        <a href="../trilha4/index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-neutral-400 hover:text-amber-400 hover:bg-amber-500/10 transition-colors"><span class="sm:hidden">T4</span><span class="hidden sm:inline">Construção</span></a>
        <a href="../trilha5/index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-neutral-400 hover:text-teal-400 hover:bg-teal-500/10 transition-colors"><span class="sm:hidden">T5</span><span class="hidden sm:inline">Comercial</span></a>
        <a href="../trilha6/index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-neutral-400 hover:text-rose-400 hover:bg-rose-500/10 transition-colors"><span class="sm:hidden">T6</span><span class="hidden sm:inline">Prática</span></a>
        <button id="theme-toggle" class="p-2 rounded-lg bg-dark-700 hover:bg-dark-600 transition-colors ml-2">
          <svg id="theme-toggle-dark-icon" class="hidden w-5 h-5 text-neutral-300" fill="currentColor" viewBox="0 0 20 20"><path d="M17.293 13.293A8 8 0 016.707 2.707a8.001 8.001 0 1010.586 10.586z"></path></svg>
          <svg id="theme-toggle-light-icon" class="hidden w-5 h-5 text-neutral-300" fill="currentColor" viewBox="0 0 20 20"><path d="M10 2a1 1 0 011 1v1a1 1 0 11-2 0V3a1 1 0 011-1zm4 8a4 4 0 11-8 0 4 4 0 018 0zm-.464 4.95l.707.707a1 1 0 001.414-1.414l-.707-.707a1 1 0 00-1.414 1.414zm2.12-10.607a1 1 0 010 1.414l-.706.707a1 1 0 11-1.414-1.414l.707-.707a1 1 0 011.414 0zM17 11a1 1 0 100-2h-1a1 1 0 100 2h1zm-7 4a1 1 0 011 1v1a1 1 0 11-2 0v-1a1 1 0 011-1zM5.05 6.464A1 1 0 106.465 5.05l-.708-.707a1 1 0 00-1.414 1.414l.707.707zm1.414 8.486l-.707.707a1 1 0 01-1.414-1.414l.707-.707a1 1 0 011.414 1.414zM4 11a1 1 0 100-2H3a1 1 0 000 2h1z" fill-rule="evenodd" clip-rule="evenodd"></path></svg>
        </button>
      </div>
    </div>
  </div>
</nav>
```

A trilha ativa: substituir o `<a>` da própria trilha por (exemplo T1):
`<a href="index.html" class="px-3 py-1.5 rounded-lg text-sm font-semibold text-emerald-400 bg-emerald-500/10">...`
(usa `index.html` porque já está na pasta da trilha).

## Light mode — bloco de acento por trilha (cole no `<style>`, além da Parte 1/3/4 base + Parte 5 bordas)

T1 Emerald → cor `#059669`, rgb `5,150,105`
T2 Blue → `#2563eb`, `37,99,235`
T3 Purple → `#7c3aed`, `124,58,237`
T4 Amber → `#92400e`, `217,119,6`
T5 Teal → `#0d9488`, `13,148,136`
T6 Rose → `#9f1239`, `225,29,72`

```css
html:not(.dark) .text-COR-400 { color: VALOR; }
html:not(.dark) .bg-COR-500\/20 { background-color: rgba(R,G,B,0.12); }
html:not(.dark) .bg-COR-500\/10 { background-color: rgba(R,G,B,0.08); }
html:not(.dark) .border-COR-500\/30 { border-color: rgba(R,G,B,0.25); }
html:not(.dark) .hover\:bg-COR-500\/30:hover { background-color: rgba(R,G,B,0.18); }
```
Sempre incluir também a Parte 5 (bordas dark): `.dark .border-dark-600{border-color:#374151}` e `.dark .divide-dark-600 > :not([hidden]) ~ :not([hidden]){border-color:#374151}`.

## Scripts (todas as páginas): toggleTopic + theme toggle + (index da trilha) openModal/closeModal com iframe. Ver MASTER Sec. 9.

## Regras não-negociáveis (resumo)
- Botões `justify-start`; números em círculo (não setas); 3 seções por tópico (O que é / Por que aprender / Conceitos-chave); ≥6 tópicos por módulo no index.
- Index da trilha: header com stats(4) + hero SVG; **Mapa da trilha** (h2 exato) com cards-âncora `#modulo-X-Y`; `<h2>Conteúdo detalhado</h2>`; cada card de módulo com `id`, tópicos expansíveis e botões "Ver em Modal" + "Ver Completo".
- Módulo: 500-800 linhas, 6-8 `<section id="topico-N">`, variedade de componentes (≥2 grids ✓/✗, ≥1 timeline, ≥2 tip boxes, ≥1 code box), ≥1 SVG futurista inline, Resumo do Módulo com próximo + CTAs.
- INEMA.CLUB (`text-sky-400`) em todas as páginas. Theme toggle funcional.
