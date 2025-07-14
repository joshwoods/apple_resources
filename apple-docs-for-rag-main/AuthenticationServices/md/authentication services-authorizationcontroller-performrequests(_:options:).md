

- Authentication Services
- AuthorizationController
-  performRequests(\_:options:) 

Instance Method

# performRequests(\_:options:)

Performs an authorization request, with explicit options, from the provided array.

AuthenticationServicesSwiftUIiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+visionOS 1.0+

``` source
@MainActor
func performRequests(
    _ requests: [ASAuthorizationRequest],
    options: ASAuthorizationController.RequestOptions
) async throws -> ASAuthorizationResult
```

## Parameters 

`requests`  

An array of supported authorization requests.

`options`  

Additional options that customize the request’s behavior. For more information, see ASAuthorizationController.RequestOptions.

## Return Value

The request’s outcome. For more information, see ASAuthorizationResult.

## Discussion

The framework checks each authorization request in the array against the credentials available on the person’s device; the more credential types your app supports, the more options a person can choose from.

## See Also

### Performing requests

func performRequest(ASAuthorizationRequest) async throws -> ASAuthorizationResult

Performs the specified authorization request.

func performRequests([ASAuthorizationRequest]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array.

func performRequest(ASAuthorizationRequest, options: ASAuthorizationController.RequestOptions) async throws -> ASAuthorizationResult

Performs the specified authorization request with explicit options.

func performRequest(ASAuthorizationRequest, customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs the authorization request using a custom authorization method.

func performRequests([ASAuthorizationRequest], customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array using a custom authorization method.

