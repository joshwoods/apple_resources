

- AVFoundation
- AVPlayerItemMetadataOutputPushDelegate
-  metadataOutput(\_:didOutputTimedMetadataGroups:from:) 

Instance Method

# metadataOutput(\_:didOutputTimedMetadataGroups:from:)

Tells the delegate a new collection of metadata items is available.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
optional func metadataOutput(
    _ output: AVPlayerItemMetadataOutput,
    didOutputTimedMetadataGroups groups: [AVTimedMetadataGroup],
    from track: AVPlayerItemTrack?
)
```

## Parameters 

`output`  

The AVPlayerItemMetadataOutput source.

`groups`  

An array of `AVTimedMetadataGroups` that contain metadata items with requested identifiers, according to the format descriptions associated with the underlying tracks.

`track`  

An instance of AVPlayerItemTrack that indicates the source of the metadata items in the group.

## Discussion

Each group provided in a single invocation of this method will have timing that does not overlap with any other group in the array.

Note that for some timed metadata formats carried by HTTP live streaming, the `timeRange` of each group must be reported as indefinite, because its duration will be unknown until the next metadata group in the stream arrives. In these cases, the groups parameter will always contain a single group.

Groups are typically packaged into arrays for delivery to your delegate according to the chunking or interleaving of the underlying metadata data.

Note that if the item carries multiple metadata tracks containing metadata with the same metadata identifiers, this method can be invoked for each one separately, each with reference to the associated AVPlayerItemTrack.

