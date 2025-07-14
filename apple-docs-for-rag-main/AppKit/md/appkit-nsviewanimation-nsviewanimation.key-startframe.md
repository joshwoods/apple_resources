

- AppKit
- NSViewAnimation
- NSViewAnimation.Key
-  startFrame 

Type Property

# startFrame

The size and location of the window or view at the start of the animation.

macOS

``` source
static let startFrame: NSViewAnimation.Key
```

## Discussion

The size and location are specified by an NSRect structure encoded in an NSValue object. This property is optional. If it is not specified, `NSViewAnimation` uses the frame of the window or view at the start of the animation.

## See Also

### Keys

static let effect: NSViewAnimation.Key

An effect to apply to the animation.

static let endFrame: NSViewAnimation.Key

The size and location of the window or view at the end of the animation.

static let target: NSViewAnimation.Key

The target of the animation.

