

- Core Video
- CVTimeStampFlags
-  videoTimeValid 

Type Property

# videoTimeValid

The value in the video time field is valid.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
static var videoTimeValid: CVTimeStampFlags { get }
```

## See Also

### Constants

static var bottomField: CVTimeStampFlags

The timestamp represents the bottom lines of an interlaced image.

static var hostTimeValid: CVTimeStampFlags

The value in the host time field is valid.

static var isInterlaced: CVTimeStampFlags

A convenience constant indicating that the timestamp is for an interlaced image.

static var rateScalarValid: CVTimeStampFlags

The value in the rate scalar field is valid.

static var smpteTimeValid: CVTimeStampFlags

The value in the SMPTE time field is valid.

static var topField: CVTimeStampFlags

The timestamp represents the top lines of an interlaced image.

static var videoHostTimeValid: CVTimeStampFlags

A convenience constant indicating that both the video time and host time fields are valid.

static var videoRefreshPeriodValid: CVTimeStampFlags

The value in the video refresh period field is valid.

