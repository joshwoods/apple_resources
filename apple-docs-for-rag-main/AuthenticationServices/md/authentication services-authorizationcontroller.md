

- Authentication Services
-  AuthorizationController 

Structure

# AuthorizationController

A SwiftUI environment value that views use to perform authorization requests.

AuthenticationServicesSwiftUIiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
@MainActor
struct AuthorizationController
```

## Overview

To access an instance of this type, use the SwiftUI Environment property wrapper and specify authorizationController as the environment value, as the following example shows:

```
struct AuthorizationControllerExample: View {
    // Get an instance of AuthorizationController using SwiftUI's @Environment 
    // property wrapper.
    @Environment(\.authorizationController) private var authorizationController

    var body: some View {
        Button("Sign In") {
            Task {
                do {
                    // Create the authorization request.
                    async let request = makeAuthorizationRequest()
                    // Perform the request and await its result.
                    let result = try await authorizationController
                        .performRequest(request)
                    switch result {
                        // Process the request's result.
                    }
                } catch {
                    // Respond to any authorization errors.
                }
            }
        }
    }
}
```

## Topics

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

func performRequests([ASAuthorizationRequest], customMethods: [ASAuthorizationCustomMethod]) async throws -> ASAuthorizationResult

Performs an authorization request from the provided array using a custom authorization method.

### Performing assisted requests

func performAutoFillAssistedRequest(ASAuthorizationRequest) async throws -> ASAuthorizationResult

Performs an AutoFill-assisted authorization request.

func performAutoFillAssistedRequests([ASAuthorizationRequest]) async throws -> ASAuthorizationResult

Performs an AutoFill-assisted authorization request from the provided array.

## Relationships

### Conforms To

- Sendable

## See Also

### Authorization requests

class ASAuthorizationController

A controller that manages authorization requests that a provider creates.

enum ASAuthorizationResult

Describes the outcome of a successful authorization request.

