

- SpriteKit
- SKScene
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var backgroundColor: UIColor { get set }
```

**macOS**

``` source
@MainActor
var backgroundColor: NSColor { get set }
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var backgroundColor: UIColor { get set }
```

## Mentioned in 

Creating a Scene with a Transparent Background

## Discussion

The default value is a gray color (RGBA `0.15, 0.15, 0.15, 1.0)`.

## See Also

### Setting the Background Appearance

Creating a Scene with a Transparent Background

Set a transparent background color to show the content of the views below.

var view: SKView?

The view that is currently presenting the scene.

