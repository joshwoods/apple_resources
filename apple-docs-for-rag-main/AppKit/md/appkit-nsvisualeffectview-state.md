

- AppKit
- NSVisualEffectView
-  state 

Instance Property

# state

A value that indicates whether a view has a visual effect applied.

macOS 10.10+

``` source
@MainActor
var state: NSVisualEffectView.State { get set }
```

## Discussion

The default value of this property is NSVisualEffectView.State.followsWindowActiveState.

## See Also

### Enabling or Disabling the Effect

enum State

Constants to specify how the material appearance should reflect window activity state.

