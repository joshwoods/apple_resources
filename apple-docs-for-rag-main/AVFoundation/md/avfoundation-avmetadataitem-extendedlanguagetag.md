

- AVFoundation
- AVMetadataItem
-  extendedLanguageTag 

Instance Property

# extendedLanguageTag

The IETF BCP 47 (RFC 4646) language identifier of the metadata item.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var extendedLanguageTag: String? { get }
```

## Discussion

The value may be `nil` if no language tag information is available.

## See Also

### Accessing Language Support

var locale: Locale?

The locale of the metadata item.

