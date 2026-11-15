# Fork da Forja — `forja`

Este é um fork de `HakanSeven12/OpenCADStudio` mantido pela plataforma **Forja**
(`dionarley/forja`). A branch `forja` é a mainline do fork: é o que o monorepo
fixa no submodule (`apps/_gpl/opencadstudio`). Mudanças entram aqui, **sem PR na origem**.

## O que muda nesta branch

Nada por enquanto: a branch é o upstream na versão que a Forja usa. Cada mudança
entra aqui com o motivo, em uma linha.

## Atualizar a partir da origem

```sh
git remote add upstream https://github.com/HakanSeven12/OpenCADStudio.git   # uma vez
git fetch upstream
git checkout forja
git rebase upstream/main
git push --force-with-lease origin forja
```

Depois, no monorepo: `git add apps/_gpl/opencadstudio && git commit -m "chore: atualiza OpenCADStudio"`.

## Licença

GPL-3.0. Por isso este fork vive em `apps/_gpl/` no monorepo: pode ser usado
como ferramenta, **não** entra no template (Gabarito) nem em produto
distribuído.

