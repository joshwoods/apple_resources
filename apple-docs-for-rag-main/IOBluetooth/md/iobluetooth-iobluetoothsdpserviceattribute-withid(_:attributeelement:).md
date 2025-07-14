

- IOBluetooth
- IOBluetoothSDPServiceAttribute
-  withID(\_:attributeElement:) 

Type Method

# withID(\_:attributeElement:)

Creates a new service attribute with the given ID and data element.

macOS

``` source
class func withID(
    _ newAttributeID: BluetoothSDPServiceAttributeID,
    attributeElement: IOBluetoothSDPDataElement!
) -> Self!
```

## Parameters 

`newAttributeID`  

The attribute ID of the new service attribute.

`attributeElement`  

The data element of the new service attribute.

## Return Value

Returns the newly allocated service attribute object. Returns nil if there was an error. The returned IOBluetoothSDPDataElement object has been autoreleased, so it is not necessary for the caller to release it. If the object is to be referenced and kept around, retain should be called.

