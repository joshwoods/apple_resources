

- IOBluetooth
- IOBluetoothSDPServiceAttribute
-  withID(\_:attributeElementValue:) 

Type Method

# withID(\_:attributeElementValue:)

Creates a new service attribute with the given ID and element value.

macOS

``` source
class func withID(
    _ newAttributeID: BluetoothSDPServiceAttributeID,
    attributeElementValue: NSObject!
) -> Self!
```

## Parameters 

`newAttributeID`  

The attribute ID of the new service attribute.

`attributeElementValue`  

The data element value of the new service attribute

## Return Value

Returns the newly allocated service attribute object. Returns nil if there was an error parsing the element value. The returned IOBluetoothSDPDataElement object has been autoreleased, so it is not necessary for the caller to release it. If the object is to be referenced and kept around, retain should be called.

## Discussion

See +\[IOBluetoothSDPDataElement withElementValue:\] for a description of the types that may be passed in as the attributeElementValue.

