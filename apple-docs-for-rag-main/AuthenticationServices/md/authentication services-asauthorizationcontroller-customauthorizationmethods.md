

- Authentication Services
- ASAuthorizationController
-  customAuthorizationMethods 

Instance Property

# customAuthorizationMethods

An array of custom authorization methods for the user to choose.

tvOS 15.0+

``` source
var customAuthorizationMethods: [ASAuthorizationCustomMethod] { get set }
```

## Discussion

Custom authorization methods provide a unified interface for signing in to apps, while allowing the developer to customize the login experience. For example, use other to display a username and password field, a web-based flow, or a custom user interface.

## See Also

### Apple TV authentication

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

struct ASAuthorizationCustomMethod

The custom authorization method.

