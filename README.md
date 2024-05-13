# Comandos para inicializar o repositório

```text
git init -b main

npm init -y

npm install @commitlint/cli @commitlint/config-conventional --save-dev

echo "module.exports = { extends: ['@commitlint/config-conventional'] };" > commitlint.config.js

npx husky init

rm .husky/pre-commit

echo "npx --no -- commitlint --edit \$1" > .husky/commit-msg

npm install commitizen --save-dev

commitizen init cz-conventional-changelog --save-dev --save-exact --force

npm install --save-dev standard-version
```

## Facilitador das mensagens de commit

```text
git cz
```

## Como gerar o CHANGELOG.MD

```text
npx standard-version
```
