# crewai-sgraal

Sgraal memory governance for CrewAI agents.

```bash
pip install crewai-sgraal
```

```python
from crewai_sgraal import SgraalMemoryGuard

guard = SgraalMemoryGuard(api_key="sg_demo_playground", domain="fintech")
safe = guard.validate(memories, action_type="irreversible")
```

## License
Apache 2.0


---

Sgraal SDK — Apache 2.0 license. Wraps the paid Sgraal API. Calibrated scoring requires an API key from [sgraal.com](https://sgraal.com).
