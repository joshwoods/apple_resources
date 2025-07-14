

- AppKit
- NSSharingServiceDelegate
-  sharingService(\_:didFailToShareItems:error:) 

Instance Method

# sharingService(\_:didFailToShareItems:error:)

Invoked when the sharing service encountered an error when sharing items.

macOS 10.8+

``` source
@MainActor
optional func sharingService(
    _ sharingService: NSSharingService,
    didFailToShareItems items: [Any],
    error: any Error
)
```

## Parameters 

`sharingService`  

The sharing service.

`items`  

The items being shared.

`error`  

The error that was encountered when trying to share the item. If the error is NSUserCancelledError, the user simply cancelled the error.

## See Also

### Sharing Items

func sharingService(NSSharingService, willShareItems: [Any])

Invoked when the sharing service will share the specified items.

func sharingService(NSSharingService, didShareItems: [Any])

Invoked when the sharing service has finished sharing the items.

