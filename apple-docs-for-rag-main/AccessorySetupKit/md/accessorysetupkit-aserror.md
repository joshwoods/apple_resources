

- AccessorySetupKit
-  ASError 

Structure

# ASError

An error encountered during accessory discovery.

iOS 18.0+iPadOS 18.0+

``` source
struct ASError
```

## Topics

### Activation errors

static var activationFailed: ASError.Code

### Life cycle errors

static var invalidated: ASError.Code

### Configuration errors

static var extensionNotFound: ASError.Code

static var invalidRequest: ASError.Code

### Picker errors

static var pickerRestricted: ASError.Code

static var pickerAlreadyActive: ASError.Code

### Cancellation and permission errors

static var userCancelled: ASError.Code

static var userRestricted: ASError.Code

### Communication errors

static var connectionFailed: ASError.Code

static var discoveryTimeout: ASError.Code

### Success cases

static var success: ASError.Code

### Unclassified errors

static var unknown: ASError.Code

### Accessing the error domain

static var errorDomain: String

The domain of the error.

let ASErrorDomain: String

NSError domain for AccessorySetupKit errors.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

Hashable Implementations

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

let ASErrorDomain: String

NSError domain for AccessorySetupKit errors.

enum Code

Codes that describe errors encountered during accessory discovery.

