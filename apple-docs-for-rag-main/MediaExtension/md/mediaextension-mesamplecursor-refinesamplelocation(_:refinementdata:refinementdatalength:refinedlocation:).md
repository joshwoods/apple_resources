

- MediaExtension
- MESampleCursor
-  refineSampleLocation(\_:refinementData:refinementDataLength:refinedLocation:) 

Instance Method

# refineSampleLocation(\_:refinementData:refinementDataLength:refinedLocation:)

Produces an exact sample location based on the estimated sample location and refinement data that you specify.

macOS 14.0+

``` source
optional func refineSampleLocation(
    _ estimatedSampleLocation: AVSampleCursorStorageRange,
    refinementData: UnsafePointer,
    refinementDataLength: Int,
    refinedLocation refinedLocationOut: UnsafeMutablePointer
) throws
```

## Parameters 

`estimatedSampleLocation`  

The estimated sample location.

`refinementData`  

The refinement data.

`refinementDataLength`  

The length of the refinement data in bytes.

`refinedLocationOut`  

The starting file offset and size of the sample in bytes.

## Discussion

Use estimatedSampleLocation() to obtain the estimated sample location to pass to this method.

## See Also

### Stepping through samples

func samplesWithEarlierDTSsMayHaveLaterPTSs(than: any MESampleCursor) -> Bool

Tests for an earlier boundary in sample reordering.

func samplesWithLaterDTSsMayHaveEarlierPTSs(than: any MESampleCursor) -> Bool

Tests for a later boundary in sample reordering.

func estimatedSampleLocation() throws -> MEEstimatedSampleLocation

Returns an estimate of the sample location indicated by the cursor.

func stepByDecodeTime(CMTime, completionHandler: (CMTime, Bool, (any Error)?) -> Void)

Moves the cursor on the decode timeline by the delta decode time that you specify.

**Required**

func stepByPresentationTime(CMTime, completionHandler: (CMTime, Bool, (any Error)?) -> Void)

Moves the cursor on the presentation timeline by the delta presentation time that you specify.

**Required**

func stepInDecodeOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in decode order.

**Required**

func stepInPresentationOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in presentation order.

**Required**

