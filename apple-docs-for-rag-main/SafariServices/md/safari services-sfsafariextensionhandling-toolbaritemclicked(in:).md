

- Safari Services
- SFSafariExtensionHandling
-  toolbarItemClicked(in:) 

Instance Method

# toolbarItemClicked(in:)

A method the system calls when a user clicks a toolbar item associated with the app extension.

macOS 10.12+

``` source
optional func toolbarItemClicked(in window: SFSafariWindow)
```

## Parameters 

`window`  

The window containing the clicked toolbar item.

## Mentioned in 

Adjusting settings for a toolbar item

## Discussion

The toolbar item can either execute a command or display a popover.

## See Also

### Working with Toolbar Items

func validateToolbarItem(in: SFSafariWindow, validationHandler: (Bool, String) -> Void)

Determines if a toolbar menu item should be enabled or have badge text when browser state changes.

