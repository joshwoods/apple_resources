

- AVFoundation
- AVMutableMetadataItem
-  dataType 

Instance Property

# dataType

The data type of the metadata item’s value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var dataType: String? { get set }
```

## See Also

### Accessing Values

var value: (any NSCopying &amp; NSObjectProtocol)?

The value for the mutable metadata item.

var extraAttributes: [AVMetadataExtraAttributeKey : Any]?

A dictionary of additional attributes for a metadata item.

var stringValue: String?

The value of the metadata item as a string.

var numberValue: NSNumber?

The value of the metadata item as a number.

var dateValue: Date?

The value of the metadata item as a date.

var dataValue: Data?

The value of the metadata item as a data value.

