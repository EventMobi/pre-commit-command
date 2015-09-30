# pre-commit-command-js

[pre-commit][] hook to run a project-defined command on files ending in **.js**

### Usage
Add this to your **.pre-commit-config.yaml**:

```yaml
-  repo: git://github.com/EventMobi/pre-commit-command-js
   sha: 'master'
   hooks:
   -  id: command-js
      args: [somecommand, --some-args]
```

##### Example

```yaml
-  repo: git://github.com/EventMobi/pre-commit-command-js
   sha: 'master'
   hooks:
   -  id: command-js
      args: [./node_modules/.bin/eslint, --fix]
```

[pre-commit]: https://github.com/pre-commit/pre-commit
