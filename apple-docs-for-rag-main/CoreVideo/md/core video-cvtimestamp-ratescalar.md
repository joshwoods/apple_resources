

- Core Video
- CVTimeStamp
-  rateScalar 

Instance Property

# rateScalar

The current rate of the device as measured by the timestamps, divided by the nominal rate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var rateScalar: Double
```

## See Also

### Properties

var flags: UInt64

A bit field containing additional information about the timestamp.

var hostTime: UInt64

The system time measured by the timestamp.

var reserved: UInt64

Reserved. Do not use.

var smpteTime: CVSMPTETime

The SMPTE time representation of the timestamp.

var version: UInt32

The current `CVTimeStamp` structure is version 0. Some functions require you to specify a version when passing in a timestamp structure to be filled.

var videoRefreshPeriod: Int64

var videoTime: Int64

The start of a frame (or field for interlaced video).

var videoTimeScale: Int32

The scale (in units per second) of the `videoTimeScale` and `videoRefreshPeriod` fields.

