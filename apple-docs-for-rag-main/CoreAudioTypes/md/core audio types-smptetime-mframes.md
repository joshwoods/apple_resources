

- Core Audio Types
- SMPTETime
-  mFrames 

Instance Property

# mFrames

The value of the frames portion of the SMPTE time.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mFrames: Int16
```

## See Also

### Instance Properties

var mCounter: UInt32

The total number of messages received. It takes 8 messages to carry a full SMPTE time code.

var mFlags: SMPTETimeFlags

A set of flags that indicate the SMPTE state (see `SMPTE Time Flags`).

var mHours: Int16

The value of the hours portion of the SMPTE time.

var mMinutes: Int16

The value of the minutes portion of the SMPTE time.

var mSeconds: Int16

The value of the seconds portion of the SMPTE time.

var mSubframeDivisor: Int16

The number of subframes per video frame (typically 80).

var mSubframes: Int16

A subframe offset to the HH:MM:SS:FF time. You can use this field to position a time marker somewhere within the time span represented by a video frame, if necessary.

var mType: SMPTETimeType

A SMPTE time type constant indicating the kind of SMPTE time used (see `SMPTE Timecode Types`).

