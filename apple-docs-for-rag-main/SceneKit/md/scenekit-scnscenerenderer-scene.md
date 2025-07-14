

- SceneKit
- SCNSceneRenderer
-  scene 

Instance Property

# scene

The scene to be displayed.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var scene: SCNScene? { get set }
```

**Required**

## Discussion

Setting a new scene immediately replaces whatever scene the renderer was previously displaying. To display a transition between scenes, use the present(_:with:incomingPointOfView:completionHandler:) method.

## See Also

### Presenting a Scene

func present(SCNScene, with: SKTransition, incomingPointOfView: SCNNode?, completionHandler: (() -> Void)?)

Displays the specified scene with an animated transition.

**Required**

