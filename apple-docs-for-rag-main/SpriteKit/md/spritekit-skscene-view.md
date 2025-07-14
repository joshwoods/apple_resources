

- SpriteKit
- SKScene
-  view 

Instance Property

# view

The view that is currently presenting the scene.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
weak var view: SKView? { get }
```

## Discussion

To present a scene, you call the presentScene(_:) method or presentScene(_:transition:) method on the SKView class. If the scene is not currently presented, this property holds `nil`.

## See Also

### Setting the Background Appearance

Creating a Scene with a Transparent Background

Set a transparent background color to show the content of the views below.

var backgroundColor: UIColor

The background color of the scene.

