

- Local Authentication
-  LAAccessControlOperation 

Enumeration

# LAAccessControlOperation

Operations to be evaluated for access control.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 3.0+

``` source
enum LAAccessControlOperation
```

## Overview

Use one of these values to specify the operation for which you want to evaluate an access control when calling the evaluateAccessControl(_:operation:localizedReason:reply:) method.

## Topics

### Constants

case createItem

Specifies that access control is used for item creation.

case useItem

Specifies that access control is used for accessing an existing item.

case createKey

Specifies that access control is used for key creation.

case useKeySign

Specifies that access control is used for accessing an existing key.

case useKeyDecrypt

Specifies that access control is used for data decryption using existing key.

case useKeyKeyExchange

Specifies that access control is used for key exchange.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Evaluating access controls

func evaluateAccessControl(SecAccessControl, operation: LAAccessControlOperation, localizedReason: String, reply: (Bool, (any Error)?) -> Void)

Evaluates an access control for a given operation.

var interactionNotAllowed: Bool

A Boolean value indicating whether authentication can be interactive.

