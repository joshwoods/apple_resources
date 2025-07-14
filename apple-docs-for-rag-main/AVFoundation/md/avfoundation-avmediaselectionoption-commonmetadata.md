

- AVFoundation
- AVMediaSelectionOption
-  commonMetadata 

Instance Property

# commonMetadata

An array of metadata items for each common metadata key for which a value is available.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var commonMetadata: [AVMetadataItem] { get }
```

## Discussion

You can filter the array of AVMetadataItem objects according to locale using metadataItems(from:with:), key using metadataItems(from:withKey:keySpace:), or language using metadataItems(from:filteredAndSortedAccordingToPreferredLanguages:).

Clients that are filtering media selection options by language should be prepared to handle cases in which the extendedLanguageTag property value is `nil`. Further, they should be prepared to handle cases in which an `extendedLanguageTag` is present but indicates that the language is “undetermined” (a language value of @“und”, as defined in ISO 639-2).

## See Also

### Managing Metadata

var availableMetadataFormats: [String]

The metadata formats that contain metadata associated with the option.

func metadata(forFormat: String) -> [AVMetadataItem]

Returns an array of metadata items—one for each metadata item in the container of a given format.

