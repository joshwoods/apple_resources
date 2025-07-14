

- AppKit
- NSGestureRecognizer
-  init(target:action:) 

Initializer

# init(target:action:)

Initializes the gesture recognizer with the specified target and action information.

macOS 10.10+

``` source
@MainActor
init(
    target: Any?,
    action: Selector?
)
```

## Parameters 

`target`  

The object whose action method is called when the gesture is recognized. You must not specify `nil` for this parameter.

`action`  

A selector that identifies the method to call when the gesture is recognized. This method must be implemented by the object in `target`. You must not specify `nil` for this parameter.

## Return Value

The initialized gesture recognizer object or `nil` if an error occurred.

## Discussion

This method is the designated initializer. Subclasses must call this method from their own custom initialization methods. Call the method before performing other tasks.

This method records the specified `target` and `action` values and prepares the gesture recognizer for use.

The `action` method must have one of the following signatures:

- Swift
- Objective-C

```
func handleGesture() { }
func handleGesture(gestureRecognizer: NSGestureRecognizer) { }
```

```
- (void)handleGesture;
- (void)handleGesture:(NSGestureRecognizer *)gestureRecognizer;
```

## See Also

### Related Documentation

var target: AnyObject?

The object that implements the action method.

Cocoa Event Handling Guide

var action: Selector?

The action method to call when the gesture is recognized.

