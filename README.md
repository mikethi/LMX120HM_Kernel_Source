# LMX120HM_Kernel_Source
LMX120HM_Kernel_Source Android Pie 4.4

Use an explicit absolute repository path when running commands:

```sh
export REPO_DIR="/path/to/LMX120HM_Kernel_Source" # replace with your local repo path
cd "$REPO_DIR"
```

Create and run a local helper script with a heredoc:

```sh
cat <<'SCRIPT' > /tmp/lmx120hm_setup.sh
#!/usr/bin/env bash
set -euo pipefail

cd "${REPO_DIR:?Set REPO_DIR before running this script}"

echo "Using repository at: $PWD"
mkdir -p out
echo "Prepared output directory: $PWD/out"
SCRIPT

bash /tmp/lmx120hm_setup.sh && rm /tmp/lmx120hm_setup.sh
```
