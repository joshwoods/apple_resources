

- ExtensionFoundation
-  AppExtensionConfiguration 

Protocol

# AppExtensionConfiguration

An object that holds configuration options for an app extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 9.0+

``` source
@MainActor @preconcurrency
protocol AppExtensionConfiguration : Sendable
```

## Topics

### Accepting Connection Requests

func accept(connection: NSXPCConnection) -> Bool

A method the system calls when a host app tries to connect.

**Required**

## Relationships

### Inherits From

- Sendable

## See Also

### App Extensions

struct AppExtensionIdentity

An object that uniquely identifies an app extension.

protocol AppExtension

Declares a type used by app extensions.

