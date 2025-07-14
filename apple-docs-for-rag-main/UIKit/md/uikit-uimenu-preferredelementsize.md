

- UIKit
- UIMenu
-  preferredElementSize 

Instance Property

# preferredElementSize

The size of the menu’s child elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var preferredElementSize: UIMenu.ElementSize { get set }
```

## Discussion

This property allows you to choose between different layouts in the context menu:

- The UIMenu.ElementSize.small size gives the menu a more compact, side-by-side appearance, allowing you to fit more actions in a single row.

- The UIMenu.ElementSize.medium size gives the menu the side-by-side appearance, but shows additional detail for each action. The text-editing menu uses this element size to display the standard edit menu.

- The UIMenu.ElementSize.large size gives the menu its default, full-width appearance.

If you specify the UIMenu.ElementSize.small or UIMenu.ElementSize.medium sizes, the menu displays any items beyond the first three (for medium) or four (for small) as full-size elements.

This property doesn’t have an effect if you build your app with Mac Catalyst.

Related Sessions from WWDC22

Session 10071: Adopt desktop-class editing interactions

## See Also

### Specifying size of menu elements

enum ElementSize

Constants that determine the size of an element in a menu.

