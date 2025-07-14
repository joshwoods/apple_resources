

- SwiftUI
- View
-  accessibilityLabeledPair(role:id:in:) 

Instance Method

# accessibilityLabeledPair(role:id:in:)

Pairs an accessibility element representing a label with the element for the matching content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

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

## See Also

### Applying labels

func accessibilityLabel(_:)

Adds a label to the view that describes its contents.

func accessibilityLabel(_:isEnabled:)

Adds a label to the view that describes its contents.

func accessibilityLabel&lt;V>(content: (PlaceholderContentView&lt;Self>) -> V) -> some View

Adds a label to the view that describes its contents.

func accessibilityInputLabels(_:)

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels(_:isEnabled:)

Sets alternate input labels with which users identify a view.

enum AccessibilityLabeledPairRole

The role of an accessibility element in a label / content pair.

