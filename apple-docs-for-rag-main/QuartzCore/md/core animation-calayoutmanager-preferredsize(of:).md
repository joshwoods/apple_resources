

- Core Animation
- CALayoutManager
-  preferredSize(of:) 

Instance Method

# preferredSize(of:)

Override to customize layer size.

Mac Catalyst 13.1+macOS 10.5+

``` source
optional func preferredSize(of layer: CALayer) -> CGSize
```

## See Also

### Managing Layout

func invalidateLayout(of: CALayer)

Invalidates the layout of a layer so it knows to refresh its content on the next frame.

func layoutSublayers(of: CALayer)

Override to customize layout of sublayers whenever the layer needs redrawing.

