

- Compositor Services
- LayerRenderer
- LayerRenderer.Drawable
-  state 

Instance Property

# state

The current operational state of a drawable instance.

visionOS 1.0+

``` source
var state: LayerRenderer.Drawable.State { get }
```

## Discussion

A state value of LayerRenderer.Drawable.State.rendering indicates the drawable type is ready for you to draw your content. Other values indicate that Compositor Services currently owns the drawable.

Compositor Services reuses the underlying data structures associated with drawable types. The drawable’s state indicates whether it’s ready for you to draw to it. Run your drawing operations only when the drawable’s state is equal to LayerRenderer.Drawable.State.rendering.

## See Also

### Managing the state machine

enum State

The state of ownership for the drawable.

