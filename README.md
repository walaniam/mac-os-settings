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
Use Eclipse (Windows) modified keymap (copy default and save as ```Eclipse - custom```. It should be available somewhere in ```~/Library/Application\ Support/JetBrains/IntelliJIdea2022.3/keymaps/Eclipse\ -\ custom.xml```)
```xml
<keymap version="1" name="Eclipse - custom" parent="Eclipse">
  <action id="$Copy">
    <keyboard-shortcut first-keystroke="ctrl c" />
    <keyboard-shortcut first-keystroke="meta c" />
  </action>
  <action id="$Cut">
    <keyboard-shortcut first-keystroke="ctrl x" />
    <keyboard-shortcut first-keystroke="shift delete" />
    <keyboard-shortcut first-keystroke="meta x" />
  </action>
  <action id="$Paste">
    <keyboard-shortcut first-keystroke="ctrl v" />
    <keyboard-shortcut first-keystroke="meta v" />
    <keyboard-shortcut first-keystroke="shift help" />
  </action>
  <action id="Back">
    <keyboard-shortcut first-keystroke="alt left" />
    <mouse-shortcut keystroke="button4" />
    <keyboard-shortcut first-keystroke="meta left" />
  </action>
  <action id="CallHierarchy">
    <keyboard-shortcut first-keystroke="ctrl alt h" />
    <keyboard-shortcut first-keystroke="ctrl meta h" />
  </action>
  <action id="ChangesView.Rename" />
  <action id="ChangesView.SetDefault" />
  <action id="Editor Copy">
    <keyboard-shortcut first-keystroke="ctrl c" />
    <keyboard-shortcut first-keystroke="meta c" />
  </action>
  <action id="Editor Cut">
    <keyboard-shortcut first-keystroke="ctrl x" />
    <keyboard-shortcut first-keystroke="meta x" />
  </action>
  <action id="Editor Paste">
    <keyboard-shortcut first-keystroke="ctrl v" />
    <keyboard-shortcut first-keystroke="meta v" />
    <keyboard-shortcut first-keystroke="shift help" />
  </action>
  <action id="ExtractMethod">
    <keyboard-shortcut first-keystroke="shift alt m" />
    <keyboard-shortcut first-keystroke="meta m" />
  </action>
  <action id="Forward">
    <keyboard-shortcut first-keystroke="alt right" />
    <mouse-shortcut keystroke="button5" />
    <keyboard-shortcut first-keystroke="meta right" />
  </action>
  <action id="Generate">
    <keyboard-shortcut first-keystroke="meta help" />
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
  <action id="NextProjectWindow">
    <keyboard-shortcut first-keystroke="ctrl alt close_bracket" />
    <keyboard-shortcut first-keystroke="meta back_quote" />
  </action>
  <action id="RenameElement">
    <keyboard-shortcut first-keystroke="shift meta r" />
  </action>
  <action id="SaveAll">
    <keyboard-shortcut first-keystroke="ctrl s" />
    <keyboard-shortcut first-keystroke="meta s" />
  </action>
  <action id="Scala.ShowImplicits">
    <keyboard-shortcut first-keystroke="shift ctrl alt equals" />
    <keyboard-shortcut first-keystroke="shift ctrl alt add" />
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
