- this is a re-implementation of Xingkai Yu's nano-vllm to understand how paged attention, continuous batching, tensor parallelism, schedulers, block manager works

- here i understodd each and every line of the real nano vllm and then reimplemented it from memory and diff against reference 

- as now i have the basic idea of how inference is happening in the real production environments like(vLLM), i will try to understand the vLLM and learn the required topics on the go.

- Original repo:-> github.com/GeeeekExplorer/nano-vllm


## Installation
> flash-attn requires a two-step install due to CUDA build isolation issues.

- pip install torch packaging setuptools psutil
- pip install flash-attn --no-build-isolation
- pip install -e .