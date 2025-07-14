

- AppKit
- NSViewAnimation
- NSViewAnimation.Key
-  endFrame 

Type Property

# endFrame

The size and location of the window or view at the end of the animation.

macOS

``` source
static let endFrame: NSViewAnimation.Key
```

## Discussion

The size and location are specified by an NSRect structure encoded in an NSValue object. This property is optional. If it is not specified, `NSViewAnimation` uses the frame of the window or view at the start of the animation. If the target is a view and the end frame is empty, the view is hidden at the end.

## See Also

### Keys

static let effect: NSViewAnimation.Key

An effect to apply to the animation.

static let startFrame: NSViewAnimation.Key

The size and location of the window or view at the start of the animation.

static let target: NSViewAnimation.Key

The target of the animation.

