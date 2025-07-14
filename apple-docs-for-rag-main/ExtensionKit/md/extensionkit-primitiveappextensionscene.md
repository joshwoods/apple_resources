

- ExtensionKit
-  PrimitiveAppExtensionScene 

Structure

# PrimitiveAppExtensionScene

A primitive you use to compose specialized app extension points.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
struct PrimitiveAppExtensionScene
```

## Topics

### Creating an Extension Scene

init&lt;Content>(id: String, content: () -> Content, onConnection: (NSXPCConnection) -> Bool)

Creates a new app extension scene.

### Defining the Scene

var body: Never

The scene’s user interface.

var debugDescription: String

A string that provides information about the scene.

### Default Implementations

CustomDebugStringConvertible Implementations

## Relationships

### Conforms To

- AppExtensionScene
- Copyable
- CustomDebugStringConvertible
- Sendable

## See Also

### UI App Extensions

protocol AppExtensionScene

A protocol that defines the user interface for an application extension.

struct AppExtensionSceneConfiguration

An object that holds configuration options for an extension scene.

struct AppExtensionSceneBuilder

A custom parameter attribute that constructs extension scenes from closures.

