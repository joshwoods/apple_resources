

- SwiftUI
- TransitionPhase
-  value 

Instance Property

# value

A value that can be used to multiply effects that are applied differently depending on the phase.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var value: Double { get }
```

## Return Value

Zero when in the `identity` case, -1.0 for `willAppear`, and 1.0 for `didDisappear`.

## See Also

### Getting phase characteristics

var isIdentity: Bool

A Boolean that indicates whether the transition should have an identity effect, i.e. not change the appearance of its view.

