

- AVFoundation
- AVAssetWriter
-  canAdd(\_:) 

Instance Method

# canAdd(\_:)

Determines whether the asset writer supports adding the input group.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func canAdd(_ inputGroup: AVAssetWriterInputGroup) -> Bool
```

## Parameters 

`inputGroup`  

The asset writer input group to add.

## Return Value

true if you can add the input group to the asset writer; otherwise false.

## Discussion

This method returns false if the asset writer’s output file type doesn’t support mutually exclusive relationships among tracks, or if the input group contains inputs with media types that you can’t relate.

## See Also

### Configuring Input Groups

var inputGroups: [AVAssetWriterInputGroup]

The input groups an asset writer contains.

func add(AVAssetWriterInputGroup)

Adds an input group to an asset writer.

