

- SwiftUI
- AnyTransition
-  init(\_:) 

Initializer

# init(\_:)

Create an instance that type-erases `transition`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(_ transition: T) where T : Transition
```

## See Also

### Creating a custom transition

static func modifier&lt;E>(active: E, identity: E) -> AnyTransition

Returns a transition defined between an active modifier and an identity modifier.

