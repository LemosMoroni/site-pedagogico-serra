# Especificação Visual — o "contrato" do site

Este é o padrão que **todas as páginas seguem** para o site encaixar no final.
Tudo aqui já está pronto no `estilo-comum.css`. Você **não escreve CSS de cor ou
fonte** — apenas usa as classes descritas abaixo.

---

## 1. Cores (já definidas como variáveis CSS)

| Uso | Variável | Hex |
|---|---|---|
| Azul principal | `--blue` | `#003087` |
| Azul escuro (rodapé, menu) | `--blue-dark` | `#002166` |
| Azul médio | `--blue-mid` | `#004BB5` |
| Azul claro (fundos) | `--blue-light` | `#E8EEF8` |
| Laranja (destaque, botões) | `--orange` | `#F47920` |
| Laranja escuro (hover) | `--orange-dark` | `#D4620A` |
| Texto | `--charcoal` | `#1C1C1E` |
| Texto secundário | `--gray-60` | `#636366` |

Para usar uma cor no seu CSS: `color: var(--blue);`

## 2. Tipografia

- Títulos: **Barlow Condensed** (`--disp`), em CAIXA ALTA.
- Texto: **Barlow** (`--body`).

As fontes já são carregadas no `<head>` do modelo. Não troque por outras.

## 3. Logos e favicon

| Arquivo | Onde é usado |
|---|---|
| `assets/Logo-SENAI_EP.png` | Cabeçalho (logo horizontal) |
| `assets/Logo-S.png` | Rodapé (logo compacto "S") |
| `favicon.ico` + `assets/favicon-32.png` | Ícone da aba do navegador |

Já estão posicionados no cabeçalho e rodapé do modelo. **Não altere.**

---

## 4. Cabeçalho e rodapé

Estão prontos no `modelo-pagina.html` e são **idênticos em todas as páginas**.
A única mudança permitida no cabeçalho é marcar a sua aba com `class="active"`.

---

## 5. Componentes prontos (copie o que a sua página precisa)

### 5.1 Título da página
```html
<div class="crumb">Início › Nome da seção</div>
<h1 class="page-title">Nome da seção</h1>
<p class="page-lead">Uma frase curta sobre a página.</p>
```

### 5.2 Subtítulo de seção
```html
<div class="section-h">Título da seção</div>
```

### 5.3 Grade de cards (para páginas de CURSOS)
```html
<div class="grid cols-3">
  <div class="course-card">
    <img src="img/nome-da-foto.jpg" alt="Descreva a imagem aqui">
    <div class="cc-body">
      <h3>Nome do Curso</h3>
      <a class="btn" href="URL-DO-PLANO">Ver plano do curso</a>
    </div>
  </div>
  <!-- repita .course-card para cada curso -->
</div>
```

### 5.4 Lista de links (para MATERIAIS, TÉCNICOS, PROFISSIONAIS, TREINAMENTOS)
```html
<div class="link-block">
  <h3>Nome da categoria</h3>
  <ul class="link-list">
    <li><a href="URL">Texto que diz para onde o link leva</a></li>
    <li><a href="URL">Outro link descritivo</a></li>
  </ul>
</div>
```

### 5.5 Cartões de unidade (para EQUIPE E UNIDADES)
```html
<div class="unit-grid">
  <div class="unit-card">
    <img src="img/unidade-lages.jpg" alt="Fachada da unidade de Lages">
    <div class="u-body">
      <h3>Lages</h3>
      <p>Descrição curta da unidade.</p>
    </div>
  </div>
</div>
```

### 5.6 Chips (etiquetas, ex.: lista de municípios)
```html
<div class="chips">
  <span class="chip">Lages</span>
  <span class="chip">Otacílio Costa</span>
</div>
```

---

## 6. Duas regras de acessibilidade (valem nota)

1. **Toda imagem** tem `alt` que descreve a imagem. Foto decorativa: `alt=""`.
2. **Todo link** tem texto que diz o destino. Troque "Acesse Aqui!" e
   "Link de acesso:" por algo como "Ver plano do curso de Mecânico Industrial".

> O site original repete "Acesse Aqui!" em quase todos os botões — corrigir isso
> é um dos objetivos da atividade.
