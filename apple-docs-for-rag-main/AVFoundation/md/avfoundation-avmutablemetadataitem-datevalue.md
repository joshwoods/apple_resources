

- AVFoundation
- AVMutableMetadataItem
-  dateValue 

Instance Property

# dateValue

The value of the metadata item as a date.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var dateValue: Date? { get }
```

## Discussion

This value is `nil` if the system can’t represent the value as a date.

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

var numberValue: NSNumber?

The value of the metadata item as a number.

var dataValue: Data?

The value of the metadata item as a data value.

