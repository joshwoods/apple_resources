

- Kernel
- Hardware Families
- FireWire
- IOFireWireDevice
-  setMaxSpeed 

# setMaxSpeed

Sets the maximum speed for this node.

``` source
inline void setMaxSpeed(
 IOFWSpeedspeed ) 
```

## Parameters 

`speed`  

Maximum speed. Refer to "bus speed numbers" in IOFireWireFamilyCommon.h.

## See Also

### Miscellaneous

clearNodeFlags

Resets the node's characteristics.

createPhysicalAddressSpace

Creates local physical FireWire address spaces for the device to access.

createPseudoAddressSpace

Creates local pseudo FireWire address spaces for the device to access.

getNodeFlags

Retrieves the node's characteristics.

getUnitCount

Returns number of units attached to this device.

init

Initializes the nub.

setNodeFlags

Sets the node's characteristics.

