

- Core Video
- CVTime
-  timeScale 

Instance Property

# timeScale

The time scale for this value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var timeScale: Int32
```

## See Also

### Properties

var flags: Int32

The flags associated with the `CVTime` value. See CVTime Values for possible values. If `kCVTimeIsIndefinite` is set, you should not use any of the other fields in this structure.

var timeValue: Int64

The time value.

