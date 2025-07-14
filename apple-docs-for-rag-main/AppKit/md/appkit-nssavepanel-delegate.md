

- AppKit
- NSSavePanel
-  delegate 

Instance Property

# delegate

A custom object you use to manage interactions with an open or save panel.

macOS

``` source
@MainActor
weak var delegate: (any NSOpenSavePanelDelegate)? { get set }
```

## See Also

### Responding to User Interactions

protocol NSOpenSavePanelDelegate

A set of methods for managing interactions with an open or save panel.

