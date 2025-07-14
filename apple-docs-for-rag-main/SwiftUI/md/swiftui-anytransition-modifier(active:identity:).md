

- SwiftUI
- AnyTransition
-  modifier(active:identity:) 

Type Method

# modifier(active:identity:)

Returns a transition defined between an active modifier and an identity modifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func modifier(
    active: E,
    identity: E
) -> AnyTransition where E : ViewModifier
```

## See Also

### Creating a custom transition

init&lt;T>(T)

Create an instance that type-erases `transition`.

