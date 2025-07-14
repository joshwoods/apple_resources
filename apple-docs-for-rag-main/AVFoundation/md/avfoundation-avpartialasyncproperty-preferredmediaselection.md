

- AVFoundation
- AVPartialAsyncProperty
-  preferredMediaSelection 

Type Property

# preferredMediaSelection

The default media selections for the media selection groups of an asset.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var preferredMediaSelection: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Media Selections

static var allMediaSelections: AVAsyncProperty&lt;Root, [AVMediaSelection]>

The available media selections for an asset.

static var availableMediaCharacteristicsWithMediaSelectionOptions: AVAsyncProperty&lt;Root, [AVMediaCharacteristic]>

The media characteristics that provide media selection options.

func loadMediaSelectionGroup(for: AVMediaCharacteristic, completionHandler: (AVMediaSelectionGroup?, (any Error)?) -> Void)

Loads a media selection group that contains one or more options with the specified media characteristic.

