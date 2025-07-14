

- SwiftUI
- View
-  accessibilityInputLabels(\_:) 

Instance Method

# accessibilityInputLabels(\_:)

Sets alternate input labels with which users identify a view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func accessibilityInputLabels(_ inputLabelKeys: [LocalizedStringKey]) -> ModifiedContent
```

Show all declarations

## Discussion

Provide labels in descending order of importance. Voice Control and Full Keyboard Access use the input labels.

Note

If you don’t specify any input labels, the user can still refer to the view using the accessibility label that you add with the `accessibilityLabel()` modifier.

## See Also

### Applying labels

func accessibilityLabel(_:)

Adds a label to the view that describes its contents.

func accessibilityLabel(_:isEnabled:)

Adds a label to the view that describes its contents.

func accessibilityLabel&lt;V>(content: (PlaceholderContentView&lt;Self>) -> V) -> some View

Adds a label to the view that describes its contents.

func accessibilityInputLabels(_:isEnabled:)

Sets alternate input labels with which users identify a view.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

enum AccessibilityLabeledPairRole

The role of an accessibility element in a label / content pair.

