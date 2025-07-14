

- RealityKit
- RealityViewDefaultPlaceholder
-  accessibilityActivationPoint(\_:isEnabled:) 

Instance Method

# accessibilityActivationPoint(\_:isEnabled:)

The activation point for an element is the location assistive technologies use to initiate gestures.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityActivationPoint(
    _ activationPoint: CGPoint,
    isEnabled: Bool
) -> ModifiedContent
```

## Parameters 

`activationPoint`  

The accessibility activation point to apply.

`isEnabled`  

If true the accessibility activation point is applied; otherwise the accessibility activation point is unchanged.

## Discussion

Use this modifier to ensure that the activation point for a small element remains accurate even if you present a larger version of the element to VoiceOver.

If an activation point is not provided, an activation point will be derived from one of the accessibility elements decedents or from the center of the accessibility frame.

