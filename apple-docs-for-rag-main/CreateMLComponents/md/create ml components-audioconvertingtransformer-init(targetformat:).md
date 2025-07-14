

- Create ML Components
- AudioConvertingTransformer
-  init(targetFormat:) 

Initializer

# init(targetFormat:)

Creates an audio conversion transformer to convert the format of the buffers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(targetFormat: AVAudioFormat)
```

## Parameters 

`targetFormat`  

The desired audio format for the output buffers.

## Discussion

- Precondition The `targetFormat` must have an AVAudioPCMFormat as its common format type.

