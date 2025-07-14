

- MediaExtension
- MESampleCursor
-  stepInDecodeOrder(by:completionHandler:) 

Instance Method

# stepInDecodeOrder(by:completionHandler:)

Moves the cursor a given number of samples in decode order.

macOS 14.0+

``` source
func stepInDecodeOrder(
    by stepCount: Int64,
    completionHandler: @escaping (Int64, (any Error)?) -> Void
)
```

``` source
func stepInDecodeOrder(by stepCount: Int64) async throws -> Int64
```

**Required**

## Parameters 

`stepCount`  

The number of samples to move. If positive, the cursor steps forward. If negative, the cursor steps backward.

`completionHandler`  

The completion block to execute when the move operation finishes.

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

func stepByPresentationTime(CMTime, completionHandler: (CMTime, Bool, (any Error)?) -> Void)

Moves the cursor on the presentation timeline by the delta presentation time that you specify.

**Required**

func stepInPresentationOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in presentation order.

**Required**

