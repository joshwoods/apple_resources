

- SwiftUI
- GestureStateGesture
-  base 

Instance Property

# base

The originating gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var base: Base
```

## See Also

### Creating an in-progress gesture

init(base: Base, state: GestureState&lt;State>, body: (GestureStateGesture&lt;Base, State>.Value, inout State, inout Transaction) -> Void)

Creates a new gesture that’s the result of an ongoing gesture.

var state: GestureState&lt;State>

A value that changes as the user performs the gesture.

