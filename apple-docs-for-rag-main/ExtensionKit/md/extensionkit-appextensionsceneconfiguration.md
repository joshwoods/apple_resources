

- ExtensionKit
-  AppExtensionSceneConfiguration 

Structure

# AppExtensionSceneConfiguration

An object that holds configuration options for an extension scene.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct AppExtensionSceneConfiguration
```

## Topics

### Creating Configuration Files

init&lt;Content>(@autoclosure () -> Content)

Creates a scene configuration from a closure.

init&lt;Content, Configuration>(@autoclosure () -> Content, configuration: Configuration?)

Creates a scene configuration object from a closure and extension configuration.

### Managing the Connection

func accept(connection: NSXPCConnection) -> Bool

A closure the framework calls when a host tries to connect to this extension.

## Relationships

### Conforms To

- AppExtensionConfiguration
- Sendable

## See Also

### UI App Extensions

protocol AppExtensionScene

A protocol that defines the user interface for an application extension.

struct AppExtensionSceneBuilder

A custom parameter attribute that constructs extension scenes from closures.

struct PrimitiveAppExtensionScene

A primitive you use to compose specialized app extension points.

