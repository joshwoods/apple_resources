

- AVFoundation
- AVAsset
-  mediaSelectionGroup(forMediaCharacteristic:) Deprecated

Instance Method

# mediaSelectionGroup(forMediaCharacteristic:)

Returns a media selection group that contains one or more options with the specified media characteristic.

iOS 5.0–16.0DeprecatediPadOS 5.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func mediaSelectionGroup(forMediaCharacteristic mediaCharacteristic: AVMediaCharacteristic) -> AVMediaSelectionGroup?
```

Deprecated

Use loadMediaSelectionGroup(for:completionHandler:) instead.

## Parameters 

`mediaCharacteristic`  

A media characteristic for which to obtain the available media selection options.

Only audible, visual, and legible are currently supported.

- Pass audible to return the group of available options for audio media in various languages and for various purposes, such as descriptive audio.

- Pass legible to return the group of available options for subtitles in various languages and for various purposes.

- Pass visual to return the group of available options for video media.

## Return Value

An AVMediaSelectionGroup that contains one or more options with the specified media characteristic, or `nil` if none could be found.

## Mentioned in 

Selecting Subtitles and Alternative Audio Tracks

## Discussion

Use the filtering methods AVMediaSelectionGroup defines to filter the group’s options according to playability, locale, and additional media characteristics.

You can call this method without blocking the current thread after you’ve asynchronously loaded the availableMediaCharacteristicsWithMediaSelectionOptions property.

