

- SwiftUI
- GestureStateGesture
-  init(base:state:body:) 

Initializer

# init(base:state:body:)

Creates a new gesture that’s the result of an ongoing gesture.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    base: Base,
    state: GestureState,
    body: @escaping (GestureStateGesture.Value, inout State, inout Transaction) -> Void
)
```

## Parameters 

`base`  

The originating gesture.

`state`  

The wrapped value of a GestureState property.

`body`  

The callback that SwiftUI invokes as the gesture’s value changes.

## See Also

### Creating an in-progress gesture

var base: Base

The originating gesture.

var state: GestureState&lt;State>

A value that changes as the user performs the gesture.

