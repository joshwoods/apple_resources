

- AppKit
- NSPopUpButton
-  preferredEdge 

Instance Property

# preferredEdge

The edge of the button on which to display the menu when screen space is constrained.

macOS

``` source
@MainActor
var preferredEdge: NSRectEdge { get set }
```

## Discussion

Possible values include NSMinXEdge, NSMinYEdge, NSMaxXEdge, or NSMaxYEdge. For pull-down menus, the default behavior is to position the menu under the button. The bottom edge corresponds to the value `NSMaxYEdge` for flipped views or `NSMinYEdge` for unflipped views. For most pop-up menus, the `NSPopUpButton` object attempts to show the selected item directly over the button.

