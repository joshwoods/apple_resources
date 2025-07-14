

- AppKit
- NSOpenPanel
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

A Boolean that indicates whether the user may select multiple files and directories.

macOS

``` source
@MainActor
var allowsMultipleSelection: Bool { get set }
```

## Discussion

When the value of this property is true, the user may select multiple items from the browser. When the selection contains multiple items, use the urls property to retrieve those items instead of the inherited url property.

## See Also

### Configuring the Open Panel

var canChooseFiles: Bool

A Boolean that indicates whether the user can choose files in the panel.

var canChooseDirectories: Bool

A Boolean that indicates whether the user can choose directories in the panel.

var resolvesAliases: Bool

A Boolean that indicates whether the panel resolves aliases.

var isAccessoryViewDisclosed: Bool

A Boolean value that indicates whether the panel’s accessory view is visible.

