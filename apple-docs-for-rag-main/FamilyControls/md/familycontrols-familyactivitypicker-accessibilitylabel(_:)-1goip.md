

- FamilyControls
- FamilyActivityPicker
-  accessibilityLabel(\_:) 

Instance Method

# accessibilityLabel(\_:)

Adds a label to the view that describes its contents.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityLabel(_ labelKey: LocalizedStringKey) -> ModifiedContent
```

## Discussion

Use this method to provide an accessibility label for a view that doesn’t display text, like an icon. For example, you could use this method to label a button that plays music with the text “Play”. Don’t include text in the label that repeats information that users already have. For example, don’t use the label “Play button” because a button already has a trait that identifies it as a button.

## See Also

### Accessibility Labels

func accessibilityLabel&lt;S>(S) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityLabel(Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

func accessibilityInputLabels([LocalizedStringKey]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels([Text]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityInputLabels&lt;S>([S]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibilityLabeledPair&lt;ID>(role: AccessibilityLabeledPairRole, id: ID, in: Namespace.ID) -> some View

Pairs an accessibility element representing a label with the element for the matching content.

