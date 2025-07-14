

- AVFoundation
- AVComposition
-  mediaSelectionGroup(forMediaCharacteristic:) 

Instance Method

# mediaSelectionGroup(forMediaCharacteristic:)

Returns a media selection group that contains one or more options with the specified media characteristic.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func mediaSelectionGroup(forMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?
```

## Parameters 

`mediaCharacteristic`  

A media characteristic for which to obtain the available media selection options.

Only audible, visual, and legible are currently supported.

- Pass audible to return the group of available options for audio media in various languages and for various purposes, such as descriptive audio.

- Pass legible to return the group of available options for subtitles in various languages and for various purposes.

- Pass visual to return the group of available options for video media.

## Return Value

An AVMediaSelectionGroup that contains one or more options with the specified media characteristic, or `nil` if none could be found.

## Discussion

Use the filtering methods AVMediaSelectionGroup defines to filter the group’s options according to playability, locale, and additional media characteristics.

You can call this method without blocking the current thread after you’ve asynchronously loaded the availableMediaCharacteristicsWithMediaSelectionOptions property.

## See Also

### Accessing Media Selections

var allMediaSelections: [AVMediaSelection]

The array of available media selections for this asset.

var availableMediaCharacteristicsWithMediaSelectionOptions: [AVMediaCharacteristic]

An array of media characteristics for which a media selection option is available.

