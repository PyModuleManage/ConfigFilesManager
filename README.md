# ConfigFilesManager
A python module to a easy manage configs files for applications


# Why?
This module help you to manage configurations files of python applications.
So, you can check the value or type of a variable in configuration file, without to 
have write more code. You can check if a required variables is present or not. And then 
raise (or not) Exceptions.


# Sample
```python
from configFilesManager import configFilesManager

schema = {'CONFIG': {'IP': {'type': 'str', 'required': True},
                        'TIMEOUT_DB_MS': {'type': 'int', 'required': True},
                        'PORT': {'type': 'int', 'required': True},
                        'DB_NAME': {'type': 'str', 'required': True},
                        'INSTALL_PATH': {'type': 'str', 'required': True}}}

config = 'path/to/config.ini'

cfm = configFilesManager(config, schema)
cfm.is_correct_information()

```


# Contribution

Please see CONTRIBUTE.md