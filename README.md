# LMX120HM_Kernel_Source
LMX120HM_Kernel_Source Android Pie 4.4

Create and run a local helper script with a heredoc (using an explicit absolute path):

```sh
bash <<'SCRIPT'
#!/usr/bin/env bash
set -euo pipefail

REPO_DIR="/absolute/path/to/LMX120HM_Kernel_Source" # replace with your local repo path
cd "$REPO_DIR"

echo "Using repository at: $PWD"
mkdir -p out
echo "Prepared output directory: $PWD/out"
SCRIPT
```
