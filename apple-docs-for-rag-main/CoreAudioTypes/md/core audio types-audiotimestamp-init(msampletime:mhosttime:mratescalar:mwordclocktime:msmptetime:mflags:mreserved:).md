

- Core Audio Types
- AudioTimeStamp
-  init(mSampleTime:mHostTime:mRateScalar:mWordClockTime:mSMPTETime:mFlags:mReserved:) 

Initializer

# init(mSampleTime:mHostTime:mRateScalar:mWordClockTime:mSMPTETime:mFlags:mReserved:)

Creates an audio time stamp.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mSampleTime: Float64,
    mHostTime: UInt64,
    mRateScalar: Float64,
    mWordClockTime: UInt64,
    mSMPTETime: SMPTETime,
    mFlags: AudioTimeStampFlags,
    mReserved: UInt32
)
```

## See Also

### Initializers

init()

Creates an empty audio timestamp.

