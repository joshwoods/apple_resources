

- Kernel
- Hardware Families
- FireWire
- IOFireWireAVCTargetSpace
-  getAVCTargetSpace 

# getAVCTargetSpace

returns the IOFireWireAVCTargetSpace object for the given FireWire bus

``` source
static IOFireWireAVCTargetSpace *getAVCTargetSpace(
 IOFireWireController *bus); 
```

## Parameters 

`bus`  

The FireWire bus

## See Also

### Miscellaneous

init

initializes the IOFireWireAVCTargetSpace object

publishAVCUnitDirectory

Creates a local AVC Unit directory if it doesn't already exist

