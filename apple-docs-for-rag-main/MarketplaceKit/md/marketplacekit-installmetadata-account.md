

- MarketplaceKit
- InstallMetadata
-  account 

Instance Property

# account

A user ID for the person installing the app.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
let account: String
```

## Discussion

You set this value and the operating system sends it back to you as:

- The `login_hint` in the call to your authorization endpoint during re-authentication

- A parameter to your marketplace extension’s additionalHeaders(for:account:) callback

The system also groups apps in restore requests based on account.

