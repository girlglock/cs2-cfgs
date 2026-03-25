launchoptions:
```
+exec_async autoexec -novconsole -disable_workshop_command_filtering -testscript "../../csgo/cfg/.vtest" -allow_third_party_software
```

`+exec_async autoexec` can be replaced with regular exec, its only used to bypass -tools restrictions

`-novconsole` can be removed, its just to force pano console with -tools

`-disable_workshop_command_filtering` makes aliased binds work on workshop maps

`-testscript "../../csgo/cfg/.vtest"` unused source 2 test scripting system, similar to exec_async, can loop indefinitely, no sv_cheats flag

`-allow_third_party_software` to make obs work
