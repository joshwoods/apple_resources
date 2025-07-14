

- Kernel
- Hardware Families
- FireWire
- IOFireWireDevice
-  init 

# init

Initializes the nub.

``` source
virtual bool init(
 OSDictionary *propTable,
 const IOFWNodeScan *scan); 
```

## Parameters 

`propTable`  

Property table passed to the standard nub initialization.

`scan`  

Pointer to the node scan structure.

## Return Value

Returns `true` if initialization was successful; `false` otherwise.

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

setMaxSpeed

Sets the maximum speed for this node.

setNodeFlags

Sets the node's characteristics.

