

- Authentication Services
- AuthorizationController
-  performRequests(\_:customMethods:) 

Instance Method

# performRequests(\_:customMethods:)

Performs an authorization request from the provided array using a custom authorization method.

AuthenticationServicesSwiftUItvOS 16.4+

``` source
@MainActor
func performRequests(
    _ requests: [ASAuthorizationRequest],
    customMethods: [ASAuthorizationCustomMethod]
) async throws -> ASAuthorizationResult
```

## Parameters 

`requests`  

An array of supported authorization requests.

`customMethods`  

An array of custom authorization methods to display in the system authorization UI. For more information, see ASAuthorizationCustomMethod.

## Return Value

The request’s outcome. For more information, see ASAuthorizationResult.

## Discussion

The framework checks each authorization request in the array against the credentials available on the person’s device; the more credential types your app supports, the more options a person can choose from.

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

func performRequest(ASAuthorizationRequest, customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs the authorization request using a custom authorization method.

