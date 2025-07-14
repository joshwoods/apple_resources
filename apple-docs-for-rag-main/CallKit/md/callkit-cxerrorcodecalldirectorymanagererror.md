

- CallKit
-  CXErrorCodeCallDirectoryManagerError 

Structure

# CXErrorCodeCallDirectoryManagerError

Errors when interacting with a call directory manager.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
struct CXErrorCodeCallDirectoryManagerError
```

## Topics

### Constants

static var unknown: CXErrorCodeCallDirectoryManagerError.Code

An unknown error occurred.

static var noExtensionFound: CXErrorCodeCallDirectoryManagerError.Code

The call directory manager can’t find a corresponding app extension.

static var currentlyLoading: CXErrorCodeCallDirectoryManagerError.Code

The call directory manager is loading the app extension.

static var loadingInterrupted: CXErrorCodeCallDirectoryManagerError.Code

The system interrupted the call directory manager while loading the app extension.

static var entriesOutOfOrder: CXErrorCodeCallDirectoryManagerError.Code

The entries in the call directory are out of order.

static var duplicateEntries: CXErrorCodeCallDirectoryManagerError.Code

There are duplicate entries in the call directory.

static var maximumEntriesExceeded: CXErrorCodeCallDirectoryManagerError.Code

There are too many entries in the call directory.

static var extensionDisabled: CXErrorCodeCallDirectoryManagerError.Code

The call directory extension isn’t in an enabled state.

static var unexpectedIncrementalRemoval: CXErrorCodeCallDirectoryManagerError.Code

A request occurred before confirming incremental loading.

### Enumerations

enum Code

Error codes the CallKit framework returns.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

enum Code

Error codes the CallKit framework returns.

let CXErrorDomainCallDirectoryManager: String

Domain for errors when interacting with a call directory manager.

