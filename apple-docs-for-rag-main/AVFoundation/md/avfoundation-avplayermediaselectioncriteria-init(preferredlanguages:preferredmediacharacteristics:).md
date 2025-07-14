

- AVFoundation
- AVPlayerMediaSelectionCriteria
-  init(preferredLanguages:preferredMediaCharacteristics:) 

Initializer

# init(preferredLanguages:preferredMediaCharacteristics:)

Creates media selection criteria with the preferred languages and media characteristics.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init(
    preferredLanguages: [String]?,
    preferredMediaCharacteristics: [AVMediaCharacteristic]?
)
```

## Parameters 

`preferredLanguages`  

An array of language identifier strings, in order of preference. This value may be `nil`.

`preferredMediaCharacteristics`  

An array of media characteristics, in order of preference. This value may be `nil`.

## See Also

### Creating Media Selection Criteria

init(principalMediaCharacteristics: [AVMediaCharacteristic]?, preferredLanguages: [String]?, preferredMediaCharacteristics: [AVMediaCharacteristic]?)

Creates media selection criteria with the principal media characteristics, and preferred languages and media characteristics.

