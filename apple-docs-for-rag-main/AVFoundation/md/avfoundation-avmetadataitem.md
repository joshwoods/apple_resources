

- AVFoundation
-  AVMetadataItem 

Class

# AVMetadataItem

A metadata item for an audiovisual asset or one of its tracks.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMetadataItem
```

## Mentioned in 

Retrieving media metadata

Loading media data asynchronously

Presenting Chapter Markers

## Overview

To effectively use `AVMetadataItem`, you need to understand how AVFoundation organizes metadata. To simplify finding and filtering metadata items, the framework groups related metadata into key spaces:

- **Format-specific key spaces.** The framework defines several format-specific key spaces. They roughly correlate to a particular container or file format, such as QuickTime (QuickTime metadata and user data) or MP3 (ID3). However, a single asset may contain metadata values across multiple key spaces. To retrieve an asset’s complete collection of format-specific metadata, you use its metadata property.

- **Common key space.** There are several common metadata values, such as a movie’s creation date or description, that can exist across multiple key spaces. To help normalize access to this common metadata, the framework provides a common key space that gives access to a limited set of metadata values common to several key spaces. This makes it easy to retrieve commonly used metadata without concern for the specific format. To retrieve an asset’s collection of common metadata, you use its commonMetadata property.

Metadata items have keys that accord with the specification of the container format from which they’re drawn. Full details of the metadata formats, metadata keys, and metadata key spaces supported by AVFoundation are available in AVMetadataKeySpace and AVMetadataKey.

To load values of a metadata item when you access them for the first time, use the methods from the AVAsynchronousKeyValueLoading protocol. The AVAsset class and other classes in turn provide their metadata as needed so that you can obtain objects from those arrays without incurring overhead for items you don’t inspect.

To filter arrays of metadata items, you use the methods of this class. For example, you can filter by key and key space, by locale, and by preferred language.

## Topics

### Creating a Metadata Item

init(propertiesOfMetadataItem: AVMetadataItem, valueLoadingHandler: (AVMetadataItemValueRequest) -> Void)

Creates a metadata item whose value loads on an on-demand basis only.

class AVMetadataItemValueRequest

An object that responds to a request to load the value of a metadata item.

### Identifying Metadata Items

var identifier: AVMetadataIdentifier?

An identifier for a metadata item.

### Loading Values

var dataType: String?

The data type of the metadata item’s value.

static var value: AVAsyncProperty&lt;Root, (any NSCopying &amp; NSObjectProtocol)?>

The value of the metadata item.

static var stringValue: AVAsyncProperty&lt;Root, String?>

The value of the metadata item as a string.

static var numberValue: AVAsyncProperty&lt;Root, NSNumber?>

The value of the metadata item as a number.

static var dateValue: AVAsyncProperty&lt;Root, Date?>

The value of the metadata item as a date.

static var dataValue: AVAsyncProperty&lt;Root, Data?>

The value of the metadata item as a data value.

static var extraAttributes: AVAsyncProperty&lt;Root, [AVMetadataExtraAttributeKey : Any]?>

A dictionary of additional attributes for the item.

### Accessing Keys and Key Spaces

var key: (any NSCopying &amp; NSObjectProtocol)?

The key of the metadata item.

var commonKey: AVMetadataKey?

The common key of the metadata item.

var keySpace: AVMetadataKeySpace?

The key space for the metadata item’s key.

### Accessing Timing

var time: CMTime

The timestamp of the metadata item.

var startDate: Date?

The start date of the timed metadata.

var duration: CMTime

The duration of the metadata item.

### Accessing Language Support

var locale: Locale?

The locale of the metadata item.

var extendedLanguageTag: String?

The IETF BCP 47 (RFC 4646) language identifier of the metadata item.

### Filtering Arrays of Metadata Items

class func metadataItems(from: [AVMetadataItem], filteredByIdentifier: AVMetadataIdentifier) -> [AVMetadataItem]

Returns metadata items for the specified identifier.

class func metadataItems(from: [AVMetadataItem], withKey: Any?, keySpace: AVMetadataKeySpace?) -> [AVMetadataItem]

Returns metadata items that match a specified key or key space.

class func metadataItems(from: [AVMetadataItem], with: Locale) -> [AVMetadataItem]

Returns metadata items that match a specified locale.

class func metadataItems(from: [AVMetadataItem], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMetadataItem]

Returns metadata items whose locales match one of the specified language identifiers.

class func metadataItems(from: [AVMetadataItem], filteredBy: AVMetadataItemFilter) -> [AVMetadataItem]

Returns filtered metadata items.

### Translating Metadata Items

class func identifier(forKey: Any, keySpace: AVMetadataKeySpace) -> AVMetadataIdentifier?

Returns a metadata identifier for the specified key and key space.

class func key(forIdentifier: AVMetadataIdentifier) -> Any?

Returns a metadata key for the specified identifier.

class func keySpace(forIdentifier: AVMetadataIdentifier) -> AVMetadataKeySpace?

Returns a metadata key space for the specified identifier.

### Accessing Values

Prefer loading values asynchronously using the symbols in Loading Values.

var value: (any NSCopying &amp; NSObjectProtocol)?

The value of the metadata item.

Deprecated

var extraAttributes: [AVMetadataExtraAttributeKey : Any]?

A dictionary of additional attributes for a metadata item.

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

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableMetadataItem

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

class AVMutableMetadataItem

A mutable metadata item for an audiovisual asset or for one of its tracks.

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

