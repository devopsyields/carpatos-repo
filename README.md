# CarpatOS package repository

Repo de distributie pentru pachete `.cpm` ale CarpatOS.

Format: `repo.index` + `pool/*.cpm` la fiecare release. Vezi
[carpatos](https://github.com/devopsyields/carpatos) pentru
sursele si tool-urile (`deb2cpm`, `build-cpm-repo`, `cpm`).

Configurare client:
```sh
echo "https://github.com/devopsyields/carpatos-repo/releases/download/<tag>" \
  | sudo tee /etc/cpm/repo.url
cpm update
cpm install <pkg>
```
