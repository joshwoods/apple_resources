

- RealityKit
- ParameterSet
-  subscript(\_:\_:) 

Instance Subscript

# subscript(\_:\_:)

Provides a bindable value for the given name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
subscript(name: String, type: T.Type = T.self) -> BindableValue? where T : BindableData { get set }
```

