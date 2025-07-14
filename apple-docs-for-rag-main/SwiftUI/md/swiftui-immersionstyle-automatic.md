

- SwiftUI
- ImmersionStyle
-  automatic 

Type Property

# automatic

The default immersion style.

visionOS 1.0+

``` source
static var automatic: AutomaticImmersionStyle { get }
```

Available when `Self` is `AutomaticImmersionStyle`.

## Discussion

The system uses this style for an ImmersiveSpace if you don’t provide an immersionStyle(selection:in:) scene modifier. You don’t typically specify the `automatic` style explicitly.

By default, the system uses the mixed immersion style as the `automatic` style.

## See Also

### Getting built-in styles

static var full: FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

static var mixed: MixedImmersionStyle

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

static var progressive: ProgressiveImmersionStyle

An immersion style that displays unbounded content that partially replaces passthrough video.

