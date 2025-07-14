

- AppKit
- NSSavePanel
-  canCreateDirectories 

Instance Property

# canCreateDirectories

A Boolean value that indicates whether the panel displays UI for creating directories.

macOS

``` source
@MainActor
var canCreateDirectories: Bool { get set }
```

## Discussion

When the value of this property is true, the panel includes UI to create new directories. When the value is false, the panel does not expose that UI.

## See Also

### Configuring the Panel’s Behavior

var canSelectHiddenExtension: Bool

A Boolean value that indicates whether the panel displays UI for hiding or showing filename extensions.

var showsHiddenFiles: Bool

A Boolean value that indicates whether the panel displays files that are normally hidden from the user.

var isExtensionHidden: Bool

A Boolean value that indicates whether to display filename extensions.

var isExpanded: Bool

A Boolean value that indicates whether whether the panel is expanded.

Button tags

Button tags that refer to items on the panel.

