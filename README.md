# Mini-Projects

#!/bin/bash
echo "# 🚀 Mini Projects" > README.md
echo "| Date | Project | Description |" >> README.md
echo "|------|---------|-------------|" >> README.md

for d in */ ; do
    if [[ "$d" != .* ]]; then
        echo "| $(date +%Y-%m-%d) | [${d%/}](./${d}) | TODO: Add description |" >> README.md
    fi
done
