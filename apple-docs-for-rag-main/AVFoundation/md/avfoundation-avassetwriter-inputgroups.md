

- AVFoundation
- AVAssetWriter
-  inputGroups 

Instance Property

# inputGroups

The input groups an asset writer contains.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var inputGroups: [AVAssetWriterInputGroup] { get }
```

## Discussion

Add input groups to the asset writer using its add(_:) method.

## See Also

### Configuring Input Groups

func canAdd(AVAssetWriterInputGroup) -> Bool

Determines whether the asset writer supports adding the input group.

func add(AVAssetWriterInputGroup)

Adds an input group to an asset writer.

