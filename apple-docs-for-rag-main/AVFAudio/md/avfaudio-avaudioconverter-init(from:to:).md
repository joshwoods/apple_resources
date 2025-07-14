

- AVFAudio
- AVAudioConverter
-  init(from:to:) 

Initializer

# init(from:to:)

Creates an audio converter object from the specified input and output formats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init?(
    from fromFormat: AVAudioFormat,
    to toFormat: AVAudioFormat
)
```

## Parameters 

`fromFormat`  

The input audio format.

`toFormat`  

The audio format to convert to.

## Return Value

An AVAudioConverter instance, or `nil` if the format conversion isn’t possible.

