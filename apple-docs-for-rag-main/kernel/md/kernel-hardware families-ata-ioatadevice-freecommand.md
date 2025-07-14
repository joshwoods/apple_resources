

- Kernel
- Hardware Families
- ATA
- IOATADevice
-  freeCommand 

# freeCommand

release a command object that is no longer needed. Do not free an object in use and do not release the object anymore times than you have retained it.

``` source
virtual void freeCommand(
 IOATACommand *inCommand); 
```

## Parameters 

`inCommand`  

the command to be released.

## See Also

### Miscellaneous

allocCommand

create IOATACommands. Device drivers should allocate command objects only through this method.

executeCommand

Submit IO requests

getDeviceType

Find out what kind of device this nub is (ata or atapi)

getUnitID

Determine whether this device is number 0 or 1 (ie, primary/secondary)

matchLocation

matching stuff for IOBSDInit and so on.

matchPropertyTable(OSDictionary *)

matching stuff for IOBSDInit and so on.

matchPropertyTable(OSDictionary *, SInt32 *)

matching stuff for IOBSDInit and so on.

notifyEvent

called by controllers when they need to send a message to client (disk) drivers.

provideBusInfo

Find out the bus capability so the client can choose the features to set and commands to run.

provideConfig

Find out what speed the bus has configured for this unit.

selectConfig

Tell the bus what speed to use for your device.

