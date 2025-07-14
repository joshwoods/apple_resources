

- Core Video
- CVTime
-  timeValue 

Instance Property

# timeValue

The time value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
var timeValue: Int64
```

## See Also

### Properties

var flags: Int32

The flags associated with the `CVTime` value. See CVTime Values for possible values. If `kCVTimeIsIndefinite` is set, you should not use any of the other fields in this structure.

var timeScale: Int32

The time scale for this value.

