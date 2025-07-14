

- Quartz
- IKImageBrowserView
-  setBackgroundLayer(\_:) 

Instance Method

# setBackgroundLayer(\_:)

The Core Animation layer used as the view’s background.

macOS 10.4+

``` source
@MainActor
func setBackgroundLayer(_ aLayer: CALayer!)
```

## Parameters 

`aLayer`  

A `CALayer` instance.

## Discussion

The background layer can have sublayers. Additionally, the layers can also contain animations.

The layer is optional.

## See Also

### Core Animation Layer Integration

func setForegroundLayer(CALayer!)

The Core Animation layer used as the foreground overlay.

func foregroundLayer() -> CALayer!

Returns the foreground Core Animation layer

func backgroundLayer() -> CALayer!

Returns the foreground Core Animation layer

