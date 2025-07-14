

- Safari Services
- SFSafariExtensionHandling
-  popoverDidClose(in:) 

Instance Method

# popoverDidClose(in:)

Tells the handler that the app extension’s popover was closed.

macOS 10.12+

``` source
optional func popoverDidClose(in window: SFSafariWindow)
```

## Parameters 

`window`  

The window that displayed the popover.

## Mentioned in 

Adjusting settings for a toolbar item

## See Also

### Working with Popovers

func popoverViewController() -> SFSafariExtensionViewController

Asks the handler to provide a popover view controller for display.

func popoverWillShow(in: SFSafariWindow)

Tells the handler that the app extension’s popover is about to be opened.

