

- AVFAudio
- AVAudioUnitEQ
-  init(numberOfBands:) 

Initializer

# init(numberOfBands:)

Creates an audio unit equalizer object with the specified number of bands.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
init(numberOfBands: Int)
```

## Parameters 

`numberOfBands`  

The number of bands that the equalizer creates.

## Return Value

A new `AVAudioUnitEQ` instance.

## See Also

### Related Documentation

var bands: [AVAudioUnitEQFilterParameters]

An array of equalizer filter parameters.

