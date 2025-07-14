

- AppKit
- NSSavePanel
-  canSelectHiddenExtension 

Instance Property

# canSelectHiddenExtension

A Boolean value that indicates whether the panel displays UI for hiding or showing filename extensions.

macOS

``` source
@MainActor
var canSelectHiddenExtension: Bool { get set }
```

## Discussion

Set the value of this property before displaying the panel. When the value of this property is true, and the Finder preference “Show all extensions” is false, the panel displays the Hide Extension menu item. The default value of this property is false.

Use the isExtensionHidden property to hide or shows extensions.

## See Also

### Configuring the Panel’s Behavior

var canCreateDirectories: Bool

A Boolean value that indicates whether the panel displays UI for creating directories.

var showsHiddenFiles: Bool

A Boolean value that indicates whether the panel displays files that are normally hidden from the user.

var isExtensionHidden: Bool

A Boolean value that indicates whether to display filename extensions.

var isExpanded: Bool

A Boolean value that indicates whether whether the panel is expanded.

Button tags

Button tags that refer to items on the panel.

