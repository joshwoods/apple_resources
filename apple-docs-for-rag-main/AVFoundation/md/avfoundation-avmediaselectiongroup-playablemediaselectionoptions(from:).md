

- AVFoundation
- AVMediaSelectionGroup
-  playableMediaSelectionOptions(from:) 

Type Method

# playableMediaSelectionOptions(from:)

Returns an array containing the media selection options from a given array that are playable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func playableMediaSelectionOptions(from mediaSelectionOptions: [AVMediaSelectionOption]) -> [AVMediaSelectionOption]
```

## Parameters 

`mediaSelectionOptions`  

An array of AVMediaSelectionOption objects to be filtered by playability.

## Return Value

An array containing the media selection options from `array` that are playable.

## See Also

### Filtering Selection Options

class func mediaSelectionOptions(from: [AVMediaSelectionOption], with: Locale) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that match the specified locale.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withoutMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that do not match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMediaSelectionOption]

Returns an array of media selection options, filtering them according to whether their locales match one of the specified languages.

