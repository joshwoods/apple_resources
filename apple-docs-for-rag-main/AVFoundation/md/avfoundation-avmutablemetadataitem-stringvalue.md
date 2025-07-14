

- AVFoundation
- AVMutableMetadataItem
-  stringValue 

Instance Property

# stringValue

The value of the metadata item as a string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var stringValue: String? { get }
```

## Discussion

This value is `nil` if the system can’t represent the value as a string.

## See Also

### Accessing Values

var value: (any NSCopying &amp; NSObjectProtocol)?

The value for the mutable metadata item.

var extraAttributes: [AVMetadataExtraAttributeKey : Any]?

A dictionary of additional attributes for a metadata item.

var dataType: String?

The data type of the metadata item’s value.

var numberValue: NSNumber?

The value of the metadata item as a number.

var dateValue: Date?

The value of the metadata item as a date.

var dataValue: Data?

The value of the metadata item as a data value.

