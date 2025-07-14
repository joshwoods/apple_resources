

- App Intents
- AppIntent
-  authenticationPolicy 

Type Property

# authenticationPolicy

A property that defines the authentication policy that indicates whether this app intent requires the device to be unlocked or otherwise authenticated.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var authenticationPolicy: IntentAuthenticationPolicy { get }
```

**Required** Default implementation provided.

## Default Implementations

### AppIntent Implementations

static var authenticationPolicy: IntentAuthenticationPolicy

A property that defines the authentication policy that indicates whether this app intent requires the device to be unlocked or otherwise authenticated.

## See Also

### Specifying the authentication policy

enum IntentAuthenticationPolicy

An enumeration that describes the authentication policy to use when running an app intent.

