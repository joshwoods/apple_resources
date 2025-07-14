

- RealityKit
- ObjectCaptureView
-  accessibilityActivationPoint(\_:) 

Instance Method

# accessibilityActivationPoint(\_:)

The activation point for an element is the location assistive technologies use to initiate gestures.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityActivationPoint(_ activationPoint: CGPoint) -> ModifiedContent
```

## Discussion

Use this modifier to ensure that the activation point for a small element remains accurate even if you present a larger version of the element to VoiceOver.

If an activation point is not provided, an activation point will be derrived from one of the accessibility elements decendents or from the center of the accessibility frame.

