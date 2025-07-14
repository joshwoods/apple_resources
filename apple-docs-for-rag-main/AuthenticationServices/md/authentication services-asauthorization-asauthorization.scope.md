

- Authentication Services
- ASAuthorization
-  ASAuthorization.Scope 

Structure

# ASAuthorization.Scope

The kinds of contact information that can be requested from the user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Scope
```

## Discussion

Use one or more of these values in the requestedScopes array that you configure in an instance of either ASAuthorizationAppleIDRequest or ASAuthorizationSingleSignOnRequest to request certain contact information from the user.

Inspect the authorizedScopes array of an ASAuthorizationAppleIDCredential instance, or the (similarly named) authorizedScopes array of an ASAuthorizationSingleSignOnCredential instance, to see what scopes the user actually authorized. This might differ from the scopes you requested.

## Topics

### Scopes

static let email: ASAuthorization.Scope

A scope that includes the user’s email address.

static let fullName: ASAuthorization.Scope

A scope that includes the user’s full name.

### Creating a Scope

init(String)

Creates a scope from the given string.

init(rawValue: String)

Creates a scope from the given string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the Scope

var requestedScopes: [ASAuthorization.Scope]?

The contact information to be requested from the user during authentication.

