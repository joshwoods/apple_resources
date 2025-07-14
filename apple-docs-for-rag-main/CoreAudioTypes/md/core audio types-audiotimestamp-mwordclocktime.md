

- Core Audio Types
- AudioTimeStamp
-  mWordClockTime 

Instance Property

# mWordClockTime

The word clock time.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mWordClockTime: UInt64
```

## See Also

### Accessing the Data

var mFlags: AudioTimeStampFlags

A set of flags indicating which representations of the time are valid; see `Audio Time Stamp Flags` and `Audio Time Stamp Flag Combination Constant`.

var mHostTime: UInt64

The host machine’s time base (see `CoreAudio/HostTime.h`).

var mRateScalar: Float64

The ratio of actual host ticks per sample frame to the nominal host ticks per sample frame.

var mReserved: UInt32

Pads the structure out to force an even 8-byte alignment.

var mSMPTETime: SMPTETime

The SMPTE time (see SMPTETime).

var mSampleTime: Float64

The absolute sample frame time.

