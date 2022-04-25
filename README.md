# vscode-extensions

Generated with:
``` sh
echo '#!/bin/sh' >vscode-extensions.sh && \
code --list-extensions | xargs -L 1 echo code --install-extension >>vscode-extensions.sh && \
chmod +x vscode-extensions.sh
```