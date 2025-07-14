

- AVFoundation
- AVMediaSelectionGroup
-  mediaSelectionOptions(from:withMediaCharacteristics:) 

Type Method

# mediaSelectionOptions(from:withMediaCharacteristics:)

Returns an array containing the media selection options from a given array that match given media characteristics.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func mediaSelectionOptions(
    from mediaSelectionOptions: [AVMediaSelectionOption],
    withMediaCharacteristics mediaCharacteristics: [AVMediaCharacteristic]
) -> [AVMediaSelectionOption]
```

## Parameters 

`mediaSelectionOptions`  

An array of AVMediaSelectionOption objects to be filtered.

`mediaCharacteristics`  

The media characteristics that must be matched for a media selection option to be present in the output array.

## Return Value

An array containing the media selection options from `array` that match `mediaCharacteristics`.

## See Also

### Filtering Selection Options

class func playableMediaSelectionOptions(from: [AVMediaSelectionOption]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that are playable.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], with: Locale) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that match the specified locale.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withoutMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that do not match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMediaSelectionOption]

Returns an array of media selection options, filtering them according to whether their locales match one of the specified languages.

