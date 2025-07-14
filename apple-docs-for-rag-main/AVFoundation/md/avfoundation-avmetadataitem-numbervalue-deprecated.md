

- AVFoundation
- AVMetadataItem
-  numberValue Deprecated

Instance Property

# numberValue

The value of the metadata item as a number.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var numberValue: NSNumber? { get }
```

Deprecated

Load the value of numberValue asynchronously instead.

## Discussion

This value is `nil` if the system can’t represent the value as a number.

## See Also

### Accessing Values

var value: (any NSCopying &amp; NSObjectProtocol)?

The value of the metadata item.

Deprecated

var extraAttributes: [AVMetadataExtraAttributeKey : Any]?

A dictionary of additional attributes for a metadata item.

Deprecated

var stringValue: String?

The value of the metadata item as a string.

Deprecated

var dateValue: Date?

The value of the metadata item as a date.

Deprecated

var dataValue: Data?

The value of the metadata item as a data value.

Deprecated

