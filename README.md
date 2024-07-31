# global-config
根据配置文件yaml或者环境变量生成项目全局变量

## install
```bash
pip install git+https://github.com/aigc-open/global-config.git
```

## GlobalConfig(全局配置，可文件可环境变量)

```python
from global_config import GlobalConfig
class GlobalConfig_(GlobalConfig):
    name:str="xxx"


global_config = GlobalConfig_()
global_config.init_config(path=".conf/config.yaml")
global_config.init_env()
```