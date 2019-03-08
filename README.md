# es-iconsthemes-ORIGINAL
Iconos originales para ES y ES-DEV

NOTA: COMO SABER QUE VERSION DE ES TENGO INSTALADA?
Ejecute este comando en la terminal "Lo puede ver con winCSP tambien": ls -all /opt/masos/supplementary/
ahora busque en la lista el directorio emulationstation u emulationstation-dev ,puede que x alguna razon
tenga los dos directorios ,no se preocupe y use los pasos para EmulationStation-dev.

###################### EmulationStation ######################
info: Para EmulationStation siga estos pasos desde la terminal....

sudo killall emulationstation

cd && mkdir temporal

cd temporal && git clone https://github.com/DOCK-PI3/es-iconsthemes-ORIGINAL.git

sudo cp -R ~/temporal/es-iconsthemes-ORIGINAL/*.svg /opt/masos/supplementary/emulationstation/resources/help/

sudo chown -R $user:$user /opt/masos/supplementary/emulationstation/

sudo rm -R ~/temporal/es-iconsthemes-ORIGINAL/

emulationstation

###################### EmulationStation-dev ######################
info: Para EmulationStation-dev siga estos pasos desde la terminal....

sudo killall emulationstation

cd && mkdir temporal

cd temporal && git clone https://github.com/DOCK-PI3/es-iconsthemes-ORIGINAL.git

sudo cp -R ~/temporal/es-iconsthemes-ORIGINAL/*.svg /opt/masos/supplementary/emulationstation-dev/resources/help/

sudo chown -R $user:$user /opt/masos/supplementary/emulationstation-dev/

sudo rm -R ~/temporal/es-iconsthemes-ORIGINAL/

emulationstation
