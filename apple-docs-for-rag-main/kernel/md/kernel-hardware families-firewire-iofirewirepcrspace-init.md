

- Kernel
- Hardware Families
- FireWire
- IOFireWirePCRSpace
-  init 

# init

initializes the IOFireWirePCRSpace object

``` source
virtual bool init(
 IOFireWireBus *bus); 
```

## See Also

### Miscellaneous

allocateInputPlug

allocates an input plug.

allocateOutputPlug

allocates an output plug.

clearAllP2PConnections

freeInputPlug

deallocates an input plug.

freeOutputPlug

deallocates an output plug.

getPCRAddressSpace

returns the IOFireWirePCRSpace object for the given FireWire bus

readInputMasterPlug

Returns the current value of the primary input plug.

readInputPlug

returns the current value of an input plug.

readOutputMasterPlug

Returns the current value of the primary output plug.

readOutputPlug

returns the current value of an output plug.

setAVCTargetSpacePointer

updateInputMasterPlug

Updates the value of the primary input plug (simulating a lock transaction).

updateInputPlug

updates the value of an input plug (simulating a lock transaction).

updateOutputMasterPlug

Updates the value of the primary output plug (simulating a lock transaction).

updateOutputPlug

updates the value of an output plug (simulating a lock transaction).

