# yaml2json
Simple bash alias for convert **YAML** to **JSON**

## Instalation with Ruby
Install Ruby and add to `.bashrc` code:

```bash
alias yaml2json="ruby -ryaml -rjson -e 'puts JSON.pretty_generate(YAML.load(ARGF))'"
```

## Instalation with Python
Install Python and add to `.bashrc` code:

```bash
alias yaml2json="python -c 'import sys,yaml,json; print(json.dumps(yaml.safe_load(str(sys.stdin.read()))))'"
```

## Usage
cat file.yaml | yaml2json

For parsing JSON use `jq`
