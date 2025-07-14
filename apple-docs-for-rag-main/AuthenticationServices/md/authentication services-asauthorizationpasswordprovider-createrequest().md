

- Authentication Services
- ASAuthorizationPasswordProvider
-  createRequest() 

Instance Method

# createRequest()

Creates a new password authorization request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 6.0+

``` source
func createRequest() -> ASAuthorizationPasswordRequest
```

## Return Value

A password authorization request that you can execute with an instance of ASAuthorizationController.

## See Also

### Creating Requests

class ASAuthorizationPasswordRequest

An authorization request that uses credentials stored in the keychain.

