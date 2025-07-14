

- AVFoundation
- AVAssetTrack
-  hasMediaCharacteristic(\_:) Deprecated

Instance Method

# hasMediaCharacteristic(\_:)

Returns a Boolean value that indicates whether the track references media with the specified media characteristic.

iOS 4.0–16.0DeprecatediPadOS 4.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
func hasMediaCharacteristic(_ mediaCharacteristic: AVMediaCharacteristic) -> Bool
```

Deprecated

Load the value of mediaCharacteristics asynchronously instead.

## Parameters 

`mediaCharacteristic`  

The media characteristic of interest.

## Return Value

true if the track references media with the specified characteristic, otherwise false.

