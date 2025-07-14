

- IOBluetooth
- IOBluetoothSDPServiceAttribute
-  init(id:attributeElement:) 

Initializer

# init(id:attributeElement:)

Initializes a new service attribute with the given ID and data element.

macOS

``` source
init!(
    id newAttributeID: BluetoothSDPServiceAttributeID,
    attributeElement: IOBluetoothSDPDataElement!
)
```

## Parameters 

`newAttributeID`  

The attribute ID of the new service attribute.

`attributeElement`  

The data element of the new service attribute.

## Return Value

Returns self if successful. Returns nil if there was an error.

## See Also

### Initializers

init!(id: BluetoothSDPServiceAttributeID, attributeElementValue: NSObject!)

Initializes a new service attribute with the given ID and element value.

