

- SwiftUI
-  AccessibilityLabeledPairRole 

Enumeration

# AccessibilityLabeledPairRole

The role of an accessibility element in a label / content pair.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
enum AccessibilityLabeledPairRole
```

## Topics

### Getting roles

case content

This element represents the content part of the label / content pair.

case label

This element represents the label part of the label / content pair.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

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

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

