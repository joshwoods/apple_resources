

- Foundation
- RunLoop
-  limitDate(forMode:) 

Instance Method

# limitDate(forMode:)

Performs one pass through the run loop in the specified mode and returns the date at which the next timer is scheduled to fire.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func limitDate(forMode mode: RunLoop.Mode) -> Date?
```

## Parameters 

`mode`  

The run loop mode to search. You may specify custom modes or use one of the modes listed in `Run Loop Modes`.

## Return Value

The date at which the next timer is scheduled to fire, or `nil` if there are no input sources for this mode.

## Discussion

The run loop is entered with an immediate timeout, so the run loop does not block, waiting for input, if no input sources need processing.

## See Also

### Accessing Run Loops and Modes

class var current: RunLoop

Returns the run loop for the current thread.

var currentMode: RunLoop.Mode?

The receiver’s current input mode.

class var main: RunLoop

Returns the run loop of the main thread.

func getCFRunLoop() -> CFRunLoop

Returns the receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

struct Mode

Modes that a run loop operates in.

