<div align="center">
<h1>Auto-QuantLLM ⚡️ </h1>
<p>Quantize Large Language Models (LLMs) Locally with a Single Command</p>
</div>

## Overview

Auto-QuantLLM is a toolkit designed to simplify the Quantization of Large Language Models (LLMs) with an emphasis on ease of use and flexibility, Auto-QuantLLM supports conversion of LLM into different efficient formats for local deployment.


## Getting Started

### Installation

Clone the repository to get started with Auto-QuantLLM:

```bash
git clone https://github.com/monk1337/AutoQuantLLM.git
cd AutoQuantLLM
```


```bash
# Convert your Hugging Face model to GGUF format for local deployment
# Usage:
# ./scripts/autogguf.sh -m <MODEL_ID> [-u USERNAME] [-t TOKEN] [-q QUANTIZATION_METHODS]

# Example command:
./scripts/autogguf.sh -m unsloth/gemma-2b
```

### More Options
```bash
# if want to upload the gguf model to hub after the conversion, provide the user and token
# Example command:
./scripts/autogguf.sh -m unsloth/gemma-2b -u user_name -t hf_token


#if wants to provide QUANTIZATION_METHODS
# Example command:
./scripts/autogguf.sh -m unsloth/gemma-2b -u user_name -t hf_token -q "q4_k_m,q5_k_m"
```
