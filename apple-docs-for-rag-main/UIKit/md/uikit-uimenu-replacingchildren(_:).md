

- UIKit
- UIMenu
-  replacingChildren(\_:) 

Instance Method

# replacingChildren(\_:)

Creates a new menu with the same configuration as the current menu, but with a new set of child elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func replacingChildren(_ newChildren: [UIMenuElement]) -> UIMenu
```

## Parameters 

`newChildren`  

The child elements to include in the new menu.

## Return Value

A new menu object containing the specified children.

## Discussion

The new menu contains the same title, image, identifier, and options as the current menu. The new menu contains only the children in the `newChildren` parameter. It doesn’t contain any child elements from the current menu.

## See Also

### Accessing child elements

var children: [UIMenuElement]

The contents of the menu.

