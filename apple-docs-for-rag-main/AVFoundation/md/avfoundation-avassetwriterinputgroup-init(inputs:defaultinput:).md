

- AVFoundation
- AVAssetWriterInputGroup
-  init(inputs:defaultInput:) 

Initializer

# init(inputs:defaultInput:)

Creates a group for the asset writer inputs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
init(
    inputs: [AVAssetWriterInput],
    defaultInput: AVAssetWriterInput?
)
```

## Parameters 

`inputs`  

The inputs with tracks to arrange into a mutually exclusive group.

`defaultInput`  

The group’s default input.

## Discussion

When you add an input group to an asset writer, the system sets the default input’s marksOutputTrackAsEnabled property value to true, and the value of the other inputs in the group to false.

