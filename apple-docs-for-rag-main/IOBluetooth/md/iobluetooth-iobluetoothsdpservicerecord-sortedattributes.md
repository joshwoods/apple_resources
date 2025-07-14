

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  sortedAttributes 

Instance Property

# sortedAttributes

Returns a sorted array of SDP attributes

macOS

``` source
var sortedAttributes: [Any]! { get }
```

## Return Value

Returns a sorted array of SDP attributes

## Discussion

This method will walk all the elements of the service record and return an array of IOBluetoothSDPServiceAttribute objects sorted by attributeID

