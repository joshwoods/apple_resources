

- Core Animation
- CALayoutManager
-  layoutSublayers(of:) 

Instance Method

# layoutSublayers(of:)

Override to customize layout of sublayers whenever the layer needs redrawing.

Mac Catalyst 13.1+macOS 10.5+

``` source
optional func layoutSublayers(of layer: CALayer)
```

## See Also

### Managing Layout

func invalidateLayout(of: CALayer)

Invalidates the layout of a layer so it knows to refresh its content on the next frame.

func preferredSize(of: CALayer) -> CGSize

Override to customize layer size.

