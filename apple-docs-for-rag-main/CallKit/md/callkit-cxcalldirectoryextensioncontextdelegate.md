

- CallKit
-  CXCallDirectoryExtensionContextDelegate 

Protocol

# CXCallDirectoryExtensionContextDelegate

A collection of methods a Call Directory extension context object calls when a request fails.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
protocol CXCallDirectoryExtensionContextDelegate : NSObjectProtocol
```

## Topics

### Handling Request Failures

func requestFailed(for: CXCallDirectoryExtensionContext, withError: any Error)

Called when a Call Directory app extension request fails.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Caller ID

Identifying and blocking calls

Create a Call Directory app extension to identify and block incoming callers by their phone number.

class CXCallDirectoryProvider

The principal object for a Call Directory app extension for a host app.

class CXCallDirectoryExtensionContext

A programmatic interface for adding identification and blocking entries to a Call Directory app extension.

class CXCallDirectoryManager

The programmatic interface to an object that manages a Call Directory app extension.

