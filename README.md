
# Prusa MK3 Klipper Config

## THIS IS A WORK IN PROGRESS AND HAS NOT BEEN VALIDATED YET!

If you are interested in contributing or testing then contact KenadyDwag44 on the Unofficial Prusa Discord or 602 Discord.

Add this to moonraker for easy updates

```yml
[update_manager prusa]
type: git_repo
origin: https://github.com/PrusaOwners/Klipper_Configs.git
path: ~/klipper_config/config
primary_branch: main
is_system_service: False
```
