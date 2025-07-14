

- Kernel
- Hardware Families
- FireWire
- IOFWAsyncCommand
-  setMaxPacket 

# setMaxPacket

``` source
IOReturn setMaxPacket(
 UInt32maxBytes) 
```

## Parameters 

`maxBytes`  

Maximum packet size in bytes. If the maxsize is 4 then quadlet transfers will be used.

## Overview

Sets the maximum size for block transfers used by the command. The command is initialized to use the maximum packet size calculated from the device's PHY speed, bus info block and the bus topology. Call this method before calling submit().

