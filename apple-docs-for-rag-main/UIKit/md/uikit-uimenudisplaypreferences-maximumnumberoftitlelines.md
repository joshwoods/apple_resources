

- UIKit
- UIMenuDisplayPreferences
-  maximumNumberOfTitleLines 

Instance Property

# maximumNumberOfTitleLines

The number of lines the menu displays for an item’s title or subtitle before it truncates the text.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
var maximumNumberOfTitleLines: Int { get set }
```

## Discussion

By default, UIMenu restricts the number of lines in a menu item’s title or subtitle to create a balance between a compact and expressive display. If you dynamically prepare menu items that might contain more text, set this value to a higher number and use this object as the menu’s displayPreferences.

Note

Setting this property has no effect on menus in Mac Catalyst apps.

