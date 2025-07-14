

- SwiftUI
- View
-  accessibilityInputLabels(\_:isEnabled:) 

Instance Method

# accessibilityInputLabels(\_:isEnabled:)

Sets alternate input labels with which users identify a view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityInputLabels(
    _ inputLabelKeys: [LocalizedStringKey],
    isEnabled: Bool
) -> ModifiedContent
```

Show all declarations

## Parameters 

`inputLabelKeys`  

The accessibility input labels to apply.

`isEnabled`  

If true the accessibility input labels are applied; otherwise the accessibility input labels are unchanged.

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

func accessibilityInputLabels(_:)

Sets alternate input labels with which users identify a view.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

enum AccessibilityLabeledPairRole

The role of an accessibility element in a label / content pair.

