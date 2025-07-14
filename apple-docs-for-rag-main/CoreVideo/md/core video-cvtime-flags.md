

- Core Video
- CVTime
-  flags 

Instance Property

# flags

The flags associated with the `CVTime` value. See CVTime Values for possible values. If `kCVTimeIsIndefinite` is set, you should not use any of the other fields in this structure.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var flags: Int32
```

## See Also

### Properties

var timeScale: Int32

The time scale for this value.

var timeValue: Int64

The time value.

