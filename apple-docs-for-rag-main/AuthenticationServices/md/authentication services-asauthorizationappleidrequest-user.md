

- Authentication Services
- ASAuthorizationAppleIDRequest
-  user 

Instance Property

# user

An identifier associated with the user’s Apple ID.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var user: String? { get set }
```

## Discussion

Typically you leave this property set to `nil` the first time you authenticate a user. Otherwise, if you previously received an authorization containing an ASAuthorizationAppleIDCredential instance, set this property to the value from the credential’s user property.

The value is an arbitrary string that’s portable among apps from a single developer, but not between apps from different developers.

