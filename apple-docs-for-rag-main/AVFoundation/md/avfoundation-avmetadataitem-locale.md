

- AVFoundation
- AVMetadataItem
-  locale 

Instance Property

# locale

The locale of the metadata item.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var locale: Locale? { get }
```

## Discussion

The locale may be `nil` if no locale information is available for the metadata item.

## See Also

### Accessing Language Support

var extendedLanguageTag: String?

The IETF BCP 47 (RFC 4646) language identifier of the metadata item.

