

- AppKit
- NSTableView
-  registeredNibsByIdentifier 

Instance Property

# registeredNibsByIdentifier

The dictionary of all registered nib files for view-based table view identifiers.

macOS 10.8+

``` source
@MainActor
var registeredNibsByIdentifier: [NSUserInterfaceItemIdentifier : NSNib]? { get }
```

## Discussion

Each key in the dictionary is the identifier string (given by NSUserInterfaceItemIdentifier) used to register the nib file in the register(_:forIdentifier:) method. The value of each key is the corresponding NSNib object.

Note

This method applies only to NSView-based table views.

## See Also

### NSView-Based Table Nib File Registration

func register(NSNib?, forIdentifier: NSUserInterfaceItemIdentifier)

Registers a NIB for the specified identifier, so that view-based table views can use it to instantiate views.

