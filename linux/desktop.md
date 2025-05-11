# Hands on create desktop

## Path

I. Specific user: `~/.local/share/applications/`  
II. All user: `/usr/share/applications/`

## Desktop

I. Create desktop

`touch ~/.local/share/applications/intellij-idea.desktop`

II. Docs desktop

`nano ~/.local/share/applications/intellij-idea.desktop`

III. Permisions

A. Desktop

`chmod +x ~/.local/share/applications/intellij-idea.desktop`

B. Exec command

`chmod +x /home/erojas/Programs/idea/bin/idea.sh`

IV. Update db desktop

`update-desktop-database ~/.local/share/applications`  

## Examples

I. IntelliJ IDEA

```
[Desktop Entry]
Name=IntelliJ IDEA
Comment=The Most Intelligent Java IDE
Exec=/home/erojas/Programs/idea/bin/idea.sh
Terminal=false
Type=Application
StartupNotify=true
Icon=/home/erojas/Programs/idea/bin/idea.png
Categories=Development;IDE;Debugger;Profiling
Keywords=idea;
```