

- AVFoundation
- AVPartialAsyncProperty
-  extendedLanguageTag 

Type Property

# extendedLanguageTag

The language tag of the track.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var extendedLanguageTag: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

The value is a BCP-47 language tag, or `nil` if the track doesn’t specify a language tag.

## See Also

### Loading Language Support

static var languageCode: AVAsyncProperty&lt;Root, String?>

The language code of the track.

