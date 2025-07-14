

- AVFoundation
- AVMediaSelectionOption
-  mediaType 

Instance Property

# mediaType

The media type of the media data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var mediaType: AVMediaType { get }
```

## Discussion

The value of the property might be, for example, audio or subtitle.

## See Also

### Accessing Media Information

var mediaSubTypes: [NSNumber]

The media sub-types of the media data associated with the option.

func hasMediaCharacteristic(AVMediaCharacteristic) -> Bool

Returns a Boolean value that indicates whether the receiver has media with the given media characteristic.

