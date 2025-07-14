

- Video Subscriber Account
- VSUserAccountManager
-  userAccounts(options:) 

Instance Method

# userAccounts(options:)

Returns a list of registered user accounts for your app.

iOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+visionOS

``` source
func userAccounts(options: VSUserAccountManager.QueryOptions = []) async throws -> [VSUserAccount]
```

## Parameters 

`options`  

An array of options you specify to customize the user account query.

## Return Value

A list of registered user accounts for your app.

## Discussion

By default, this fetches and returns the list of registered user accounts on the current device. Provide the query option allDevices to fetch the list of registered user accounts on all the devices the user has in their iCloud account.

## See Also

### Getting user accounts

struct QueryOptions

Constants that represent options you use to fetch a list of user accounts.

