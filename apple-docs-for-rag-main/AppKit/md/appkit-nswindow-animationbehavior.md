

- AppKit
- NSWindow
-  animationBehavior 

Instance Property

# animationBehavior

The window’s automatic animation behavior.

macOS 10.7+

``` source
@MainActor
var animationBehavior: NSWindow.AnimationBehavior { get set }
```

## Discussion

This property controls the automatic window animation behavior used when the orderFront(_:) or orderOut(_:) methods are called. See NSWindow.AnimationBehavior for the possible values of this property.

By default, a window’s animation behavior is set to NSWindow.AnimationBehavior.default, which causes AppKit to determine the style of animation to use automatically based on its inference of a window’s “type” from various window properties. A window’s animation behavior can be set to NSWindow.AnimationBehavior.none to disable AppKit’s automatic animations for the window, which may be useful if that animation interferes with an animation that your application implements.

The animation behavior can also be set to one of the other non-default NSWindow.AnimationBehavior values to override AppKit’s automatic inference of appropriate animation behavior based on the window’s apparent type, although this is not recommended.

