

- Safari Services
- SFSafariExtensionHandling
-  validateToolbarItem(in:validationHandler:) 

Instance Method

# validateToolbarItem(in:validationHandler:)

Determines if a toolbar menu item should be enabled or have badge text when browser state changes.

macOS 10.12+

``` source
optional func validateToolbarItem(
    in window: SFSafariWindow,
    validationHandler: @escaping (Bool, String) -> Void
)
```

## Parameters 

`window`  

The window containing the clicked toolbar item.

`validationHandler`  

A code block used to set the state of the toolbar item.

## Mentioned in 

Adjusting settings for a toolbar item

## Discussion

This method is called by the setToolbarItemsNeedUpdate() method or when Safari’s state changes in a way that may affect the toolbar item’s enabled or badge state. Your handler should decide whether the toolbar menu should be enabled and whether it should have any badge text, and then call the `validationHandler` block to update the toolbar item state.

## See Also

### Working with Toolbar Items

func toolbarItemClicked(in: SFSafariWindow)

A method the system calls when a user clicks a toolbar item associated with the app extension.

