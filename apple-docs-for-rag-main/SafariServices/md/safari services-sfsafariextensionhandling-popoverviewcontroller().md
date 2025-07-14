

- Safari Services
- SFSafariExtensionHandling
-  popoverViewController() 

Instance Method

# popoverViewController()

Asks the handler to provide a popover view controller for display.

macOS 10.12+

``` source
optional func popoverViewController() -> SFSafariExtensionViewController
```

## Return Value

The app extension’s popover view controller.

## Mentioned in 

Adjusting settings for a toolbar item

## See Also

### Working with Popovers

func popoverWillShow(in: SFSafariWindow)

Tells the handler that the app extension’s popover is about to be opened.

func popoverDidClose(in: SFSafariWindow)

Tells the handler that the app extension’s popover was closed.

