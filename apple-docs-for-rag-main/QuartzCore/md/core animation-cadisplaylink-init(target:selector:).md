

- Core Animation
- CADisplayLink
-  init(target:selector:) 

Initializer

# init(target:selector:)

Creates a display link for a target that calls its selector.

iOS 3.1+iPadOS 3.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
init(
    target: Any,
    selector sel: Selector
)
```

## Parameters 

`target`  

An object in your app that you want the system to notify each time it updates a display.

`sel`  

A selector instance that represents a method for `target`.

## Return Value

A new CADisplayLink object.

## Discussion

The selector on the target must be a method with the following signature, where sender is the display link returned by this method.

- Swift
- Objective-C

```
@objc func selector(sender: CADisplayLink)
```

```
- (void) selector:(CADisplayLink *)sender;
```

The newly constructed display link retains the target.

