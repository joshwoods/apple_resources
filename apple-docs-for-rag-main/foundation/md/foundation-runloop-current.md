

- Foundation
- RunLoop
-  current 

Type Property

# current

Returns the run loop for the current thread.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var current: RunLoop { get }
```

## Return Value

The `NSRunLoop` object for the current thread.

## Discussion

If a run loop does not yet exist for the thread, one is created and returned.

## See Also

### Related Documentation

Threading Programming Guide

### Accessing Run Loops and Modes

var currentMode: RunLoop.Mode?

The receiver’s current input mode.

func limitDate(forMode: RunLoop.Mode) -> Date?

Performs one pass through the run loop in the specified mode and returns the date at which the next timer is scheduled to fire.

class var main: RunLoop

Returns the run loop of the main thread.

func getCFRunLoop() -> CFRunLoop

Returns the receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

struct Mode

Modes that a run loop operates in.

