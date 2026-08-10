## Installation
> flash-attn requires a two-step install due to CUDA build isolation issues.

pip install torch packaging setuptools psutil
pip install flash-attn --no-build-isolation
pip install -e .