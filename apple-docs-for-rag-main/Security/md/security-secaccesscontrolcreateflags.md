

- Security
-  SecAccessControlCreateFlags 

Structure

# SecAccessControlCreateFlags

Access control constants that dictate how a keychain item may be used.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct SecAccessControlCreateFlags
```

## Mentioned in 

Protecting keys with the Secure Enclave

Restricting keychain item accessibility

## Overview

Use these flags with the SecAccessControlCreateWithFlags(_:_:_:_:) function, or as the value associated with the kSecAttrAccessControl key in a keychain item’s attribute dictionary, to control keychain item accessibility.

## Topics

### Constraints

static var devicePasscode: SecAccessControlCreateFlags

Constraint to access an item with a passcode.

static var biometryAny: SecAccessControlCreateFlags

Constraint to access an item with Touch ID for any enrolled fingers, or Face ID.

static var biometryCurrentSet: SecAccessControlCreateFlags

Constraint to access an item with Touch ID for currently enrolled fingers, or from Face ID with the currently enrolled user.

static var userPresence: SecAccessControlCreateFlags

Constraint to access an item with either biometry or passcode.

static var watch: SecAccessControlCreateFlags

Constraint to access an item with a watch.

Deprecated

### Conjunctions

static var and: SecAccessControlCreateFlags

Indicates that all constraints must be satisfied.

static var or: SecAccessControlCreateFlags

Indicates that at least one constraint must be satisfied.

### Additional Options

static var applicationPassword: SecAccessControlCreateFlags

Option to use an application-provided password for data encryption key generation.

static var privateKeyUsage: SecAccessControlCreateFlags

Enable a private key to be used in signing a block of data or verifying a signed block.

### Initializers

init(rawValue: CFOptionFlags)

Initialize an access control creation flags object.

### Legacy Constraints

static var touchIDAny: SecAccessControlCreateFlags

Constraint to access an item with Touch ID for any enrolled fingers.

Deprecated

static var touchIDCurrentSet: SecAccessControlCreateFlags

Constraint to access an item with Touch ID for currently enrolled fingers.

Deprecated

### Type Properties

static var companion: SecAccessControlCreateFlags

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

