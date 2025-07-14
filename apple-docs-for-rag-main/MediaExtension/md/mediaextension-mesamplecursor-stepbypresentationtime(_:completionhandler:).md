

- MediaExtension
- MESampleCursor
-  stepByPresentationTime(\_:completionHandler:) 

Instance Method

# stepByPresentationTime(\_:completionHandler:)

Moves the cursor on the presentation timeline by the delta presentation time that you specify.

macOS 14.0+

``` source
func stepByPresentationTime(
    _ deltaPresentationTime: CMTime,
    completionHandler: @escaping (CMTime, Bool, (any Error)?) -> Void
)
```

``` source
func stepByPresentationTime(_ deltaPresentationTime: CMTime) async throws -> (CMTime, Bool)
```

**Required**

## Parameters 

`deltaPresentationTime`  

The presentation time to move the sample cursor to.

`completionHandler`  

The completion block to execute when the move operation finishes.

## Discussion

The value for `actualDecodeTime` is the final cursor presentation time. Because sample cursors snap to sample boundaries when stepped, this value may not be equal to the current sample decode time + `deltaPresentationTime`, even if the cursor isn’t pinned.

If the request would advance the cursor past the end of the last sample or before the first sample, this method sets the cursor to point to that limiting sample, and sets `positionWasPinned` to true. Otherwise, it sets `positionWasPinned` to false.

## See Also

### Stepping through samples

func samplesWithEarlierDTSsMayHaveLaterPTSs(than: any MESampleCursor) -> Bool

Tests for an earlier boundary in sample reordering.

func samplesWithLaterDTSsMayHaveEarlierPTSs(than: any MESampleCursor) -> Bool

Tests for a later boundary in sample reordering.

func estimatedSampleLocation() throws -> MEEstimatedSampleLocation

Returns an estimate of the sample location indicated by the cursor.

func refineSampleLocation(AVSampleCursorStorageRange, refinementData: UnsafePointer&lt;UInt8>, refinementDataLength: Int, refinedLocation: UnsafeMutablePointer&lt;AVSampleCursorStorageRange>) throws

Produces an exact sample location based on the estimated sample location and refinement data that you specify.

func stepByDecodeTime(CMTime, completionHandler: (CMTime, Bool, (any Error)?) -> Void)

Moves the cursor on the decode timeline by the delta decode time that you specify.

**Required**

func stepInDecodeOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in decode order.

**Required**

func stepInPresentationOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in presentation order.

**Required**

