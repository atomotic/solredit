# solredit

a dirty hack of tools to search documents from a solr core, filter results, preview and edit a single document.


### requirements

[solrdump](https://github.com/ubleipzig/solrdump), [jq](https://github.com/stedolan/jq), [fzf](https://github.com/junegunn/fzf), [curl](https://curl.se/)

```
apt install jq fzf curl
go get github.com/ubleipzig/solrdump/...
```

### configuration

tweak env in .envrc (use [direnv](https://direnv.net/))
```bash
export SOLR=http://localhost:8983/solr/core
export FIELD=title
export FZF_DEFAULT_OPTS="--info inline --layout=reverse --border"
```

### usage

```
./solredit (solr query, default to *:*)
```

[![asciicast](https://asciinema.org/a/378012.svg)](https://asciinema.org/a/378012)
