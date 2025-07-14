

- SwiftUI
- EnvironmentalModifier
-  resolve(in:) 

Instance Method

# resolve(in:)

Resolve to a concrete modifier in the given `environment`.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func resolve(in environment: EnvironmentValues) -> Self.ResolvedModifier
```

**Required**

## See Also

### Resolving a modifier

associatedtype ResolvedModifier : ViewModifier

The type of modifier to use after being resolved.

**Required**

