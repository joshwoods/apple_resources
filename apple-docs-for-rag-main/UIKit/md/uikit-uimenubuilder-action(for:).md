

- UIKit
- UIMenuBuilder
-  action(for:) 

Instance Method

# action(for:)

Gets the action for the specified action identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func action(for identifier: UIAction.Identifier) -> UIAction?
```

**Required**

## Parameters 

`identifier`  

The identifier of the action to retrieve.

## Return Value

An action object; otherwise, `nil` if there are no actions with the specified identifier.

## See Also

### Getting menu systems and elements

var system: UIMenuSystem

The menu system that the menu builder modifies.

**Required**

func menu(for: UIMenu.Identifier) -> UIMenu?

Gets the menu for the specified menu identifier.

**Required**

func command(for: Selector, propertyList: Any?) -> UICommand?

Gets the command for the specified selector and property list.

