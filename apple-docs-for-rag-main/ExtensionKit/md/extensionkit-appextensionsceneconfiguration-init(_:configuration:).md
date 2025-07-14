

- ExtensionKit
- AppExtensionSceneConfiguration
-  init(\_:configuration:) 

Initializer

# init(\_:configuration:)

Creates a scene configuration object from a closure and extension configuration.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(
    _ content: @autoclosure @escaping @MainActor () -> Content,
    configuration: Configuration? = nil
) where Content : AppExtensionScene, Configuration : AppExtensionConfiguration
```

## Parameters 

`content`  

The SwiftUI closure from which to build the user interface for the scene configuration.

`configuration`  

An optional extension configuration file.

## Discussion

To provide a user interface, the extension’s `configuration` must be an AppExtensionSceneConfiguration, which combines an AppExtensionScene with an optional non-UI AppExtensionConfiguration. The `configuration` value you pass manages global interprocess comunications with the host process, while the `content` value you pass defines the extension’s user interface.

## See Also

### Creating Configuration Files

init&lt;Content>(@autoclosure () -> Content)

Creates a scene configuration from a closure.

