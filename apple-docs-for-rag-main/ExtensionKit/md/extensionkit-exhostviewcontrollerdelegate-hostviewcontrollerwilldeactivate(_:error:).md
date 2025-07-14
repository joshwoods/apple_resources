

- ExtensionKit
- EXHostViewControllerDelegate
-  hostViewControllerWillDeactivate(\_:error:) 

Instance Method

# hostViewControllerWillDeactivate(\_:error:)

A delegate method the host view controller calls when an extension disconnects.

macOS 13.0+

``` source
@MainActor
optional func hostViewControllerWillDeactivate(
    _ viewController: EXHostViewController,
    error: (any Error)?
)
```

## Parameters 

`viewController`  

The view controller for the extension that’s disconnecting

`error`  

An error object containing information about why the object disconnected, or `nil` if it’s disconnecting without error.

## Discussion

Called when the host view controller stops hosting the remote user interface. This can occur when the extension exits or when the view controller’s configuration property changes.

## See Also

### Delegate Methods

func hostViewControllerDidActivate(EXHostViewController)

A delegate method the view controller calls when a connection succeeds.

