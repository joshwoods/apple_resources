

- AppKit
- NSMenuItem
-  view 

Instance Property

# view

The content view for the menu item.

macOS 10.5+

``` source
var view: NSView? { get set }
```

## Discussion

A menu item with a view does not draw its title, state, font, or other standard drawing attributes, and assigns drawing responsibility entirely to the view. Keyboard equivalents and type-select continue to use the key equivalent and title as normal. For more details, see Application Menu and Pop-up List Programming Topics

By default, a menu item has a `nil` view.

