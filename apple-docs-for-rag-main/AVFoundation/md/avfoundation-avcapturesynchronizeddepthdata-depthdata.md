

- AVFoundation
- AVCaptureSynchronizedDepthData
-  depthData 

Instance Property

# depthData

The depth data captured at this synchronization point.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var depthData: AVDepthData { get }
```

## Discussion

If the depthDataWasDropped property is true, this AVDepthData object does not contain a depth map (instead, it contains only metadata).

This value is equivalent to that provided by the depthDataOutput(_:didOutput:timestamp:connection:) or depthDataOutput(_:didDrop:timestamp:connection:reason:) delegate method when using a depth capture output without a data output synchronizer.

