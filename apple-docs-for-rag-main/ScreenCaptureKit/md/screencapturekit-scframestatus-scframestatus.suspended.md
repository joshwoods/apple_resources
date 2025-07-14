

- ScreenCaptureKit
- SCFrameStatus
-  SCFrameStatus.suspended 

Case

# SCFrameStatus.suspended

A status that indicates the system didn’t generate a new frame because you suspended updates.

Mac Catalyst 18.2+macOS 12.3+

``` source
case suspended
```

## See Also

### Status values

case complete

A status that indicates the system successfully generated a new frame.

case idle

A status that indicates the system didn’t generate a new frame because the display didn’t change.

case blank

A status that indicates the system didn’t generate a new frame because the display is blank.

case started

A status that indicates the frame is the first one sent after the stream starts.

case stopped

A status that indicates the frame is in a stopped state.

