

- AVFoundation
- AVMediaSelectionGroup
-  mediaSelectionOptions(from:with:) 

Type Method

# mediaSelectionOptions(from:with:)

Returns an array containing the media selection options from a given array that match the specified locale.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class func mediaSelectionOptions(
    from mediaSelectionOptions: [AVMediaSelectionOption],
    with locale: Locale
) -> [AVMediaSelectionOption]
```

## Parameters 

`mediaSelectionOptions`  

An array of AVMediaSelectionOption objects to be filtered.

`locale`  

The locale that must be matched for a media selection option to be copied to the output array.

## Return Value

An array containing the media selection options from `array` that match the `locale`.

## See Also

### Filtering Selection Options

class func playableMediaSelectionOptions(from: [AVMediaSelectionOption]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that are playable.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], withoutMediaCharacteristics: [AVMediaCharacteristic]) -> [AVMediaSelectionOption]

Returns an array containing the media selection options from a given array that do not match given media characteristics.

class func mediaSelectionOptions(from: [AVMediaSelectionOption], filteredAndSortedAccordingToPreferredLanguages: [String]) -> [AVMediaSelectionOption]

Returns an array of media selection options, filtering them according to whether their locales match one of the specified languages.

