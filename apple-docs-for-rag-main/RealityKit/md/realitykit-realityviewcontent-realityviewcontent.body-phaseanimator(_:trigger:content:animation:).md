

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  phaseAnimator(\_:trigger:content:animation:) 

Instance Method

# phaseAnimator(\_:trigger:content:animation:)

Animates effects that you apply to a view over a sequence of phases that change based on a trigger.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
nonisolated
func phaseAnimator(
    _ phases: some Sequence,
    trigger: some Equatable,
    @ViewBuilder content: @escaping (PlaceholderContentView, Phase) -> some View,
    animation: @escaping (Phase) -> Animation? = { _ in .default }
) -> some View where Phase : Equatable
```

## Parameters 

`phases`  

The sequence of phases to cycle through. Ensure that the sequence isn’t empty. If it is, SwiftUI logs a runtime warning and also returns a visual warning as the output view.

`trigger`  

A value whose changes cause the animator to use the next phase.

`content`  

A view builder closure that takes two parameters: a proxy value representing the modified view and the current phase. You can apply effects to the proxy based on the current phase.

`animation`  

A closure that takes the current phase as input. Return the animation to use when transitioning to the next phase. If you return `nil`, the transition doesn’t animate. If you don’t set this parameter, SwiftUI uses a default animation.

## Discussion

When the modified view first appears, this modifier renders its `content` closure using the first phase as input to the closure, along with a proxy for the modified view. Apply effects to the proxy — and thus to the modified view — in a way that’s appropriate for the first phase value.

Later, when the value of the `trigger` input changes, the modifier provides its `content` closure with the value of the second phase. Update the effects that you apply to the proxy view accordingly, and the modifier animates the change for you. The next time the `trigger` input changes, this procedure repeats using successive phases until reaching the last phase, at which point the modifier loops back to the first phase.

