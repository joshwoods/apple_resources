

- Core Animation
- CALayoutManager
-  invalidateLayout(of:) 

Instance Method

# invalidateLayout(of:)

Invalidates the layout of a layer so it knows to refresh its content on the next frame.

Mac Catalyst 13.1+macOS 10.5+

``` source
optional func invalidateLayout(of layer: CALayer)
```

## See Also

### Managing Layout

func layoutSublayers(of: CALayer)

Override to customize layout of sublayers whenever the layer needs redrawing.

func preferredSize(of: CALayer) -> CGSize

Override to customize layer size.

