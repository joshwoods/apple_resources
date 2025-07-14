

- CallKit
-  CXCallDirectoryProvider 

Class

# CXCallDirectoryProvider

The principal object for a Call Directory app extension for a host app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
class CXCallDirectoryProvider
```

## Mentioned in 

Identifying and blocking calls

## Topics

### Beginning a Request

func beginRequest(with: CXCallDirectoryExtensionContext)

Tells the extension to prepare for a host app’s request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Caller ID

Identifying and blocking calls

Create a Call Directory app extension to identify and block incoming callers by their phone number.

class CXCallDirectoryExtensionContext

A programmatic interface for adding identification and blocking entries to a Call Directory app extension.

protocol CXCallDirectoryExtensionContextDelegate

A collection of methods a Call Directory extension context object calls when a request fails.

class CXCallDirectoryManager

The programmatic interface to an object that manages a Call Directory app extension.

