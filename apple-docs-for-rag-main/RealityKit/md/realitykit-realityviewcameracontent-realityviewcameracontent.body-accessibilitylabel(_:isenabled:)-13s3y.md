

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  accessibilityLabel(\_:isEnabled:) 

Instance Method

# accessibilityLabel(\_:isEnabled:)

Adds a label to the view that describes its contents.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityLabel(
    _ label: S,
    isEnabled: Bool
) -> ModifiedContent where S : StringProtocol
```

## Parameters 

`label`  

The accessibility label to apply.

`isEnabled`  

If true the accessibility label is applied; otherwise the accessibility label is unchanged.

## Discussion

Use this method to provide an accessibility label for a view that doesn’t display text, like an icon. For example, you could use this method to label a button that plays music with the text “Play”. Don’t include text in the label that repeats information that users already have. For example, don’t use the label “Play button” because a button already has a trait that identifies it as a button.

