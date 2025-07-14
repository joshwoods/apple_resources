

- AppKit
- NSSharingServiceDelegate
-  sharingService(\_:willShareItems:) 

Instance Method

# sharingService(\_:willShareItems:)

Invoked when the sharing service will share the specified items.

macOS 10.8+

``` source
@MainActor
optional func sharingService(
    _ sharingService: NSSharingService,
    willShareItems items: [Any]
)
```

## Parameters 

`sharingService`  

The sharing service.

`items`  

The items being shared.

## See Also

### Sharing Items

func sharingService(NSSharingService, didShareItems: [Any])

Invoked when the sharing service has finished sharing the items.

func sharingService(NSSharingService, didFailToShareItems: [Any], error: any Error)

Invoked when the sharing service encountered an error when sharing items.

