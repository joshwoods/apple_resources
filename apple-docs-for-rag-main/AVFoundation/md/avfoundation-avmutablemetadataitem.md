

- AVFoundation
-  AVMutableMetadataItem 

Class

# AVMutableMetadataItem

A mutable metadata item for an audiovisual asset or for one of its tracks.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMutableMetadataItem
```

## Overview

You can initialize a mutable metadata item from an existing AVMetadataItem object or with a one or more of the basic properties of a metadata item: a key, a key space, a locale, and a value.

## Topics

### Identifying Metadata Items

var identifier: AVMetadataIdentifier?

Indicates the identifier of the metadata item.

### Accessing Keys and Key Spaces

var key: (any NSCopying &amp; NSObjectProtocol)?

The key for a mutable metadata item.

var keySpace: AVMetadataKeySpace?

The key space of the metadata item’s key.

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

var dateValue: Date?

The value of the metadata item as a date.

var dataValue: Data?

The value of the metadata item as a data value.

### Accessing Timing

var time: CMTime

The timestamp for a mutable metadata item.

var startDate: Date?

The start date of the timed metadata.

var duration: CMTime

The duration of a mutable metadata item.

### Accessing Language Support

var locale: Locale?

The locale for a mutable metadata item.

var extendedLanguageTag: String?

The IETF BCP 47 (RFC 4646) language identifier of the metadata item.

## Relationships

### Inherits From

- AVMetadataItem

### Conforms To

- AVAsynchronousKeyValueLoading
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Metadata

Retrieving media metadata

Load descriptive metadata for media assets and their tracks.

class AVMetadataItem

A metadata item for an audiovisual asset or one of its tracks.

struct AVMetadataIdentifier

A structure that defines identifiers for metadata formats.

struct AVMetadataKey

A structure that defines a metadata key.

struct AVMetadataKeySpace

A structure that defines a metadata key space.

struct AVMetadataExtraAttributeKey

A structure that defines keys for extra metadata attributes.

struct AVMetadataFormat

A structure that defines metadata formats.

class AVMetadataItemFilter

An object that filters selected information from a metadata item.

