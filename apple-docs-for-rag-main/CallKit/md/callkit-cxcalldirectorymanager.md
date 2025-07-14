

- CallKit
-  CXCallDirectoryManager 

Class

# CXCallDirectoryManager

The programmatic interface to an object that manages a Call Directory app extension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
class CXCallDirectoryManager
```

## Topics

### Accessing the Shared Instance

class var sharedInstance: CXCallDirectoryManager

Returns the shared call directory manager instance for the app.

### Working with a Call Directory App Extension

func getEnabledStatusForExtension(withIdentifier: String, completionHandler: (CXCallDirectoryManager.EnabledStatus, (any Error)?) -> Void)

Asynchronously returns the enabled status of the extension with the specified identifier.

func reloadExtension(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Asynchronously reloads the extension with the specified identifier.

enum EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

### Opening the Settings App

func openSettings(completionHandler: (((any Error)?) -> Void)?)

Opens the iOS Settings app and shows the Call Blocking & Identification settings.

### Errors

enum EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

struct CXErrorCodeCallDirectoryManagerError

Errors when interacting with a call directory manager.

enum Code

Error codes the CallKit framework returns.

let CXErrorDomainCallDirectoryManager: String

Domain for errors when interacting with a call directory manager.

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

## See Also

### Caller ID

Identifying and blocking calls

Create a Call Directory app extension to identify and block incoming callers by their phone number.

class CXCallDirectoryProvider

The principal object for a Call Directory app extension for a host app.

class CXCallDirectoryExtensionContext

A programmatic interface for adding identification and blocking entries to a Call Directory app extension.

protocol CXCallDirectoryExtensionContextDelegate

A collection of methods a Call Directory extension context object calls when a request fails.

