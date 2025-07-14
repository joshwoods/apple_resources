

- Authentication Services
- AuthorizationController
-  performRequest(\_:customMethods:) 

Instance Method

# performRequest(\_:customMethods:)

Performs the authorization request using a custom authorization method.

AuthenticationServicesSwiftUItvOS 16.4+

``` source
@MainActor
func performRequest(
    _ request: ASAuthorizationRequest,
    customMethods: [ASAuthorizationCustomMethod]
) async throws -> ASAuthorizationResult
```

## Parameters 

`request`  

The authorization request to perform.

`customMethods`  

An array of custom authorization methods to display in the system authorization UI. For more information, see ASAuthorizationCustomMethod.

## Return Value

The request’s outcome. For more information, see ASAuthorizationResult.

## Discussion

If the return value is ASAuthorizationResult.customMethod(_:), use the case’s associated value to access the chosen authorization method.

## See Also

### Performing requests

func performRequest(ASAuthorizationRequest) async throws -> ASAuthorizationResult

Performs the specified authorization request.

func performRequests([ASAuthorizationRequest]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array.

func performRequest(ASAuthorizationRequest, options: ASAuthorizationController.RequestOptions) async throws -> ASAuthorizationResult

Performs the specified authorization request with explicit options.

func performRequests([ASAuthorizationRequest], options: ASAuthorizationController.RequestOptions) async throws -> ASAuthorizationResult

Performs an authorization request, with explicit options, from the provided array.

func performRequests([ASAuthorizationRequest], customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array using a custom authorization method.

