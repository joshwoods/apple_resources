

- AVFoundation
- AVMutableMetadataItem
-  numberValue 

Instance Property

# numberValue

The value of the metadata item as a number.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var numberValue: NSNumber? { get }
```

## Discussion

This value is `nil` if the system can’t represent the value as a number.

## See Also

### Accessing Values

var value: (any NSCopying &amp; NSObjectProtocol)?

The value for the mutable metadata item.

var extraAttributes: [AVMetadataExtraAttributeKey : Any]?

A dictionary of additional attributes for a metadata item.

var dataType: String?

The data type of the metadata item’s value.

var stringValue: String?

The value of the metadata item as a string.

var dateValue: Date?

The value of the metadata item as a date.

var dataValue: Data?

The value of the metadata item as a data value.

