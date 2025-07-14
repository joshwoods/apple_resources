

- App Intents
- SiriTipView
-  accessibilityLabeledPair(role:id:in:) 

Instance Method

# accessibilityLabeledPair(role:id:in:)

Pairs an accessibility element representing a label with the element for the matching content.

AppIntentsSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func accessibilityLabeledPair(
    role: AccessibilityLabeledPairRole,
    id: ID,
    in namespace: Namespace.ID
) -> some View where ID : Hashable
```

## Parameters 

`role`  

Determines whether this element should be used as the label in the pair, or the content in the pair.

`id`  

The identifier for the label / content pair. Elements with matching identifiers within the same namespace will be paired together.

`namespace`  

The namespace used to organize label and content. Label and content under the same namespace with matching identifiers will be paired together.

## Discussion

Use `accessibilityLabeledPair` with a role of `AccessibilityLabeledPairRole.label` to identify the label, and a role of `AccessibilityLabeledPairRole.content` to identify the content. This improves the behavior of accessibility features such as VoiceOver when navigating such elements, allowing users to better understand the relationship between them.

