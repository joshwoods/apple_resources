

- AppKit
- NSSplitView
-  autosaveName 

Instance Property

# autosaveName

The name to use when the system automatically saves the split view’s divider configuration.

macOS 10.5+

``` source
@MainActor
var autosaveName: NSSplitView.AutosaveName? { get set }
```

## Discussion

If this property’s value is `nil` or empty, autosaving doesn’t occur.

## See Also

### Saving Subview Positions

typealias AutosaveName

The type that specifies the split view’s autosave name.

