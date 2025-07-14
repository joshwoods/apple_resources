

- FinanceKit
- FinanceStore
-  requestAuthorization() 

Instance Method

# requestAuthorization()

Prompts a person to give FinanceKit authorization to access financial data.

iOS 17.4+iPadOS 17.4+

``` source
func requestAuthorization() async throws -> AuthorizationStatus
```

## Return Value

An AuthorizationStatus value that indicates the current state of authorization.

## Discussion

If there are no accounts are available to display, the framework presents a “No Accounts” screen and returns a status of AuthorizationStatus.authorized or AuthorizationStatus.denied depending on the state of a person’s consent.

It’s safe to call this method multiple times; the framework prompts a person only if necessary.

## See Also

### Authorization

func authorizationStatus() async throws -> AuthorizationStatus

Checks the authorization status for the calling application.

enum AuthorizationStatus

