

- RealityKit
- RealityViewDefaultPlaceholder
-  accessibilityLabel(\_:) 

Instance Method

# accessibilityLabel(\_:)

Adds a label to the view that describes its contents.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func accessibilityLabel(_ labelKey: LocalizedStringKey) -> ModifiedContent
```

## Discussion

Use this method to provide an accessibility label for a view that doesn’t display text, like an icon. For example, you could use this method to label a button that plays music with the text “Play”. Don’t include text in the label that repeats information that users already have. For example, don’t use the label “Play button” because a button already has a trait that identifies it as a button.

