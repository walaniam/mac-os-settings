# mac-os-settings

## Keyboard

### Remap key bindings
In file ~/Library/KeyBindings/DefaultKeyBinding.dict
```bash
/* Remap Home / End keys to be correct */
"\UF729" = "moveToBeginningOfLine:"; /* Home */
"\UF72B" = "moveToEndOfLine:"; /* End */
"$\UF729" = "moveToBeginningOfLineAndModifySelection:"; /* Shift + Home */
"$\UF72B" = "moveToEndOfLineAndModifySelection:"; /* Shift + End */
"^\UF729" = "moveToBeginningOfDocument:"; /* Ctrl + Home */
"^\UF72B" = "moveToEndOfDocument:"; /* Ctrl + End */
}'
```

### System Preferrences -> Keyboard -> Input Sources
Uncheck settings that use 'Space'

## Intellij
Use Eclipse (Windows) modified keymap (on mac OS it's ~/Library/Application\ Support/JetBrains/IntelliJIdea2022.2/keymaps/Eclipse\ -\ custom.xml
