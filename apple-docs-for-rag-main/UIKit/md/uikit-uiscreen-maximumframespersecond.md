

- UIKit
- UIScreen
-  maximumFramesPerSecond 

Instance Property

# maximumFramesPerSecond

The maximum number of frames per second a screen can render.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+tvOS 10.2+

``` source
@MainActor
var maximumFramesPerSecond: Int { get }
```

## Discussion

In iOS, the value of this property can be up to `120` for devices with ProMotion displays.

In tvOS, the value of this property depends on the hardware capabilities of the attached screen and the user’s selected resolution on Apple TV.

## See Also

### Getting a display link

func displayLink(withTarget: Any, selector: Selector) -> CADisplayLink?

Returns a display link object for the current screen.

