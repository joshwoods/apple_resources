

- AVFoundation
- AVMediaSelectionOption
-  hasMediaCharacteristic(\_:) 

Instance Method

# hasMediaCharacteristic(\_:)

Returns a Boolean value that indicates whether the receiver has media with the given media characteristic.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func hasMediaCharacteristic(_ mediaCharacteristic: AVMediaCharacteristic) -> Bool
```

## Parameters 

`mediaCharacteristic`  

The media characteristic of interest, for example, visual, audible, or legible.

## Return Value

true if the media selection option has media with mediaCharacteristic, otherwise false.

## See Also

### Accessing Media Information

var mediaType: AVMediaType

The media type of the media data.

var mediaSubTypes: [NSNumber]

The media sub-types of the media data associated with the option.

