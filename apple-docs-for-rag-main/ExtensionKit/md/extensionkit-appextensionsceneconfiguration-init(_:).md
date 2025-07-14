

- ExtensionKit
- AppExtensionSceneConfiguration
-  init(\_:) 

Initializer

# init(\_:)

Creates a scene configuration from a closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(_ content: @autoclosure @escaping @MainActor () -> Content) where Content : AppExtensionScene
```

## Parameters 

`content`  

The SwiftUI closure from which to build the user interface for the scene configuration.

## See Also

### Creating Configuration Files

init&lt;Content, Configuration>(@autoclosure () -> Content, configuration: Configuration?)

Creates a scene configuration object from a closure and extension configuration.

