

- AppKit
- NSApplication
-  detachDrawingThread(\_:toTarget:with:) 

Type Method

# detachDrawingThread(\_:toTarget:with:)

Creates and executes a new thread based on the specified target and selector.

macOS

``` source
@MainActor
class func detachDrawingThread(
    _ selector: Selector,
    toTarget target: Any,
    with argument: Any?
)
```

## Parameters 

`selector`  

The selector whose code you want to execute in the new thread.

`target`  

The object that defines the specified selector.

`argument`  

An optional argument you want to pass to the selector.

## Discussion

This method is a convenience wrapper for the detachNewThreadSelector(_:toTarget:with:) method of Thread. This method automatically creates an `@autoreleasepool` block for the new thread before invoking `selector`.

