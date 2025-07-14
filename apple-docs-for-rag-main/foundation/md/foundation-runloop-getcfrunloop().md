

- Foundation
- RunLoop
-  getCFRunLoop() 

Instance Method

# getCFRunLoop()

Returns the receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getCFRunLoop() -> CFRunLoop
```

## Return Value

The receiver’s underlying doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht object.

## Discussion

You can use the returned run loop to configure the current run loop using Core Foundation function calls. For example, you might use this function to set up a run loop observer.

## See Also

### Accessing Run Loops and Modes

class var current: RunLoop

Returns the run loop for the current thread.

var currentMode: RunLoop.Mode?

The receiver’s current input mode.

func limitDate(forMode: RunLoop.Mode) -> Date?

Performs one pass through the run loop in the specified mode and returns the date at which the next timer is scheduled to fire.

class var main: RunLoop

Returns the run loop of the main thread.

struct Mode

Modes that a run loop operates in.

