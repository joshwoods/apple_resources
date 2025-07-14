

- Authentication Services
- ASAuthorizationController
-  authorizationRequests 

Instance Property

# authorizationRequests

The authorization requests that the controller manages.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var authorizationRequests: [ASAuthorizationRequest] { get }
```

## Discussion

Use an authorization provider, like ASAuthorizationAppleIDProvider, ASAuthorizationPasswordProvider, or ASAuthorizationSingleSignOnProvider, to create a request for a particular purpose.

## See Also

### Inspecting requests

class ASAuthorizationRequest

A base class for different kinds of authorization requests.

var customAuthorizationMethods: [ASAuthorizationCustomMethod]

An array of custom authorization methods for the user to choose.

