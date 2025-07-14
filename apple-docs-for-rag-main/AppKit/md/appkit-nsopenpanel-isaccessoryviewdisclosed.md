

- AppKit
- NSOpenPanel
-  isAccessoryViewDisclosed 

Instance Property

# isAccessoryViewDisclosed

A Boolean value that indicates whether the panel’s accessory view is visible.

macOS 10.11+

``` source
@MainActor
var isAccessoryViewDisclosed: Bool { get set }
```

## Discussion

The value of this property is true when the accessory view is visible, and false when it isn’t. Setting the value of this property programmatically changes the visibility of the accessory panel. If no accessory panel is present, setting this property does nothing.

## See Also

### Configuring the Open Panel

var canChooseFiles: Bool

A Boolean that indicates whether the user can choose files in the panel.

var canChooseDirectories: Bool

A Boolean that indicates whether the user can choose directories in the panel.

var resolvesAliases: Bool

A Boolean that indicates whether the panel resolves aliases.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user may select multiple files and directories.

