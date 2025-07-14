

- MediaExtension
- MESampleCursor
-  estimatedSampleLocation() 

Instance Method

# estimatedSampleLocation()

Returns an estimate of the sample location indicated by the cursor.

macOS 14.0+

``` source
optional func estimatedSampleLocation() throws -> MEEstimatedSampleLocation
```

## Return Value

An object that provides information about the estimated sample location.

## Discussion

Some formats may need to read some data on a per-sample basis to produce the exact sample location. For these formats, it’s more efficient to read a larger chunk of data that contains both the data to produce the exact sample location and the actual sample data.

Note

If you implement this method, also implement refineSampleLocation(_:refinementData:refinementDataLength:refinedLocation:).

Pass the value this method returns to refineSampleLocation(_:refinementData:refinementDataLength:refinedLocation:) to obtain the exact sample location.

To indicate that refinement isn’t necessary, return a value for refinementDataLocation that has a zero length. If refinementDataLocation has a non-zero length, the range for the estimated sample location needs to fully cover the refined range that refineSampleLocation(_:refinementData:refinementDataLength:refinedLocation:) returns, and the refinement data location.

This method fails with the error MEError.Code.locationNotAvailable if the sample location indicated by the cursor isn’t contiguous or the method isn’t supported. In this case, use loadSampleBufferContainingSamples(to:completionHandler:) to load the sample data.

## See Also

### Stepping through samples

func samplesWithEarlierDTSsMayHaveLaterPTSs(than: any MESampleCursor) -> Bool

Tests for an earlier boundary in sample reordering.

func samplesWithLaterDTSsMayHaveEarlierPTSs(than: any MESampleCursor) -> Bool

Tests for a later boundary in sample reordering.

func refineSampleLocation(AVSampleCursorStorageRange, refinementData: UnsafePointer&lt;UInt8>, refinementDataLength: Int, refinedLocation: UnsafeMutablePointer&lt;AVSampleCursorStorageRange>) throws

Produces an exact sample location based on the estimated sample location and refinement data that you specify.

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

