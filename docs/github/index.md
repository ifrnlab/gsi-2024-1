# GitHub

Crie um arquivo com o nome de seu usuário do GitHub e com a extensão ".txt". No conteúdo, insira um Nome Sobrenome.

## Adição de colaboradores

O seguinte script escrito em Bash[^1] foi usado para adicionar os colaboradores.

```bash

for arq in *.txt
do
    gh api -X PUT repos/ifrnlab/gsi-2024-1/collaborators/"${arq%.txt}"
done
```

[^1]: A seguinte página da web foi consultada: <https://gist.github.com/marchampson/4655798>.