

- Foundation
- URLCredential
-  URLCredential.Persistence 

Enumeration

# URLCredential.Persistence

Constants that specify how long the credential will be kept.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum Persistence
```

## Overview

In iOS, credentials are stored in the app’s keychain, and can be accessed only by that app (and other apps in the same keychain access group, where applicable).

In macOS, credentials are stored in the user’s keychain. The credential’s initial access control list (ACL) allows access only by that app. However, other apps can see that a password exists for a given host, port, and realm combination, and can request that the user grant permission to use that credential.

## Topics

### Persistence strategies

case none

The credential should not be stored.

case forSession

The credential should be stored only for this session.

case permanent

The credential should be stored in the keychain.

case synchronizable

The credential should be stored permanently in the keychain, and in addition should be distributed to other devices based on the owning Apple ID.

case none

The credential should not be stored.

case forSession

The credential should be stored only for this session.

case permanent

The credential should be stored in the keychain.

case synchronizable

The credential should be stored permanently in the keychain, and in addition should be distributed to other devices based on the owning Apple ID.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a credential

init(forTrust: SecTrust)

Creates a URL credential instance for server trust authentication with a given accepted trust.

init(identity: SecIdentity, certificates: [Any]?, persistence: URLCredential.Persistence)

Creates a URL credential instance for resolving a client certificate authentication challenge.

init(trust: SecTrust)

Creates a URL credential instance for server trust authentication, initialized with a accepted trust.

init(user: String, password: String, persistence: URLCredential.Persistence)

Creates a URL credential instance initialized with a given user name and password, using a given persistence setting.

