# Respostas do LAB 01

Nome:Ricardo Ongari Rodrigues
Dupla (M2 em diante):Isabella Macedo Kawecki

---

## M2 - Quem quebrou o painel

**Hash curto do commit que introduziu o erro:** 01ef93b

**Autor:** Tarcisio Melo

**Data:** 2026-06-15

**Linha alterada (antes e depois):**

```
antes: return (leitura - 32) * 5 / 9;
depois: return leitura * 9 / 5 + 32
```

---

## M3 - O segredo vazado

**O que voce esperava ver no `git status` e o que apareceu:** Eu espera ver o status ignorando o credenciais.env. 

apareceu:
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    config/credenciais.env

nothing added to commit but untracked files present (use "git add" to track)



**Depois do push, alguem que clonar o repositorio ainda consegue ler a chave?
Responda em duas linhas, explicando o motivo:**

Antes não tinha dado certo pois o arquivo ja tinha sido publicado, e o gitignore não deleta ele.
Agora com o comando  "git rm --cached config/credenciais.env" ele para de rastrear o arquivo.

---

## M4 - Colisao

**O que significavam os marcadores que apareceram dentro do arquivo:**

- `<<<<<<<` :
- `=======` :
- `>>>>>>>` :

**Qual pedaco veio de quem, e qual titulo voces decidiram manter:**

---

## Casa - Incidente na linha 3

**Hash do commit que quebrou o painel:**

**Hash do commit de revert:**

**Por que `git revert` e nao `git reset` neste caso:**
