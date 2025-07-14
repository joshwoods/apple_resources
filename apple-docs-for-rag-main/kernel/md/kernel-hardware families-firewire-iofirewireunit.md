

- Kernel
- Hardware Families
- FireWire
-  IOFireWireUnit 

Class

# IOFireWireUnit

macOS 10.0+

``` source
class IOFireWireUnit : IOFireWireNub
```

## Topics

### Instance Methods

- attach

- clearNodeFlags

- createAuxiliary

- createPhysicalAddressSpace

- createPseudoAddressSpace

- free

- getMetaClass

- getNodeFlags

- handleClose

- handleOpen

- init

- matchPropertyTable

- message

- setConfigDirectory

- setMaxSpeed

- setNodeFlags

- terminateUnit

### Type Methods

+ terminateUnitThreadFunc

## Relationships

### Inherits From

- IOFireWireNub

## See Also

### Nubs

IOFireWireLocalNode

IOFireWireSBP2LUN

Provider for most drivers.

IOFireWireAVCSubUnit

nub for sub unit of AVC devices. Just for matching, calls the AVC unit for all functions.

IOFireWireAVCUnit

nub for AVC devices

IOFireWireAVCNub

nub for AVC devices

IOFireWireNub

