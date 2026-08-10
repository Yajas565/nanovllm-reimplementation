## About this repo
Re-implementation of Xingkai Yu's [nano-vllm](https://github.com/GeeeekExplorer/nano-vllm), built to deeply understand production LLM serving internals — paged KV cache, continuous batching, tensor parallelism, and request scheduling.

**Approach:** read every line of the original -> reimplement each file from memory -> diff my implementation against the reference to catch bugs and correct wrong assumptions.


**Next:** move to studying real vLLM and contributing small PRs.


## Installation
> flash-attn requires a two-step install due to CUDA build isolation issues.

- pip install torch packaging setuptools psutil
- pip install flash-attn --no-build-isolation
- pip install -e .

## Verification
Ran both implementations on the same prompt and confirmed matching output tokens and comparable latency, confirming the reimplementation is functionally equivalent to the reference.