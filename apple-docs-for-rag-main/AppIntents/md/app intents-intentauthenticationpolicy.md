

- App Intents
-  IntentAuthenticationPolicy 

Enumeration

# IntentAuthenticationPolicy

An enumeration that describes the authentication policy to use when running an app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum IntentAuthenticationPolicy
```

## Topics

### Authentication policies

case alwaysAllowed

A policy that allows the app intent to always run, even on a locked device.

case requiresAuthentication

A policy that requires the user to authenticate.

case requiresLocalDeviceAuthentication

A policy that requires the user to authenticate on the local device.

### Operators

static func == (IntentAuthenticationPolicy, IntentAuthenticationPolicy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Specifying the authentication policy

static var authenticationPolicy: IntentAuthenticationPolicy

A property that defines the authentication policy that indicates whether this app intent requires the device to be unlocked or otherwise authenticated.

**Required** Default implementation provided.

