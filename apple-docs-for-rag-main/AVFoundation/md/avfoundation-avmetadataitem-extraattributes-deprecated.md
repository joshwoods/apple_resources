

- AVFoundation
- AVMetadataItem
-  extraAttributes Deprecated

Instance Property

# extraAttributes

A dictionary of additional attributes for a metadata item.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var extraAttributes: [AVMetadataExtraAttributeKey : Any]? { get }
```

Deprecated

Load the value of extraAttributes asynchronously instead.

## Discussion

Extra attributes, when they’re present, are specific to metadata container formats and keys in their associated key-spaces. For example, a metadata item can represent the “attached picture” frame defined by the ID3 tag specification with keyspace id3 and key id3MetadataKeyAttachedPicture, a value that carries the image data, and extra attributes that include a description of the picture as carried in the ‘APIC’ frame of the ID3 tag.

## See Also

### Accessing Values

var value: (any NSCopying &amp; NSObjectProtocol)?

The value of the metadata item.

Deprecated

var stringValue: String?

The value of the metadata item as a string.

Deprecated

var numberValue: NSNumber?

The value of the metadata item as a number.

Deprecated

var dateValue: Date?

The value of the metadata item as a date.

Deprecated

var dataValue: Data?

The value of the metadata item as a data value.

Deprecated

