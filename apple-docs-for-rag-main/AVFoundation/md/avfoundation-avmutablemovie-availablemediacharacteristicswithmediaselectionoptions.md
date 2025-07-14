

- AVFoundation
- AVMutableMovie
-  availableMediaCharacteristicsWithMediaSelectionOptions 

Instance Property

# availableMediaCharacteristicsWithMediaSelectionOptions

An array of media characteristics for which a media selection option is available.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+visionOS 1.0+watchOS 1.0+

``` source
var availableMediaCharacteristicsWithMediaSelectionOptions: [AVMediaCharacteristic] { get }
```

## See Also

### Accessing Media Selections

var allMediaSelections: [AVMediaSelection]

The array of available media selections for this asset.

func mediaSelectionGroup(forMediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?

Returns a media selection group that contains one or more options with the specified media characteristic.

