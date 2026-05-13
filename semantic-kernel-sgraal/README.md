# semantic-kernel-sgraal

Sgraal preflight validation bridge for [Microsoft Semantic Kernel](https://github.com/microsoft/semantic-kernel).

## Install

```bash
pip install semantic-kernel-sgraal
```

## Usage

```python
from semantic_kernel_sgraal import SemanticKernelSgraal

sgraal = SemanticKernelSgraal("sg_demo_playground", domain="coding")

memories = await kernel.memory.search("project_docs", "deployment process")
if sgraal.is_safe([m.text for m in memories]):
    # proceed with kernel invocation
    pass
```


---

Sgraal SDK — Apache 2.0 license. Wraps the paid Sgraal API. Calibrated scoring requires an API key from [sgraal.com](https://sgraal.com).
