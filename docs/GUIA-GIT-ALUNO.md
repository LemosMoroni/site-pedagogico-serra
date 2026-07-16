# Guia de Git e GitHub — para o aluno

Você nunca usou git? Sem problema. Neste projeto você só precisa de **um ciclo de
três passos**, sempre na branch do seu grupo: **editar → commit → push**.

---

## Antes de começar (uma vez só)

1. Crie uma conta no [github.com](https://github.com) (se ainda não tiver).
2. Instale o Git: [git-scm.com/downloads](https://git-scm.com/downloads).
3. Configure seu nome e e-mail (uma vez, no computador):
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu-email@exemplo.com"
   ```

## Passo 1 — Clonar o repositório (uma vez por grupo)

```bash
git clone <url-do-repositorio>
cd site-pedagogico
```

## Passo 2 — Entrar na branch do seu grupo

O professor já criou as branches (`grupo-1`, `grupo-2`, …). Entre na sua:

```bash
git checkout grupo-N
```

> ⚠️ Confira sempre em qual branch você está antes de trabalhar:
> ```bash
> git branch        # a branch atual aparece com um *
> ```

## Passo 3 — Abrir a sua página

O arquivo do seu grupo **já existe** no repositório (ex.: `g1-equipe.html`). Abra-o
no VS Code e comece a editar o miolo. Coloque as imagens na pasta `img/`.

> O `modelo-pagina.html` fica só como referência — você não precisa copiá-lo.

## Passo 4 — O ciclo do dia a dia (repita sempre)

```bash
git add .                                  # separa o que mudou
git commit -m "Grupo N: descreva o que fez"  # tira uma 'foto' das mudanças
git push                                     # envia para o GitHub
```

Pronto. Repita esse ciclo várias vezes por aula — quanto mais commits pequenos,
melhor.

---

## Aula 0 — aquecimento (antes de mexer no site)

Para passar pelo ciclo uma vez sem pressão:

1. Abra o arquivo `README.md`.
2. Escreva o nome do seu grupo e dos integrantes no final.
3. Faça `git add .` → `git commit -m "Grupo N: integrantes"` → `git push`.

Se apareceu no GitHub, você já sabe o essencial. 🎉

---

## Como o professor junta tudo

Quando a sua página estiver pronta, avise o professor. Ele vai revisar usando a
[Rubrica de Validação](RUBRICA-VALIDACAO.md) e, se estiver ok, unir a sua branch
na `main`. Você **não precisa** fazer merge — só cuidar da sua branch.

---

## Perguntas rápidas

**"Deu erro no push, algo sobre pull."**
Alguém do seu grupo enviou algo antes de você. Rode `git pull` e depois `git push`.

**"Editei o arquivo errado / o cabeçalho."**
Sem pânico. Fale com o professor — dá para desfazer. Regra: mexa só no seu
`gN-....html` e na pasta `img/`.

**"Quero ver como ficou no navegador."**
Abra o seu arquivo `.html` com o VS Code + extensão *Live Server*, ou dê dois
cliques no arquivo. (A busca do topo é só visual por enquanto — não vai buscar de
verdade, e tudo bem.)
