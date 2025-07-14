

- MarketplaceKit
- AppLibrary
-  didAuthenticate(account:) 

Instance Method

# didAuthenticate(account:)

Instructs iOS to reinstall an app after a required reuthorization completes.

iOS 17.5+iPadOS 17.5+

``` source
nonisolated
final func didAuthenticate(account: String) async
```

## Parameters 

`account`  

The account ID or username for the person. The marketplace server provides this value in the MarketplaceKitURIScheme installation request.

## Mentioned in 

Reauthenticating a person to manage apps

## Discussion

The marketplace or other web-distributed app calls this method after reauthenticating a person when the access token expires. For more information, see Reauthenticating a person to manage apps.

