# yaml2json
Simple bash alias for convert **YAML** to **JSON**

## Instalation
Install Ruby and add to `.bashrc` code:

```bash
alias yaml2json="ruby -ryaml -rjson -e 'puts JSON.pretty_generate(YAML.load(ARGF))'"
```

## Usage
cat file.yaml | yaml2json

For parsing JSON use `jq`
