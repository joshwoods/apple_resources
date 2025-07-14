

- Kernel
- Hardware Families
- FireWire
- IOFWLocalIsochPort
-  notify 

# notify

Informs hardware of a change to the DCL program.

``` source
virtual IOReturn notify( 
 IOFWDCLNotificationTypenotificationType, 
 DCLCommand **dclCommandList, 
 UInt32numDCLCommands ); 
```

## Parameters 

`notificationType`  

Type of change.

`dclCommandList`  

List of DCL commands that have been changed.

`numDCLCommands`  

Number of commands in list.

## Return Value

IOKit error code.

