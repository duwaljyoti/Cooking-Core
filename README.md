## Project setup

Project setup instructions here. => =>f => updated 

```bash
mkdir -p local
cp cooking_core/project/settings/templates/settings.dev.py ./local/settings.dev.py
cp cooking_core/project/settings/templates/settings.unittests.py ./local/settings.unittests.py
```

```bash
make shell

from cooking_core.config.models import Config
Config.objects.create(owner=None, transaction_fee=1)
```
