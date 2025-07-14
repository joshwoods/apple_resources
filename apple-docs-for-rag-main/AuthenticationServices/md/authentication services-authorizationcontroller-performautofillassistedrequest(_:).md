

- Authentication Services
- AuthorizationController
-  performAutoFillAssistedRequest(\_:) 

Instance Method

# performAutoFillAssistedRequest(\_:)

Performs an AutoFill-assisted authorization request.

AuthenticationServicesSwiftUIiOS 16.4+iPadOS 16.4+visionOS 1.0+

``` source
@MainActor
func performAutoFillAssistedRequest(_ request: ASAuthorizationRequest) async throws -> ASAuthorizationResult
```

## Parameters 

`request`  

The authorization request to perform.

## Return Value

The request’s outcome. For more information, see ASAuthorizationResult.

## Discussion

To perform AutoFill-assisted authorization requests, add the appropriate textContentType(_:) to any sign-in related fields, such as those for usernames and passwords:

```
TextField("Username", text: $username)
    .textContentType(.username)
```

Then use task(priority:_:) or task(id:priority:_:) to perform the request when the view appears:

```
.task {
    // Create the authorization request.
    async let request = makeAutoFillAuthorizationRequest()
    // Perform the request and await its result.
    let result = try await authorizationController
        .performAutoFillAssistedRequest(request)
    switch result {
        // Process the request's result.
    }
}
```

## See Also

### Performing assisted requests

func performAutoFillAssistedRequests([ASAuthorizationRequest]) async throws -> ASAuthorizationResult

Performs an AutoFill-assisted authorization request from the provided array.

