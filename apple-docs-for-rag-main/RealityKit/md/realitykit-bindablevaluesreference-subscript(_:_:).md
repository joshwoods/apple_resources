

- RealityKit
- BindableValuesReference
-  subscript(\_:\_:) 

Instance Subscript

# subscript(\_:\_:)

Returns the bindable value at the subscripted index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
subscript(bindTarget: BindTarget, type: T.Type = T.self) -> BindableValue? where T : BindableData { get set }
```

