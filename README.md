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

### Keyboard key modifiers (for Windows keyboard)
In case of using Windows keyboard, remap your 'Command' and 'Option' keys (Big thanks to https://9to5mac.com/2016/03/17/how-to-remap-windows-keyboard-buttons-match-mac-layout/)

## Intellij
### Eclipse keymap (more like Windows one)
Use Eclipse (Windows) modified keymap (copy default and save as ```Eclipse - custom```. It should be available somewhere in ```~/Library/Application\ Support/JetBrains/IntelliJIdea2022.2/keymaps/Eclipse\ -\ custom.xml```)
```xml
<keymap version="1" name="Eclipse_custom" parent="Eclipse">
  <action id="CallHierarchy">
    <keyboard-shortcut first-keystroke="ctrl alt h" />
    <keyboard-shortcut first-keystroke="ctrl meta h" />
  </action>
  <action id="ChangesView.Rename" />
  <action id="ChangesView.SetDefault" />
  <action id="ExtractMethod">
    <keyboard-shortcut first-keystroke="shift alt m" />
    <keyboard-shortcut first-keystroke="meta m" />
  </action>
  <action id="Git.Rename.Local.Branch" />
  <action id="IntroduceConstant">
    <keyboard-shortcut first-keystroke="ctrl alt c" />
    <keyboard-shortcut first-keystroke="ctrl meta c" />
  </action>
  <action id="IntroduceField">
    <keyboard-shortcut first-keystroke="ctrl alt f" />
    <keyboard-shortcut first-keystroke="ctrl meta f" />
  </action>
  <action id="IntroduceFunctionalParameter">
    <keyboard-shortcut first-keystroke="shift ctrl alt p" />
    <keyboard-shortcut first-keystroke="shift ctrl meta p" />
  </action>
  <action id="IntroduceParameter">
    <keyboard-shortcut first-keystroke="ctrl alt p" />
    <keyboard-shortcut first-keystroke="ctrl meta p" />
  </action>
  <action id="IntroduceVariable">
    <keyboard-shortcut first-keystroke="shift alt l" />
    <keyboard-shortcut first-keystroke="ctrl meta v" />
  </action>
  <action id="RenameElement">
    <keyboard-shortcut first-keystroke="shift meta r" />
  </action>
  <action id="ShelvedChanges.Rename">
    <keyboard-shortcut first-keystroke="shift meta r" />
  </action>
  <action id="ShowIntentionActions">
    <keyboard-shortcut first-keystroke="ctrl 1" />
    <keyboard-shortcut first-keystroke="alt enter" />
    <keyboard-shortcut first-keystroke="meta enter" />
  </action>
</keymap>
```
