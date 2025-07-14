

- SwiftUI
- Gesture
-  handActivationBehavior(\_:) 

Instance Method

# handActivationBehavior(\_:)

Customizes the activation behavior for a gesture when driven by hand or hand-like input.

visionOS 1.0+

``` source
@MainActor @preconcurrency
func handActivationBehavior(_ behavior: HandActivationBehavior) -> some Gesture
```

## Parameters 

`behavior`  

The hand activation behavior to use for the gesture.

## Return Value

A new gesture with a preference to activate with the provided behavior.

## Discussion

Use automatic to allow a gesture to activate with default system behaviors. Use pinch when a gesture should only trigger when the hand is pinched.

For example, in a 3D chess application, a DragGesture that enables movement of the pieces could use the pinch behavior to ensure that piece movement is only possible when a hand is pinched in order to avoid pushing the piece around by only touching it:

```
Model3D(named: "Pawn")
    .gesture(
        DragGesture()
            .handActivationBehavior(.pinch)
            .updating($chessDragState) { value, state, _ in
                // ...
            }
    )
```

