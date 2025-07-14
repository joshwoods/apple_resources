

- Authentication Services
-  ASOneTimeCodeCredentialIdentity 

Class

# ASOneTimeCodeCredentialIdentity

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
class ASOneTimeCodeCredentialIdentity
```

## Overview

An ASOneTimeCodeCredentialIdentity is used to describe an identity that can use a service upon successful one time code based authentication. Use this class to save entries into ASCredentialIdentityStore.

## Topics

### Initializers

init(serviceIdentifier: ASCredentialServiceIdentifier, label: String, recordIdentifier: String?)

### Instance Properties

var label: String

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASCredentialIdentity
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

