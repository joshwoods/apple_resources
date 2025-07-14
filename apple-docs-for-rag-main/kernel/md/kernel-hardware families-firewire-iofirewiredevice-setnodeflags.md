

- Kernel
- Hardware Families
- FireWire
- IOFireWireDevice
-  setNodeFlags 

# setNodeFlags

Sets the node's characteristics.

``` source
virtual void setNodeFlags(
 UInt32flags ); 
```

## Parameters 

`flags`  

Refer to "node flags" in IOFireWireFamilyCommon.h.

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

setMaxSpeed

Sets the maximum speed for this node.

