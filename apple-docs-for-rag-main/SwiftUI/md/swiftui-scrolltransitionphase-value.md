

- SwiftUI
- ScrollTransitionPhase
-  value 

Instance Property

# value

A phase-derived value that can be used to scale or otherwise modify effects.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var value: Double { get }
```

## Discussion

Returns -1.0 when in the topLeading phase, zero when in the identity phase, and 1.0 when in the bottomTrailing phase.

## See Also

### Accessing the phase state

var isIdentity: Bool

