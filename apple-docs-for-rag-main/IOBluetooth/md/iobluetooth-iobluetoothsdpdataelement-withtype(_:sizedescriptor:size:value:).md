

- IOBluetooth
- IOBluetoothSDPDataElement
-  withType(\_:sizeDescriptor:size:value:) 

Type Method

# withType(\_:sizeDescriptor:size:value:)

Creates a new IOBluetoothSDPDataElement with the given attributes.

macOS

``` source
class func withType(
    _ type: BluetoothSDPDataElementTypeDescriptor,
    sizeDescriptor newSizeDescriptor: BluetoothSDPDataElementSizeDescriptor,
    size newSize: UInt32,
    value newValue: NSObject!
) -> Self!
```

## Parameters 

`type`  

The type descriptor for the data element.

`newSizeDescriptor`  

The size descriptor for the data element (verify it matches the size parameter).

`newSize`  

The size of the data element in bytes (make sure it is a valid size for the given size descriptor).

`newValue`  

The raw value itself. This must be the base NSString, NSNumber, NSArray or NSData objects. It may not be NSDictionary. If a dictionary format is present, use +withElementValue:.

## Return Value

Returns the newly allocated data element object. Returns nil if an error is encountered (not likely due to the limited error checking currently done). The returned IOBluetoothSDPDataElement object has been autoreleased, so it is not necessary for the caller to release it. If the object is to be referenced and kept around, retain should be called.

## Discussion

Warning - be careful using this method. There is next to no error checking done on the attributes. It is entirely possible to construct an invalid data element. It is recommended that +withElementValue: be used instead of this one.

