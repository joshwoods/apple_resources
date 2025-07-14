

- FinanceKit
- FinanceStore
-  authorizationStatus() 

Instance Method

# authorizationStatus()

Checks the authorization status for the calling application.

iOS 17.4+iPadOS 17.4+

``` source
func authorizationStatus() async throws -> AuthorizationStatus
```

## Return Value

An AuthorizationStatus value that indicates the current state of authorization.

## See Also

### Authorization

func requestAuthorization() async throws -> AuthorizationStatus

Prompts a person to give FinanceKit authorization to access financial data.

enum AuthorizationStatus

