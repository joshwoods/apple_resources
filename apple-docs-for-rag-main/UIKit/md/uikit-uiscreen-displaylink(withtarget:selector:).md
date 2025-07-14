

- UIKit
- UIScreen
-  displayLink(withTarget:selector:) 

Instance Method

# displayLink(withTarget:selector:)

Returns a display link object for the current screen.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
func displayLink(
    withTarget target: Any,
    selector sel: Selector
) -> CADisplayLink?
```

## Parameters 

`target`  

An object to be notified when the screen should be updated.

`sel`  

The method of `target` to call. This selector must have the following signature:

```
- (void)selector:(CADisplayLink *)sender;
```

## Return Value

A newly constructed display link object.

## Discussion

You use display link objects to synchronize your drawing code to the screen’s refresh rate. The newly constructed display link retains the target.

## See Also

### Getting a display link

var maximumFramesPerSecond: Int

The maximum number of frames per second a screen can render.

