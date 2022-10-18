# vscode-extensions
One liner:
```
/bin/bash -c "$(curl -sS https://raw.githubusercontent.com/manuelgustavo/vscode-extensions/main/vscode-extensions.sh)"
```
Generated with:
``` sh
echo '#!/bin/sh' >vscode-extensions.sh && \
code --list-extensions | xargs -L 1 echo code --install-extension >>vscode-extensions.sh && \
chmod +x vscode-extensions.sh
```
