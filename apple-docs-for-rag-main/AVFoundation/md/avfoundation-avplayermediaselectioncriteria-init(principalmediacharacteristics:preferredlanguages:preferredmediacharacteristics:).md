

- AVFoundation
- AVPlayerMediaSelectionCriteria
-  init(principalMediaCharacteristics:preferredLanguages:preferredMediaCharacteristics:) 

Initializer

# init(principalMediaCharacteristics:preferredLanguages:preferredMediaCharacteristics:)

Creates media selection criteria with the principal media characteristics, and preferred languages and media characteristics.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
init(
    principalMediaCharacteristics: [AVMediaCharacteristic]?,
    preferredLanguages: [String]?,
    preferredMediaCharacteristics: [AVMediaCharacteristic]?
)
```

## Parameters 

`principalMediaCharacteristics`  

An array of media characteristics that are essential to selecting media with the characteristic. This value may be `nil`.

`preferredLanguages`  

An array of language identifier strings, in order of preference. This value may be `nil`.

`preferredMediaCharacteristics`  

An array of media characteristics, in order of preference. This value may be `nil`.

## Discussion

Principal media characteristics, when present, override language preferences when making selections within a specific media selection group. However, language preferences may still pertain to selections in other groups. For example, the system may consider language preferences when choosing whether to select nonforced subtitles for translation purposes.

## See Also

### Creating Media Selection Criteria

init(preferredLanguages: [String]?, preferredMediaCharacteristics: [AVMediaCharacteristic]?)

Creates media selection criteria with the preferred languages and media characteristics.

