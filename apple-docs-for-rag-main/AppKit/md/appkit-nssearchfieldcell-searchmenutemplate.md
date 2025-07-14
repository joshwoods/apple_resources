

- AppKit
- NSSearchFieldCell
-  searchMenuTemplate 

Instance Property

# searchMenuTemplate

The menu object used to dynamically construct the search field’s pop-up icon menu.

macOS

``` source
@MainActor
var searchMenuTemplate: NSMenu? { get set }
```

## Discussion

The cell looks for the tag constants described in Menu tags to determine how to populate the menu with items related to recent searches. For an example of how you might set up the search menu template, see Configuring a Search Menu.

