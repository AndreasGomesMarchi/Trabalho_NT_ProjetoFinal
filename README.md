## Como executar

Este projeto utiliza **Git LFS** para armazenar os arquivos CSV e o modelo treinado.

Antes de executar o notebook, instale o Git LFS:

```bash
git lfs install
```

Após clonar o repositório, execute:

```bash
git lfs pull
```

Caso os arquivos apareçam apenas como ponteiros (`version https://git-lfs.github.com/spec/v1`), execute:

```bash
git lfs checkout
```

Depois disso, abra o notebook normalmente.
