

- RealityKit
- RealityViewAttachmentBuilderContent
-  accessibilityInputLabels(\_:) 

Instance Method

# accessibilityInputLabels(\_:)

Sets alternate input labels with which users identify a view.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func accessibilityInputLabels(_ inputLabels: [Text]) -> ModifiedContent
```

## Parameters 

`inputLabels`  

An array of Text elements to use as input labels.

## Discussion

Provide labels in descending order of importance. Voice Control and Full Keyboard Access use the input labels.

Note

If you don’t specify any input labels, the user can still refer to the view using the accessibility label that you add with the `accessibilityLabel()` modifier.

