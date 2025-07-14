

- AppKit
- NSSavePanel
-  showsHiddenFiles 

Instance Property

# showsHiddenFiles

A Boolean value that indicates whether the panel displays files that are normally hidden from the user.

macOS

``` source
@MainActor
var showsHiddenFiles: Bool { get set }
```

## Discussion

When the value of this property is true, the panel displays hidden files; if false, it does not. The default value is false.

## See Also

### Configuring the Panel’s Behavior

var canCreateDirectories: Bool

A Boolean value that indicates whether the panel displays UI for creating directories.

var canSelectHiddenExtension: Bool

A Boolean value that indicates whether the panel displays UI for hiding or showing filename extensions.

var isExtensionHidden: Bool

A Boolean value that indicates whether to display filename extensions.

var isExpanded: Bool

A Boolean value that indicates whether whether the panel is expanded.

Button tags

Button tags that refer to items on the panel.

