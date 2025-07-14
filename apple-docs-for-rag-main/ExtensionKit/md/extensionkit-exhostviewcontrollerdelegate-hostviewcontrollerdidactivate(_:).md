

- ExtensionKit
- EXHostViewControllerDelegate
-  hostViewControllerDidActivate(\_:) 

Instance Method

# hostViewControllerDidActivate(\_:)

A delegate method the view controller calls when a connection succeeds.

macOS 13.0+

``` source
@MainActor
optional func hostViewControllerDidActivate(_ viewController: EXHostViewController)
```

## Parameters 

`viewController`  

The user interface object from the remote process.

## Discussion

This delegate method gets called when the extension process has launched and the remote scene connects. After this delegate method gets called the host view controller can establish an XPC connection with the scene in the extension process.

## See Also

### Delegate Methods

func hostViewControllerWillDeactivate(EXHostViewController, error: (any Error)?)

A delegate method the host view controller calls when an extension disconnects.

