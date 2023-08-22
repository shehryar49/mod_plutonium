# mod_plutonium
A plutonium module for Apache2
This module is currently incomplete. It handles .plt extensions and returns a "hello world" response. 
# Compilation
  ```apxs -i -a -c plutonium.c```
  Create a configuration file plutonium.conf in mods-enabled directory with the following content
  
  ```
FilesMatch "\.plt">
    SetHandler plutonium-handler
</FilesMatch>
```
