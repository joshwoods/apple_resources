

- Local Authentication
-  LARight 

Class

# LARight

A grouped set of requirements that gate access to a resource or operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class LARight
```

## Overview

Use LARight instances to protect access to portions of your app that may contain sensitive information. By default, LARight instances require people to authenticate with Face ID, Touch ID, Apple Watch, or the device passcode. The following creates an LARight with the default authentication requirements:

```
let loginRight = LARight()

func login() async throws {
    try await loginRight.authorize(localizedReason: "Access sandcastle competition designs")
}

func logout() async {
    await loginRight.deauthorize()
}
```

## Topics

### Authorizing a right

init()

Creates a right using the default authorization requirements.

init(requirement: LAAuthenticationRequirement)

Creates a right with the authentication requirements you supply.

var tag: Int

An integer you use to identify a right.

func authorize(localizedReason: String, completion: ((any Error)?) -> Void)

Performs an authorization on the right.

func authorize(localizedReason: String, in: LAPresentationContext, completion: ((any Error)?) -> Void)

Performs an authorization on the right with a window context you supply.

### Deauthorizing a right

func deauthorize(completion: () -> Void)

Invalidates a previously authorized right.

### Monitoring authorization status

func checkCanAuthorize(completion: ((any Error)?) -> Void)

Checks whether the right has permission to perform authorization.

var state: LARight.State

The current authorization state for a right.

enum State

The possible states for a right during authorization.

## Relationships

### Inherits From

- NSObject

### Inherited By

- LAPersistedRight

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Authentication and access

enum State

The possible states for a right during authorization.

class LAContext

A mechanism for evaluating authentication policies and access controls.

