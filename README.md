# Site Pedagógico — Serra Catarinense

Reconstrução em **HTML e CSS** do site pedagógico da Serra Catarinense, feita pela turma de
**Técnico em Desenvolvimento de Sistemas** — SENAI Lages · T DESI 2026/1.

🔗 **Site publicado:** https://lemosmoroni.github.io/site-pedagogico-serra/

Cada grupo é responsável por **uma página** e trabalha na **sua própria branch**.
Ao final, todas as branches são validadas e unidas na `main` pelo professor.

---

## 📋 Materiais da atividade

| Material | Link |
|---|---|
| 📘 **Guia do Aluno** (passo a passo completo) | [https://drive.google.com/file/d/1fj6kp8r1Ja2oi5KQ65RvJkyI5GOf9yet/view?usp=sharing] |
| 🎨 **Guia de Cores** (paleta, fontes e logos) | [https://drive.google.com/file/d/1IVfBrBmgnKZSkpMi6XgoThBdbB8z0Rqm/view?usp=sharing] |
| 🌍 **Site Modelo**  | [https://www.figma.com/make/7WMJcV3R83Y9kJAaL9B2hs/Warframe---SITE-SENAI?code-node-id=0-6&p=f&t=noRBZgn16Bi5hDfY-0&fullscreen=1] |

---

## 👥 Grupos e páginas

| Grupo | Página | Arquivo a criar | Branch |
|---|---|---|---|
| — | Início (Home) | `index.html` | `main` *(professor)* |
| **G1** | Equipe e Unidades | `g1-equipe.html` | `grupo-1` |
| **G2** | Cursos de Aprendizagem Industrial | `g2-aprendizagem-industrial.html` | `grupo-2` |
| **G3** | Cursos Técnicos | `g3-cursos-tecnicos.html` | `grupo-3` |
| **G4** | Materiais de Apoio | `g4-materiais-apoio.html` | `grupo-4` |
| **G5** | Cursos Profissionais | `g5-cursos-profissionais.html` | `grupo-5` |
| **G6** | Treinamentos | `g6-treinamentos.html` | `grupo-6` |
| **G7** | PPPs e Regulamento Escolar | `g7-ppps-regulamento.html` | `grupo-7` |

> ⚠️ **O nome do arquivo não é detalhe.** O menu de todas as páginas já aponta para esses
> nomes. Se usar outro, o link do seu grupo não vai funcionar no site final.

---

## 🚀 Início rápido

```bash
# 1. Baixar o projeto (uma vez)
git clone https://github.com/LemosMoroni/site-pedagogico-serra.git
cd site-pedagogico-serra

# 2. Entrar na branch do seu grupo
git checkout grupo-3          # troque pelo número do seu grupo
git branch                    # confira: o * deve estar na sua branch

# 3. Criar a sua página a partir do modelo
cp modelo-pagina.html g3-cursos-tecnicos.html

# 4. O ciclo do dia a dia (repita várias vezes por aula)
git add .
git commit -m "Grupo 3: descreva o que fez"
git push
```

Passo a passo completo e ilustrado no **Guia do Aluno** (link na tabela acima).

---

## 📁 Estrutura do repositório

```
/
├── index.html            Home do site (mantida pelo professor)
├── modelo-pagina.html    Modelo com cabeçalho e rodapé prontos — copie este
├── estilo-comum.css      Design system compartilhado — NÃO EDITAR
├── menu.js               Comportamento do menu — NÃO EDITAR
├── favicon.ico
├── assets/               Logos e ícones — NÃO EDITAR
├── img/                  Imagens das páginas (cada grupo coloca as suas)
└── docs/
    ├── ESPECIFICACAO-VISUAL.md   Cores, fontes e componentes para copiar
    └── GUIA-GIT-ALUNO.md         Passo a passo de Git/GitHub
```

---

## ⚖️ Regras de ouro

1. **Mexa apenas no seu arquivo** `gN-....html` e nas suas imagens em `img/`.
2. **Não edite** `estilo-comum.css`, `menu.js`, `assets/`, o cabeçalho ou o rodapé.
3. **Sempre na sua branch.** Nunca faça commit direto na `main` (ela é protegida).
4. **Toda imagem precisa de `alt`**; **todo link precisa dizer para onde vai**
   (nada de "Acesse Aqui!").
5. **Só o que está no GitHub existe.** Dê `git push` ao final de toda aula.

---

## ✅ Como entregar

1. Passe pelo **checklist** do Guia do Aluno.
2. Faça o `git push` final e confira no GitHub que subiu.
3. Avise o professor.
4. O professor valida pela rubrica e faz o **merge** na `main`.
5. Em poucos minutos, sua página entra no ar — e o link do seu grupo, que antes dava 404
   na Home, passa a funcionar. 🎉

---

## 🎨 Identidade visual

| | |
|---|---|
| **Azul principal** `#003087` | cabeçalho e títulos |
| **Laranja** `#F47920` | botões e destaques |
| **Fontes** | Barlow Condensed (títulos) e Barlow (textos) |

Detalhes completos no **Guia de Cores**.

---

## 👨‍🏫 Grupos

| Grupo | Integrantes |
|---|---|
| 1 | |
| 2 | |
| 3 | |
| 4 | |
| 5 | |
| 6 | |
| 7 | |

---

<sub>SENAI Lages · Educação Profissional — Serra Catarinense</sub>
