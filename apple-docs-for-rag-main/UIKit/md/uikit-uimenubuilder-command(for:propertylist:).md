

- UIKit
- UIMenuBuilder
-  command(for:propertyList:) 

Instance Method

# command(for:propertyList:)

Gets the command for the specified selector and property list.

iOS 13.0+iPadOS 13.0+Mac CatalysttvOS 14.0+visionOS

``` source
@MainActor @preconcurrency
func command(
    for action: Selector,
    propertyList: Any? = nil
) -> UICommand?
```

## Parameters 

`action`  

The selector of the command to retrieve.

`propertyList`  

The property list object that identifies the command when more than one command uses the same action.

## Return Value

A command object; otherwise, `nil` if there is no such command.

## See Also

### Getting menu systems and elements

var system: UIMenuSystem

The menu system that the menu builder modifies.

**Required**

func menu(for: UIMenu.Identifier) -> UIMenu?

Gets the menu for the specified menu identifier.

**Required**

func action(for: UIAction.Identifier) -> UIAction?

Gets the action for the specified action identifier.

**Required**

