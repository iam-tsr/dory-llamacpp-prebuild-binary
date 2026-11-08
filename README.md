# llama.cpp NVIDIA Dory1.0-4B Pre-build Binaries

## Recommended command to run the server

```
llama-server \
    -hf nvidia/NVIDIA-Nemotron-Labs-Dory1.0-4B-GGUF:Q5_K_M \
    --alias dory \
    --host 127.0.0.1 \
    --port 8080 \
    -ngl 999 \
    --ctx-size 4096 \
    --parallel 1 \
    --cache-type-k f16 \
    --cache-type-v f16 \
    --flash-attn off \
    --no-context-shift \
    --jinja \
    --reasoning on \
    --no-ui \
    --temp 1.0
```