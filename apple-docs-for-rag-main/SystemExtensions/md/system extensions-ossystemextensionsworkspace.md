

- System Extensions
-  OSSystemExtensionsWorkspace 

Class

# OSSystemExtensionsWorkspace

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.1+

``` source
class OSSystemExtensionsWorkspace
```

## Overview

Note

Using the workspace API requires the system extension entitlement

## Topics

### Instance Methods

func addObserver(any OSSystemExtensionsWorkspaceObserver) throws

func removeObserver(any OSSystemExtensionsWorkspaceObserver)

func systemExtensions(forApplicationWithBundleID: String) throws -> Set&lt;OSSystemExtensionProperties>

### Type Properties

class var shared: OSSystemExtensionsWorkspace

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

