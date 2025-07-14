

- CallKit
- CXErrorCodeCallDirectoryManagerError
-  CXErrorCodeCallDirectoryManagerError.Code 

Enumeration

# CXErrorCodeCallDirectoryManagerError.Code

Error codes the CallKit framework returns.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Constants

case unknown

An unknown error occurred.

case noExtensionFound

The call directory manager could not find a corresponding app extension.

case currentlyLoading

The call directory manager is loading the app extension.

case loadingInterrupted

The call directory manager was interrupted while loading the app extension.

case entriesOutOfOrder

The entries in the call directory are out of order.

case duplicateEntries

There are duplicate entries in the call directory.

case maximumEntriesExceeded

There are too many entries in the call directory.

case extensionDisabled

The call directory extension isn’t enabled by the system.

case unexpectedIncrementalRemoval

A request occurred before confirming incremental loading.

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

### Errors

enum EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

struct CXErrorCodeCallDirectoryManagerError

Errors when interacting with a call directory manager.

let CXErrorDomainCallDirectoryManager: String

Domain for errors when interacting with a call directory manager.

