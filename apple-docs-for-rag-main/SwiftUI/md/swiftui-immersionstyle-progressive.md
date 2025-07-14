

- SwiftUI
- ImmersionStyle
-  progressive 

Type Property

# progressive

An immersion style that displays unbounded content that partially replaces passthrough video.

visionOS 1.0+

``` source
static var progressive: ProgressiveImmersionStyle { get }
```

Available when `Self` is `ProgressiveImmersionStyle`.

## Discussion

The system initially uses a radial portal effect that replaces passthrough in a portion of the field of view. People can interactively adjust the size of the portal by turning the Digital Crown, including down to a minimum amount of immersion defined by the system and up to the point where the portal fully covers passthrough. If someone tries to reduce the portal size below the minimum value, the portal smoothly bounces back to the minimum size. The portal’s behavior at the maximum size matches the behavior of the full immersion style, including the configurable visibility of the viewer’s upper limbs.

When this immersion style is selected, the immersion amount reported by the closure of `View/onImmersionChange(_:)` is within the range of the immersion that this style uses.

Use the immersionStyle(selection:in:) scene modifier to specify this style for an ImmersiveSpace:

```
@main
struct ImmersiveApp: App {
    @State private var immersionStyle: ImmersionStyle = .progressive
    var body: some Scene {
        ImmersiveSpace { ... }
        .immersionStyle(selection: $immersionStyle, in: .progressive))
    }
}
```

The immersion style affects how windows interact with virtual objects in the environment. In `progressive` immersion, windows always render in front of virtual content, no matter how someone positions the window or the content. This helps people avoid losing track of windows behind virtual content when passthrough is off.

## See Also

### Getting built-in styles

static var automatic: AutomaticImmersionStyle

The default immersion style.

static var full: FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

static var mixed: MixedImmersionStyle

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

