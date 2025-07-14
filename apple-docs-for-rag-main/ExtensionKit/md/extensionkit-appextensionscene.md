

- ExtensionKit
-  AppExtensionScene 

Protocol

# AppExtensionScene

A protocol that defines the user interface for an application extension.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
protocol AppExtensionScene
```

## Topics

### Configuring the App Extension

var body: Self.Body

The content and behavior of the scene’s user interface.

**Required**

associatedtype Body : AppExtensionScene

The type for this scene’s body.

**Required**

## Relationships

### Conforming Types

- PrimitiveAppExtensionScene

## See Also

### UI App Extensions

struct AppExtensionSceneConfiguration

An object that holds configuration options for an extension scene.

struct AppExtensionSceneBuilder

A custom parameter attribute that constructs extension scenes from closures.

struct PrimitiveAppExtensionScene

A primitive you use to compose specialized app extension points.

