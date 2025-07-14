

- AVFoundation
- AVAssetWriter
-  add(\_:) 

Instance Method

# add(\_:)

Adds an input group to an asset writer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func add(_ inputGroup: AVAssetWriterInputGroup)
```

## Parameters 

`inputGroup`  

A compatible asset writer input group to add.

## Discussion

An asset writer marks tracks associated with grouped inputs as mutually exclusive to each other for playback or other processing, if the output container format supports mutually exclusive relationships among tracks.

When you add an input group to an asset writer, the system sets the value of the default input’s marksOutputTrackAsEnabled property to true and sets the values of the group’s other inputs to false.

You can’t add input groups after writing starts.

## See Also

### Configuring Input Groups

var inputGroups: [AVAssetWriterInputGroup]

The input groups an asset writer contains.

func canAdd(AVAssetWriterInputGroup) -> Bool

Determines whether the asset writer supports adding the input group.

