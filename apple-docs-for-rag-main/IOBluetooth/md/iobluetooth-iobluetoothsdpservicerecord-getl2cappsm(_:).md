

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  getL2CAPPSM(\_:) 

Instance Method

# getL2CAPPSM(\_:)

Allows the discovery of the L2CAP PSM assigned to the service.

macOS

``` source
func getL2CAPPSM(_ outPSM: UnsafeMutablePointer!) -> IOReturn
```

## Parameters 

`outPSM`  

A pointer to the location that will get the found L2CAP PSM.

## Return Value

Returns kIOReturnSuccess if the PSM is found.

## Discussion

This method will search through the ProtoclDescriptorList attribute to find an entry with the L2CAP UUID (UUID16: 0x0100). If one is found, it gets the second element of the data element sequence and sets the outPSM pointer to it. The PSM value only gets set when kIOReturnSuccess is returned.

