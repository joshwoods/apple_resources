

- AVFoundation
- AVMutableMetadataItem
-  extraAttributes 

Instance Property

# extraAttributes

A dictionary of additional attributes for a metadata item.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var extraAttributes: [AVMetadataExtraAttributeKey : Any]? { get set }
```

## See Also

### Accessing Values

var value: (any NSCopying &amp; NSObjectProtocol)?

The value for the mutable metadata item.

var dataType: String?

The data type of the metadata item’s value.

var stringValue: String?

The value of the metadata item as a string.

var numberValue: NSNumber?

The value of the metadata item as a number.

var dateValue: Date?

The value of the metadata item as a date.

var dataValue: Data?

The value of the metadata item as a data value.

