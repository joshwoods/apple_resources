

- Foundation
- RunLoop
-  main 

Type Property

# main

Returns the run loop of the main thread.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var main: RunLoop { get }
```

## Return Value

An object representing the main thread’s run loop.

## See Also

### Accessing Run Loops and Modes

class var current: RunLoop

Returns the run loop for the current thread.

var currentMode: RunLoop.Mode?

The receiver’s current input mode.

func limitDate(forMode: RunLoop.Mode) -> Date?

Performs one pass through the run loop in the specified mode and returns the date at which the next timer is scheduled to fire.

func getCFRunLoop() -> CFRunLoop

Returns the receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

struct Mode

Modes that a run loop operates in.

