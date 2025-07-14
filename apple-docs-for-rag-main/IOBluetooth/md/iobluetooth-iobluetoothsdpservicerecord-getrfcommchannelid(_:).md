

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  getRFCOMMChannelID(\_:) 

Instance Method

# getRFCOMMChannelID(\_:)

Allows the discovery of the RFCOMM channel ID assigned to the service.

macOS

``` source
func getRFCOMMChannelID(_ rfcommChannelID: UnsafeMutablePointer!) -> IOReturn
```

## Parameters 

`rfcommChannelID`  

A pointer to the location that will get the found RFCOMM channel ID.

## Return Value

Returns kIOReturnSuccess if the channel ID is found.

## Discussion

This method will search through the ProtoclDescriptorList attribute to find an entry with the RFCOMM UUID (UUID16: 0x0003). If one is found, it gets the second element of the data element sequence and sets the rfcommChannelID pointer to it. The channel ID only gets set when kIOReturnSuccess is returned.

