

- Foundation
- RunLoop
-  currentMode 

Instance Property

# currentMode

The receiver’s current input mode.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var currentMode: RunLoop.Mode? { get }
```

## Discussion

The receiver’s current input mode. This method returns the current input mode *only* while the receiver is running; otherwise, it returns `nil`.

The current mode is set by the methods that run the run loop, such as acceptInput(forMode:before:) and run(mode:before:).

## See Also

### Related Documentation

func run(until: Date)

Runs the loop until the specified date, during which time it processes data from all attached input sources.

func run()

Puts the receiver into a permanent loop, during which time it processes data from all attached input sources.

### Accessing Run Loops and Modes

class var current: RunLoop

Returns the run loop for the current thread.

func limitDate(forMode: RunLoop.Mode) -> Date?

Performs one pass through the run loop in the specified mode and returns the date at which the next timer is scheduled to fire.

class var main: RunLoop

Returns the run loop of the main thread.

func getCFRunLoop() -> CFRunLoop

Returns the receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

struct Mode

Modes that a run loop operates in.

