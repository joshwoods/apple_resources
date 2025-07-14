

- AVFoundation
- AVAssetWriterInputMetadataAdaptor
-  append(\_:) 

Instance Method

# append(\_:)

Appends a timed metadata group to the adaptor.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func append(_ timedMetadataGroup: AVTimedMetadataGroup) -> Bool
```

## Parameters 

`timedMetadataGroup`  

The timed metadata group to append.

## Return Value

true if the adaptor appends the group; otherwise, false.

## Discussion

The timing of metadata items in the output asset correspond to the time range of the timed metadata group, regardless of the values of their individual time and duration properties.

Important

Only call this method after you’ve attached the related input to the asset writer and called its startWriting() method.

