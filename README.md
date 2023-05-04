# vscode-extensions

One liner:

With `wget`:

``` bash
wget -qO- https://raw.githubusercontent.com/manuelgustavo/vscode-extensions/main/vscode-extensions.sh | bash
```

With `curl`:

``` bash
/bin/bash -c "$(curl -sS https://raw.githubusercontent.com/manuelgustavo/vscode-extensions/main/vscode-extensions.sh)"
```

Generated with:

``` bash
echo '#!/bin/sh' >vscode-extensions.sh && \
code --list-extensions | xargs -L 1 echo code --install-extension >>vscode-extensions.sh && \
chmod +x vscode-extensions.sh
```
