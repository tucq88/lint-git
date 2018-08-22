# Lint Git
With [conventional commit](https://conventionalcommits.org/) rules
---

## Conventional commit
```
<type>[optional scope]: <description>

[optional body]

[optional footer]
```
- *type* must be one of `build, chore, ci, docs, feat, fix, perf, refactor, revert, style, test`
- *scope* would be context of commit:
```
feat(lang): added polish language
refactor(home): cleanup dashboard service
```
- *description* is a short description of the code changes, no more than 50 chars

## Prerequisites
- [husky](https://github.com/typicode/husky):
```
npm install husky@next --save-dev
```
- [commitlint](https://github.com/marionebl/commitlint):
```
# Install commitlint cli and angular config
npm install --save-dev @commitlint/{config-conventional,cli}
# For Windows:
npm install --save-dev @commitlint/config-conventional @commitlint/cli

# Configure commitlint to use angular config
echo "module.exports = {extends: ['@commitlint/config-conventional']}" > commitlint.config.js
```