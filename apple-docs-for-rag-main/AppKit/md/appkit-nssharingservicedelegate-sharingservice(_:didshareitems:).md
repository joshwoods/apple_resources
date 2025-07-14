

- AppKit
- NSSharingServiceDelegate
-  sharingService(\_:didShareItems:) 

Instance Method

# sharingService(\_:didShareItems:)

Invoked when the sharing service has finished sharing the items.

macOS 10.8+

``` source
@MainActor
optional func sharingService(
    _ sharingService: NSSharingService,
    didShareItems items: [Any]
)
```

## Parameters 

`sharingService`  

The sharing service.

`items`  

The items being shared.

## See Also

### Sharing Items

func sharingService(NSSharingService, willShareItems: [Any])

Invoked when the sharing service will share the specified items.

func sharingService(NSSharingService, didFailToShareItems: [Any], error: any Error)

Invoked when the sharing service encountered an error when sharing items.

