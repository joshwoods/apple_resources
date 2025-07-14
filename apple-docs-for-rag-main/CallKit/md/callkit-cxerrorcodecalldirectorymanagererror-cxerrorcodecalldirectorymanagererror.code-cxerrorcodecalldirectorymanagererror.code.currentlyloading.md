

- CallKit
- CXErrorCodeCallDirectoryManagerError
- CXErrorCodeCallDirectoryManagerError.Code
-  CXErrorCodeCallDirectoryManagerError.Code.currentlyLoading 

Case

# CXErrorCodeCallDirectoryManagerError.Code.currentlyLoading

The call directory manager is loading the app extension.

iOS 10.3+iPadOS 10.3+Mac Catalyst 10.3+visionOS 1.0+watchOS 3.2+

``` source
case currentlyLoading
```

## See Also

### Constants

case unknown

An unknown error occurred.

case noExtensionFound

The call directory manager could not find a corresponding app extension.

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

