

- Authentication Services
- AuthorizationController
-  performRequest(\_:) 

Instance Method

# performRequest(\_:)

Performs the specified authorization request.

AuthenticationServicesSwiftUIiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
@MainActor
func performRequest(_ request: ASAuthorizationRequest) async throws -> ASAuthorizationResult
```

## Parameters 

`request`  

The authorization request to perform.

## Return Value

The request’s outcome. For more information, see ASAuthorizationResult.

## See Also

### Performing requests

func performRequests([ASAuthorizationRequest]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array.

func performRequest(ASAuthorizationRequest, options: ASAuthorizationController.RequestOptions) async throws -> ASAuthorizationResult

Performs the specified authorization request with explicit options.

func performRequests([ASAuthorizationRequest], options: ASAuthorizationController.RequestOptions) async throws -> ASAuthorizationResult

Performs an authorization request, with explicit options, from the provided array.

func performRequest(ASAuthorizationRequest, customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs the authorization request using a custom authorization method.

func performRequests([ASAuthorizationRequest], customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array using a custom authorization method.

