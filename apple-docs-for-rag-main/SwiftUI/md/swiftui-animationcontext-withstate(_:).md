

- SwiftUI
- AnimationContext
-  withState(\_:) 

Instance Method

# withState(\_:)

Creates a new context from another one with a state that you provide.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func withState(_ state: AnimationState) -> AnimationContext where T : VectorArithmetic
```

## Parameters 

`state`  

The initial state for the new context.

## Return Value

A new context that contains the specified state.

## Discussion

Use this method to create a new context that contains the state that you provide and view environment values from the original context.

