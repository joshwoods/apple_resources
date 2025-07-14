

- Safari Services
- SFSafariExtensionHandling
-  popoverWillShow(in:) 

Instance Method

# popoverWillShow(in:)

Tells the handler that the app extension’s popover is about to be opened.

macOS 10.12+

``` source
optional func popoverWillShow(in window: SFSafariWindow)
```

## Parameters 

`window`  

The window to display the popover in.

## Mentioned in 

Adjusting settings for a toolbar item

## Discussion

This method is called when a popover associated with the app extension is triggered.

## See Also

### Working with Popovers

func popoverViewController() -> SFSafariExtensionViewController

Asks the handler to provide a popover view controller for display.

func popoverDidClose(in: SFSafariWindow)

Tells the handler that the app extension’s popover was closed.

