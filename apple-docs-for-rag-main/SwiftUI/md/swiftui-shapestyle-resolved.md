

- SwiftUI
- ShapeStyle
-  Resolved 

Associated Type

# Resolved

The type of shape style this will resolve to.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
associatedtype Resolved : ShapeStyle = Never
```

**Required**

## Discussion

When you create a custom shape style, Swift infers this type from your implementation of the required `resolve` function.

## See Also

### Resolving a shape style in an environment

func resolve(in: EnvironmentValues) -> Self.Resolved

Evaluate to a resolved shape style given the current `environment`.

**Required** Default implementation provided.

