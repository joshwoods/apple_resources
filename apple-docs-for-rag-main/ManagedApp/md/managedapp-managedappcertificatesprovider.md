

- ManagedApp
-  ManagedAppCertificatesProvider 

Class

# ManagedAppCertificatesProvider

A class that provides certificates that an MDM admin provisions for a managed app or extension.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
class ManagedAppCertificatesProvider
```

## Mentioned in 

Accessing provisioned secrets with identifiers

## Overview

Create an instance of this class when your app needs to access certificates that the MDM admin provisions for your app from their MDM server.

## Topics

### Initializing a certificates provider

init()

Initializes a managed app certificates provider.

### Identifying cerificates

var identifiers: some AsyncSequence&lt;Array&lt;String>, Never>

An asynchronous sequence of arrays of certificate identifiers provided by the MDM server.

### Accessing certificates

func certificate(withIdentifier: String) async throws(ManagedAppError) -> SecCertificate

Provides a certificate by its identifier.

## See Also

### Secrets and identifiers

Accessing provisioned secrets with identifiers

Specify the secrets your app requires for device management features, receive secrets from MDM servers and use secrets in your app.

class ManagedAppIdentitiesProvider

A class that provides identities that an MDM admin provisions for a managed app or extension.

class ManagedAppPasswordsProvider

A class that provides passwords that an MDM admin provisions for a managed app or extension.

