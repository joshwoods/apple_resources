

- UIKit
- UIMenu
-  children 

Instance Property

# children

The contents of the menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var children: [UIMenuElement] { get }
```

## Discussion

If the menu doesn’t have any child menu elements, this property contains an empty array.

## See Also

### Accessing child elements

func replacingChildren([UIMenuElement]) -> UIMenu

Creates a new menu with the same configuration as the current menu, but with a new set of child elements.

