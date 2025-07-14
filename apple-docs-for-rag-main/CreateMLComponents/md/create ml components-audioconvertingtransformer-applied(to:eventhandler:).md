

- Create ML Components
- AudioConvertingTransformer
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Performs conversion of the input audio buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to input: AVAudioPCMBuffer,
    eventHandler: EventHandler? = nil
) throws -> AVAudioPCMBuffer
```

## Parameters 

`input`  

The audio buffer that will be converted.

`eventHandler`  

An event handler.

## Return Value

An output audio buffer by converting the input buffer to the `targetFormat`.

