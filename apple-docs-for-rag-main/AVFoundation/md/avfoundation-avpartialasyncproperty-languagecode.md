

- AVFoundation
- AVPartialAsyncProperty
-  languageCode 

Type Property

# languageCode

The language code of the track.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var languageCode: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

The value is an ISO 639-2/T language code, or `nil` if the track doesn’t specify a language code.

## See Also

### Loading Language Support

static var extendedLanguageTag: AVAsyncProperty&lt;Root, String?>

The language tag of the track.

