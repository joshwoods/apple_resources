

- AppKit
- NSSavePanel
-  isExtensionHidden 

Instance Property

# isExtensionHidden

A Boolean value that indicates whether to display filename extensions.

macOS

``` source
@MainActor
var isExtensionHidden: Bool { get set }
```

## Discussion

When the value of this property is false, NSSavePanel shows the filename extension in places where you refer to the file by name. The user can override this value by checking the hide extension menu item, which reflects this value. The default value is true.

If a user adds or removes a filename extension in the panel’s name field, the panel updates this property to reflect that choice.

Note

Setting this property has no effect if the user has chosen to show all file extensions in Finder.

## See Also

### Configuring the Panel’s Behavior

var canCreateDirectories: Bool

A Boolean value that indicates whether the panel displays UI for creating directories.

var canSelectHiddenExtension: Bool

A Boolean value that indicates whether the panel displays UI for hiding or showing filename extensions.

var showsHiddenFiles: Bool

A Boolean value that indicates whether the panel displays files that are normally hidden from the user.

var isExpanded: Bool

A Boolean value that indicates whether whether the panel is expanded.

Button tags

Button tags that refer to items on the panel.

