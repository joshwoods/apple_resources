

- IOBluetooth
- IOBluetoothSDPDataElement
-  init(elementValue:) 

Initializer

# init(elementValue:)

Initializes a new IOBluetoothSDPDataElement with the given value.

macOS

``` source
init!(elementValue element: NSObject!)
```

## Parameters 

`element`  

The data element value of one of the specified types.

## Return Value

Returns self if successful. Returns nil if there was an error parsing the element value.

## Discussion

The value must follow the format listed above and must be an instance of NSData, NSString, NSNumber, NSArray, NSDictionary, IOBluetoothSDPUUID.

## See Also

### Initializers

init!(type: BluetoothSDPDataElementTypeDescriptor, sizeDescriptor: BluetoothSDPDataElementSizeDescriptor, size: UInt32, value: NSObject!)

Initializes a new IOBluetoothSDPDataElement with the given attributes.

