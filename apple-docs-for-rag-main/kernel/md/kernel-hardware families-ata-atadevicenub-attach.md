

- Kernel
- Hardware Families
- ATA
- ATADeviceNub
-  attach 

# attach

override of IOService method.

``` source
virtual bool attach(
 IOService *provider ); 
```

## See Also

### Miscellaneous

allocCommand

create command objects for clients.

ataDeviceNub

static creator function - used by IOATAControllers to create nubs.

executeCommand

Submit IO requests

freeCommand

Clients use this method to dispose of command objects.

getDeviceID

get the unit id of this drive (0 or 1)

init

used after creating the nub.

MyATACallback

to be deprecated.

processCallback

to be deprecated.

publishBusProperties

puts info about this device's bus capability in the device tree.

publishProperties

publish the nub's properties in the device tree.

publishVendorProperties

will be deprecated.

swapBytes16

to be deprecated.

