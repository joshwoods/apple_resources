

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  getAttributeDataElement(\_:) 

Instance Method

# getAttributeDataElement(\_:)

Returns the data element for the given attribute ID in the target service.

macOS

``` source
func getAttributeDataElement(_ attributeID: BluetoothSDPServiceAttributeID) -> IOBluetoothSDPDataElement!
```

## Parameters 

`attributeID`  

The attribute ID of the desired attribute.

## Return Value

Returns the data element for the given attribute ID in the target service. If the service does not contain an attribute with the given ID, then nil is returned.

