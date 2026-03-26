# llama.cpp-llm-settings-for-23B-A3B

Settings for GLM-4.7-FLASH-23B-A3B for RTX5060ti

## Quick Start

Save the following configuration in a file named `llm.sh` and execute it to start the server with optimized settings for RTX5060ti.

```bash
#!/bin/bash

llama-server -m /home/extra/llamacpp-models/unsloth_GLM-4.7-Flash-REAP-23B-A3B-GGUF_GLM-4.7-Flash-REAP-23B-A3B-UD-Q4_K_XL.gguf \
-c 185600 \
-ctk q8_0 \
-ctv q8_0 \
-fa on \
-ncmoe 20 \
--top-p 1.0 \
--temp 0.7 \
--min-p 0.01 \
-fit on \
-fitc 185600 \
-lv 3 \
--webui-mcp-proxy
```
to run `llm.sh` execute the following commands in terminal

```bash
bash llm.sh
```
