

- Quartz
- IKImageBrowserView
-  setForegroundLayer(\_:) 

Instance Method

# setForegroundLayer(\_:)

The Core Animation layer used as the foreground overlay.

macOS 10.4+

``` source
@MainActor
func setForegroundLayer(_ aLayer: CALayer!)
```

## Parameters 

`aLayer`  

A `CALayer` instance.

## Discussion

The foreground overlay layer can have sublayers. Additionally, the layers can also contain animations.

The foreground layer is an overlay that is applied to the view. It can be used to provide information such as loading progress or for pure cosmetic purposes, such as dark gradients on top and bottom of the browser view.

This layer is optional.

## See Also

### Core Animation Layer Integration

func foregroundLayer() -> CALayer!

Returns the foreground Core Animation layer

func setBackgroundLayer(CALayer!)

The Core Animation layer used as the view’s background.

func backgroundLayer() -> CALayer!

Returns the foreground Core Animation layer

