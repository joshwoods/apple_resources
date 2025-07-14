

- UIKit
- UIMenuBuilder
-  menu(for:) 

Instance Method

# menu(for:)

Gets the menu for the specified menu identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func menu(for identifier: UIMenu.Identifier) -> UIMenu?
```

**Required**

## Parameters 

`identifier`  

The identifier of the menu to retrieve.

## Return Value

A menu object; otherwise, `nil` if there are no menus with the specified identifier.

## See Also

### Getting menu systems and elements

var system: UIMenuSystem

The menu system that the menu builder modifies.

**Required**

func action(for: UIAction.Identifier) -> UIAction?

Gets the action for the specified action identifier.

**Required**

func command(for: Selector, propertyList: Any?) -> UICommand?

Gets the command for the specified selector and property list.

