

- SwiftUI
- ImmersionStyle
-  mixed 

Type Property

# mixed

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

visionOS 1.0+

``` source
static var mixed: MixedImmersionStyle { get }
```

Available when `Self` is `MixedImmersionStyle`.

## Discussion

When this immersion style is selected, the immersion amount reported by the closure of `View/onImmersionChange(_:)` is `0.0`.

Use the immersionStyle(selection:in:) scene modifier to specify this style for an ImmersiveSpace. However, this is the default immersion style if you don’t specify one.

The immersion style affects how windows interact with virtual objects in the environment. In `mixed` immersion, a virtual object obscures part or all of a window that’s behind the object. Similarly, a window obscures a virtual object that’s behind the window.

## See Also

### Getting built-in styles

static var automatic: AutomaticImmersionStyle

The default immersion style.

static var full: FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

static var progressive: ProgressiveImmersionStyle

An immersion style that displays unbounded content that partially replaces passthrough video.

