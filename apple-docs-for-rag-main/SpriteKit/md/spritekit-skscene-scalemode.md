

- SpriteKit
- SKScene
-  scaleMode 

Instance Property

# scaleMode

A setting that defines how the scene is mapped to the view that presents it.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
var scaleMode: SKSceneScaleMode { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var scaleMode: SKSceneScaleMode { get set }
```

## Mentioned in 

Scaling a Scene’s Content to Fit the View

## Discussion

It is possible for a scene’s size to differ from the size of the view it is presented in. The scale mode determines how the visible portion of the scene is mapped to the view. The possible values are listed in SKSceneScaleMode. The default value is SKSceneScaleMode.fill.

## See Also

### Stretching Content to Fit the View

Scaling a Scene’s Content to Fit the View

Configure the scale mode to determine how a scene is sized to fit its view.

enum SKSceneScaleMode

The modes that determine how the scene’s area is mapped to the view that presents it.

