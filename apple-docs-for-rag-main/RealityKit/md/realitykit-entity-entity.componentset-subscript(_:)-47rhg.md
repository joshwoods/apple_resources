

- RealityKit
- Entity
- Entity.ComponentSet
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Gets or sets the component with a specific dynamically supplied type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
subscript(componentType: any Component.Type) -> (any Component)? { get set }
```

## See Also

### Accessing members

subscript&lt;T>(T.Type) -> T?

Gets or sets the component of the specified type.

