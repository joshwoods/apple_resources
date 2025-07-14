

- Foundation
-  URLCredential 

Class

# URLCredential

`A`n authentication credential consisting of information specific to the type of credential and the type of persistent storage to use, if any.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLCredential
```

## Mentioned in 

Performing manual server trust authentication

## Overview

The URL Loading System supports password-based user credentials, certificate-based user credentials, and certificate-based server credentials.

When you create a credential, you can specify it for a single request, persist it temporarily (until your app quits), or persist it permanently. Permanent persistence can be local persistence in the keychain, or synchronized persistence across the user’s devices, based on their Apple ID.

Note

Permanent storage of credentials is only available for password-based credentials. TLS credentials are never stored permanently by URLCredentialStorage. In general, use for-session persistence for TLS credentials.

## Topics

### Creating a credential

init(forTrust: SecTrust)

Creates a URL credential instance for server trust authentication with a given accepted trust.

init(identity: SecIdentity, certificates: [Any]?, persistence: URLCredential.Persistence)

Creates a URL credential instance for resolving a client certificate authentication challenge.

init(trust: SecTrust)

Creates a URL credential instance for server trust authentication, initialized with a accepted trust.

init(user: String, password: String, persistence: URLCredential.Persistence)

Creates a URL credential instance initialized with a given user name and password, using a given persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

### Getting credential properties

var user: String?

The credential’s user name.

var certificates: [Any]

The intermediate certificates of the credential, if it is a client certificate credential.

var hasPassword: Bool

A Boolean value that indicates whether the credential has a password.

var password: String?

The credential’s password.

var identity: SecIdentity?

The identity of this credential if it is a client certificate credential.

var persistence: URLCredential.Persistence

The credential’s persistence setting.

enum Persistence

Constants that specify how long the credential will be kept.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Authentication and credentials

Handling an authentication challenge

Respond appropriately when a server demands authentication for a URL request.

class URLAuthenticationChallenge

A challenge from a server requiring authentication from the client.

class URLCredentialStorage

The manager of a shared credentials cache.

class URLProtectionSpace

A server or an area on a server, commonly referred to as a realm, that requires authentication.

