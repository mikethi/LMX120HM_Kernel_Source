# LMX120HM_Kernel_Source
LMX120HM_Kernel_Source Android Pie 4.4

Use an explicit absolute repository path when running commands:

```sh
export REPO_DIR="/PATH/TO/LMX120HM_Kernel_Source" # replace with your local repo path
cd "$REPO_DIR"
```

Create and run a local helper script with a heredoc:

```sh
bash <<'SCRIPT'
#!/usr/bin/env bash
set -euo pipefail

cd "${REPO_DIR:?REPO_DIR must be set (see instructions above)}"

echo "Using repository at: $PWD"
mkdir -p out
echo "Prepared output directory: $PWD/out"
SCRIPT
```
