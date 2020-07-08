# Branch naming rules
<img alt="GitHub Actions status" src="https://github.com/deepakputhraya/action-pr-title/workflows/main/badge.svg">

Github action to enforce Pull Request title conventions

## Usage

See [action.yml](./action.yml)

```yaml
steps:
- uses: naveenk1223/action-pr-title@master
  with:
    regex: '.+' # Regex the title should match.
    allowed_prefixes: 'feature,fix,bugfix,patch,enhancement,hotfix' # title should start with the given prefix
    prefix_case_sensitive: false # title prefix are case insensitive
    min_length: 10 # Min length of the title
    max_length: -1 # Max length of the title
```

## License
The scripts and documentation in this project are released under the [MIT License](./LICENSE)
