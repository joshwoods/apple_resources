

- Security Foundation
-  SFAuthorization 

Class

# SFAuthorization

A class that allows you to restrict a user’s access to particular features in your Mac app or daemon.

macOS 10.3+

``` source
class SFAuthorization
```

## Overview

Important

The authorization services API is not supported within an app sandbox because it allows privilege escalation.

The SFAuthorization class is an interface for some of the functions in the Authorization Services API. You can use the authorizationRef() method to obtain an authorization reference, used in other calls to Authorization Services functions. The Authorization Services API is documented in Authorization Services.

## Topics

### Allocating and initializing an authorization object

class func authorization() -> Any!

Returns an authorization object initialized with a default environment, flags, and rights.

class func authorization(with: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!) -> Any!

Returns an authorization object initialized with the specified flags, rights and environment.

init!()

Initializes an authorization object with default environment, flags, and rights.

init!(flags: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!)

Initializes an authorization object with the specified flags, rights, and environment.

### Obtaining an authorization reference

func authorizationRef() -> AuthorizationRef!

Returns the authorization reference for this object.

### Authorizing rights

func obtain(withRights: UnsafePointer&lt;AuthorizationRights>!, flags: AuthorizationFlags, environment: UnsafePointer&lt;AuthorizationEnvironment>!, authorizedRights: UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AuthorizationRights>?>!) throws

Authorizes and preauthorizes rights to access a privileged operation and returns the granted rights.

func obtain(withRight: AuthorizationString!, flags: AuthorizationFlags) throws

Authorizes and preauthorizes one specific right.

### Preventing credentials from being shared

func invalidateCredentials()

Prevents any rights that were obtained by this object from being preserved.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

