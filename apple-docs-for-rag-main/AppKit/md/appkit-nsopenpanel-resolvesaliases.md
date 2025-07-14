

- AppKit
- NSOpenPanel
-  resolvesAliases 

Instance Property

# resolvesAliases

A Boolean that indicates whether the panel resolves aliases.

macOS

``` source
@MainActor
var resolvesAliases: Bool { get set }
```

## Discussion

When the value of this property is true, dropping an alias on the panel or asking for filenames or URLs returns the resolved aliases. The default value of this property is true. When this value is false, selecting an alias returns the alias instead of the file or directory it represents.

## See Also

### Configuring the Open Panel

var canChooseFiles: Bool

A Boolean that indicates whether the user can choose files in the panel.

var canChooseDirectories: Bool

A Boolean that indicates whether the user can choose directories in the panel.

var allowsMultipleSelection: Bool

A Boolean that indicates whether the user may select multiple files and directories.

var isAccessoryViewDisclosed: Bool

A Boolean value that indicates whether the panel’s accessory view is visible.

