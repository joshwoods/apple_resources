

- MediaExtension
- MESampleCursor
-  samplesWithLaterDTSsMayHaveEarlierPTSs(than:) 

Instance Method

# samplesWithLaterDTSsMayHaveEarlierPTSs(than:)

Tests for a later boundary in sample reordering.

macOS 14.0+

``` source
optional func samplesWithLaterDTSsMayHaveEarlierPTSs(than cursor: any MESampleCursor) -> Bool
```

## Parameters 

`cursor`  

A sample cursor to use to test the sample reordering boundary.

## Return Value

true if it’s possible that later samples in decode order can have an earlier presentation timestamp than that of the specified cursor; otherwise false.

## Discussion

This method tests for a boundary in the reordering from decode order to presentation order. This determines when it’s possible for any sample later in decode order than the current sample to have an earllier presentation time than the current sample of the specified cursor. You can use this test to limit backward scans, such as to start forward playback. For example, with the argument cursor fixed, step the cursor forward until it’s impossible for any later-in-decode-order samples to be earlier-in-presentation-order than the argument cursor sample.

Don’t implement this method for formats where sample reordering doesn’t make sense for the track content, which also indicates that the samples aren’t reordered.

Important

Only pass a cursor to this method that references the same sequence of samples as the cursor you call this method on, such as that the same instance of METrackReader created. Otherwise, the result is undefined.

## See Also

### Stepping through samples

func samplesWithEarlierDTSsMayHaveLaterPTSs(than: any MESampleCursor) -> Bool

Tests for an earlier boundary in sample reordering.

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

func stepInDecodeOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in decode order.

**Required**

func stepInPresentationOrder(by: Int64, completionHandler: (Int64, (any Error)?) -> Void)

Moves the cursor a given number of samples in presentation order.

**Required**

