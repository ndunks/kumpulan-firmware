 
 #Tools
 
 Using ch341a_spi and `flashrom` on linux
 
 #Detecting
Example loop until detected
``` bash
while ! sudo flashrom -p ch341a_spi --flash-name; do echo Retry.. ; sleep 3; done
```

#Reading
``` bash
flashrom -p ch341a_spi -r rom.bin
```

#Writing
``` bash
flashrom -p ch341a_spi -n -w rom.bin
```

