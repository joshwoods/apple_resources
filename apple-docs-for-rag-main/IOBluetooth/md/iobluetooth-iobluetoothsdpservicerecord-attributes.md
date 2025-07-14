

- IOBluetooth
- IOBluetoothSDPServiceRecord
-  attributes 

Instance Property

# attributes

Returns an NSDictionary containing the attributes for the service.

macOS

``` source
var attributes: [AnyHashable : Any]! { get }
```

## Return Value

Returns an NSDictionary containing the attributes for the target service.

## Discussion

The attribute dictionary is keyed off of the attribute id represented as an NSNumber. The values in the NSDictionary are IOBluetoothSDPDataElement objects representing the data element for the given attribute.

