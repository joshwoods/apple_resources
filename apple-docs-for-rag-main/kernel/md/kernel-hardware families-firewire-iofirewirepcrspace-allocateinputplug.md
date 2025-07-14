

- Kernel
- Hardware Families
- FireWire
- IOFireWirePCRSpace
-  allocateInputPlug 

# allocateInputPlug

allocates an input plug.

``` source
virtual IOReturn allocateInputPlug(
 void *refcon,
 IOFireWirePCRCallbackfunc,
 UInt32 &plug); 
```

## Parameters 

`refcon`  

arbitrary value passed back as first argument of callback.

`func`  

callback function when a successful lock transaction to the plug has been performed

`plug`  

set to the plug number if a plug is successfully allocated

## See Also

### Miscellaneous

allocateOutputPlug

allocates an output plug.

clearAllP2PConnections

freeInputPlug

deallocates an input plug.

freeOutputPlug

deallocates an output plug.

getPCRAddressSpace

returns the IOFireWirePCRSpace object for the given FireWire bus

init

initializes the IOFireWirePCRSpace object

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

