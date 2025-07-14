

- SwiftUI
- EnvironmentalModifier
-  ResolvedModifier 

Associated Type

# ResolvedModifier

The type of modifier to use after being resolved.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype ResolvedModifier : ViewModifier
```

**Required**

## See Also

### Resolving a modifier

func resolve(in: EnvironmentValues) -> Self.ResolvedModifier

Resolve to a concrete modifier in the given `environment`.

**Required**

