

- Video Subscriber Account
- VSUserAccount
-  init(accountType:updateURL:) 

Initializer

# init(accountType:updateURL:)

Creates a user account object with a URL for account update requests.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS

``` source
init(
    accountType: VSUserAccount.AccountType = .free,
    updateURL: URL?
)
```

## Parameters 

`accountType`  

A constant that represents whether a user has access to paid content.

`updateURL`  

A URL that points to the application’s JavaScript endpoint for update requests.

## See Also

### Creating user accounts

enum AccountType

Constants that represent whether a user has access to paid content.

