

- Kernel
- Hardware Families
- ATA
- ATADeviceNub
-  MyATACallback 

# MyATACallback

to be deprecated.

``` source
static void MyATACallback(
 IOATACommand *command ); 
```

## See Also

### Miscellaneous

allocCommand

create command objects for clients.

ataDeviceNub

static creator function - used by IOATAControllers to create nubs.

attach

override of IOService method.

executeCommand

Submit IO requests

freeCommand

Clients use this method to dispose of command objects.

getDeviceID

get the unit id of this drive (0 or 1)

init

used after creating the nub.

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

