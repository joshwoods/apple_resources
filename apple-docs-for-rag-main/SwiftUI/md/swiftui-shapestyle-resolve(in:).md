

- SwiftUI
- ShapeStyle
-  resolve(in:) 

Instance Method

# resolve(in:)

Evaluate to a resolved shape style given the current `environment`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func resolve(in environment: EnvironmentValues) -> Self.Resolved
```

**Required** Default implementation provided.

## Default Implementations

### ShapeStyle Implementations

func resolve(in: EnvironmentValues) -> Never

## See Also

### Resolving a shape style in an environment

associatedtype Resolved : ShapeStyle = Never

The type of shape style this will resolve to.

**Required**

