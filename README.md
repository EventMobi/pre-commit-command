# pre-commit-command

[pre-commit][] hook to run a project-defined command.

### Usage
Add this to your **.pre-commit-config.yaml**:

```yaml
-  repo: git://github.com/EventMobi/pre-commit-command
   sha: 'master'
   hooks:
   -  id: command
      files: \.txt$
      args: [somecommand, --some-args]
```

##### Example

```yaml
-  repo: git://github.com/EventMobi/pre-commit-command
   sha: 'master'
   hooks:
   -  id: command
      files: \.js$
      args: [./node_modules/.bin/eslint, --fix]
```

[pre-commit]: https://github.com/pre-commit/pre-commit
