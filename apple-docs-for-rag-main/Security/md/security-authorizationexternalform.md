

- Security
-  AuthorizationExternalForm 

Structure

# AuthorizationExternalForm

The external representation of an authorization reference.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AuthorizationExternalForm
```

## Overview

Authorization references are bound by session, process, and time limits, so you can’t store the authorization references for another process to use. Use the functions AuthorizationMakeExternalForm(_:_:) and AuthorizationCreateFromExternalForm(_:_:) to externalize and internalize the authorization reference. Apps should take care not to disclose the external authorization reference to potential attackers since any process can use this external authorization reference to access the authorization reference.

## Topics

### Initializers

init()

init(bytes: (CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar))

### Instance Properties

var bytes: (CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar, CChar)

An array of characters representing the external form of an authorization reference.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

