

- HomeKit
-  HMCharacteristicMetadataFormatTLV8 

Global Variable

# HMCharacteristicMetadataFormatTLV8

Indicates that the characteristic has TLV8 values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicMetadataFormatTLV8: String
```

## Discussion

The value is an NSData object containing a set of one or more TLV8’s, which are packed type-length-value items with an 8-bit type, 8-bit length, and N-byte value.

## See Also

### Data

let HMCharacteristicMetadataFormatData: String

Indicates that the characteristic has data blob values.

