

- Authentication Services
- ASAuthorizationControllerDelegate
-  authorizationController(\_:didCompleteWithCustomMethod:) 

Instance Method

# authorizationController(\_:didCompleteWithCustomMethod:)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

tvOS 15.0+

``` source
@MainActor
optional func authorizationController(
    _ controller: ASAuthorizationController,
    didCompleteWithCustomMethod method: ASAuthorizationCustomMethod
)
```

## Parameters 

`controller`  

The controller performing the authorization attempt.

`method`  

The custom method the user selected. For a list of custom methods, see ASAuthorizationCustomMethod.

## See Also

### Apple TV authentication

var customAuthorizationMethods: [ASAuthorizationCustomMethod]

An array of custom authorization methods for the user to choose.

struct ASAuthorizationCustomMethod

The custom authorization method.

