

- FamilyControls
- FamilyActivityPicker
-  accessibilityInputLabels(\_:) 

Instance Method

# accessibilityInputLabels(\_:)

Sets alternate input labels with which users identify a view.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityInputLabels(_ inputLabels: [S]) -> ModifiedContent where S : StringProtocol
```

## Discussion

Provide labels in descending order of importance. Voice Control and Full Keyboard Access use the input labels.

Note

If you don’t specify any input labels, the user can still refer to the view using the accessibility label that you add with the `accessibilityLabel()` modifier.

## See Also

### Accessibility Labels

func accessibilityLabel&lt;S>(S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel(Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel(LocalizedStringKey) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityInputLabels([LocalizedStringKey]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels([Text]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

