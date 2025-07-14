

- IOBluetooth
- IOBluetoothSDPServiceAttribute
-  init(id:attributeElementValue:) 

Initializer

# init(id:attributeElementValue:)

Initializes a new service attribute with the given ID and element value.

macOS

``` source
init!(
    id newAttributeID: BluetoothSDPServiceAttributeID,
    attributeElementValue: NSObject!
)
```

## Parameters 

`newAttributeID`  

The attribute ID of the new service attribute.

`attributeElementValue`  

The data element value of the new service attribute

## Return Value

Returns self if successful. Returns nil if there was an error parsing the element value.

## Discussion

See +\[IOBluetoothSDPDataElement withElementValue:\] for a description of the types that may be passed in as the attributeElementValue.

## See Also

### Initializers

init!(id: BluetoothSDPServiceAttributeID, attributeElement: IOBluetoothSDPDataElement!)

Initializes a new service attribute with the given ID and data element.

