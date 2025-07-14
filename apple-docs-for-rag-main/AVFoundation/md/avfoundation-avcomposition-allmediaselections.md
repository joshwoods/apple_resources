

- AVFoundation
- AVComposition
-  allMediaSelections 

Instance Property

# allMediaSelections

The array of available media selections for this asset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var allMediaSelections: [AVMediaSelection] { get }
```

## See Also

### Accessing Media Selections

var availableMediaCharacteristicsWithMediaSelectionOptions: [AVMediaCharacteristic]

An array of media characteristics for which a media selection option is available.

func mediaSelectionGroup(forMediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?

Returns a media selection group that contains one or more options with the specified media characteristic.

