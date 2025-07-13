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

II. Postman

```
[Desktop Entry]
Name=Postman
Comment=Postman
Exec=/home/erojas/Programs/postman/Postman
Terminal=false
Type=Application
StartupNotify=true
Icon=/home/erojas/Programs/postman/app/icons/icon_128x128.png
Categories=Development;
Keywords=postman;
```

III. VisualVM

```
[Desktop Entry]
Name=VisualVM
Comment=VsualVM
Exec=/home/erojas/Programs/visualvm/bin/visualvm
Terminal=false
Type=Application
StartupNotify=true
Icon=/home/erojas/Programs/visualvm/bin/visualvm.svg
Categories=Development;IDE;Debugger;Profiling
Keywords=visualvm;
```

IV. Jmeter

Script: run\_jmeter.sh

```
#!/bin/bash

# Cargar SDKMAN! si lo usas

if \[ -f "$HOME/.sdkman/bin/sdkman-init.sh" \]; then  
source "$HOME/.sdkman/bin/sdkman-init.sh"  
fi

# Cargar Java Home (si no usas SDKMAN!)

# export JAVA\_HOME=/path/to/your/java

# Ejecutar JMeter

/home/erojas/Programs/jmeter/bin/jmeter.sh
```

desktop

```
[Desktop Entry]
Name=JMeter  
Comment=JMeter  
Exec=/home/erojas/Programs/jmeter/run\_jmeter.sh  
Terminal=false  
Type=Application  
StartupNotify=true  
Icon=/home/erojas/Programs/jmeter/docs/images/jmeter.png  
Categories=Development;Testing;Profiling  
Keywords=jmeter;
```

V. Pycharm Comunyity
```
[Desktop Entry]
Name=Pycharm Comunity
Comment=The Most Intelligent Python IDE
Exec=/home/erojas/Programs/pycharm/bin/pycharm.sh
Terminal=false
Type=Application
StartupNotify=true
Icon=/home/erojas/Programs/pycharm/bin/pycharm.svg
Categories=Development;IDE;Debugger;Profiling
Keywords=python;
```