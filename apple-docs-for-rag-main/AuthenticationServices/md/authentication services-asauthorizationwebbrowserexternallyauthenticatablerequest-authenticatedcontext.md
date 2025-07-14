

- Authentication Services
- ASAuthorizationWebBrowserExternallyAuthenticatableRequest
-  authenticatedContext 

Instance Property

# authenticatedContext

The local authentication context for the authorization.

macOS 13.3+

``` source
var authenticatedContext: LAContext? { get set }
```

**Required**

## Discussion

Ensure the person authenticates, for example using FaceID, before accessing their credentials.

