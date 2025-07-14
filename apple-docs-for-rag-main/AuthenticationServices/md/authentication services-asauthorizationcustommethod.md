

- Authentication Services
-  ASAuthorizationCustomMethod 

Structure

# ASAuthorizationCustomMethod

The custom authorization method.

tvOS 15.0+

``` source
struct ASAuthorizationCustomMethod
```

## Discussion

Use ASAuthorizationCustomMethod to specify a type of custom sign-in in tvOS, like enabling the user to sign in manually or by restoring a purchase.

## Topics

### Creating the Structure

init(rawValue: String)

Initializes the object with a custom authorization method.

### Getting the Properties

static let videoSubscriberAccount: ASAuthorizationCustomMethod

A type of authorization that uses a TV provider account to sign in.

static let restorePurchase: ASAuthorizationCustomMethod

A type of authorization that restores an in-app purchase to sign in.

static let other: ASAuthorizationCustomMethod

A type of authorization that uses a custom sign-in method.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Apple TV authentication

var customAuthorizationMethods: [ASAuthorizationCustomMethod]

An array of custom authorization methods for the user to choose.

func authorizationController(ASAuthorizationController, didCompleteWithCustomMethod: ASAuthorizationCustomMethod)

Informs the delegate when authorization completes, and specifies the custom method the user selected.

