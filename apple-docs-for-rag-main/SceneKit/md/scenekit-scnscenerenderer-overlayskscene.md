

- SceneKit
- SCNSceneRenderer
-  overlaySKScene 

Instance Property

# overlaySKScene

A Sprite Kit scene to be rendered on top of the SceneKit content.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var overlaySKScene: SKScene? { get set }
```

**Required**

## Discussion

Use this property to render 2D content that overlays your scene—for example, a heads-up-display for a game. The Sprite Kit scene shares the same underlying GPU resources as the SceneKit renderer, so using this property can provide much better performance than overlaying other views or layers above the view rendering your SceneKit content.

