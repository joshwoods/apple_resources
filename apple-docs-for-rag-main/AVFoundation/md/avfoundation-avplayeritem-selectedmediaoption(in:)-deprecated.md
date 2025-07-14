

- AVFoundation
- AVPlayerItem
-  selectedMediaOption(in:) Deprecated

Instance Method

# selectedMediaOption(in:)

Returns the media selection option that’s currently selected from the specified group.

iOS 5.0–11.0DeprecatediPadOS 5.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.13DeprecatedtvOS 9.0–11.0Deprecated

``` source
@MainActor
func selectedMediaOption(in mediaSelectionGroup: AVMediaSelectionGroup) -> AVMediaSelectionOption?
```

Deprecated

Use currentMediaSelection instead.

## Parameters 

`mediaSelectionGroup`  

A media selection group obtained from the player item’s asset.

## Return Value

An instance of AVMediaSelectionOption that describes the currently selected option in the group.

## Discussion

If the value of the allowsEmptySelection property of `mediaSelectionGroup` is true, the currently selected option in the group may be `nil`.

