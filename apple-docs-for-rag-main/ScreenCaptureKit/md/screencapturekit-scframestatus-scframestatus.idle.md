

- ScreenCaptureKit
- SCFrameStatus
-  SCFrameStatus.idle 

Case

# SCFrameStatus.idle

A status that indicates the system didn’t generate a new frame because the display didn’t change.

Mac Catalyst 18.2+macOS 12.3+

``` source
case idle
```

## See Also

### Status values

case complete

A status that indicates the system successfully generated a new frame.

case blank

A status that indicates the system didn’t generate a new frame because the display is blank.

case started

A status that indicates the frame is the first one sent after the stream starts.

case suspended

A status that indicates the system didn’t generate a new frame because you suspended updates.

case stopped

A status that indicates the frame is in a stopped state.

