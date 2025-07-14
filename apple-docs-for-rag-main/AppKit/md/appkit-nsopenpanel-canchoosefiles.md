

- AppKit
- NSOpenPanel
-  canChooseFiles 

Instance Property

# canChooseFiles

A Boolean that indicates whether the user can choose files in the panel.

macOS

``` source
@MainActor
var canChooseFiles: Bool { get set }
```

## Discussion

When the value of this property is true, users can choose files in the panel.

## See Also

### Configuring the Open Panel

var canChooseDirectories: Bool

A Boolean that indicates whether the user can choose directories in the panel.

var resolvesAliases: Bool

A Boolean that indicates whether the panel resolves aliases.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user may select multiple files and directories.

var isAccessoryViewDisclosed: Bool

A Boolean value that indicates whether the panel’s accessory view is visible.

