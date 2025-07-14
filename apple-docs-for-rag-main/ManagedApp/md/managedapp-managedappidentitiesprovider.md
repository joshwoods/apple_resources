

- ManagedApp
-  ManagedAppIdentitiesProvider 

Class

# ManagedAppIdentitiesProvider

A class that provides identities that an MDM admin provisions for a managed app or extension.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
class ManagedAppIdentitiesProvider
```

## Mentioned in 

Accessing provisioned secrets with identifiers

## Overview

Create an instance of this class when your app needs to access identities that the MDM admin provisions for your app from their MDM server.

## Topics

### Initializing an identities provider

init()

Initializes an identities provider.

### Identifying identities

var identifiers: some AsyncSequence&lt;Array&lt;String>, Never>

An asynchronous sequence of arrays of identity identifiers provided by the MDM server.

### Accessing identities

func identity(withIdentifier: String) async throws(ManagedAppError) -> SecIdentity

Provides an identity by its identifier.

## See Also

### Secrets and identifiers

Accessing provisioned secrets with identifiers

Specify the secrets your app requires for device management features, receive secrets from MDM servers and use secrets in your app.

class ManagedAppCertificatesProvider

A class that provides certificates that an MDM admin provisions for a managed app or extension.

class ManagedAppPasswordsProvider

A class that provides passwords that an MDM admin provisions for a managed app or extension.

