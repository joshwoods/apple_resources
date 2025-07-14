

- FamilyControls
- FamilyActivityPicker
-  accessibility(label:) 

Instance Method

# accessibility(label:)

Adds a label to the view that describes its contents.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func accessibility(label: Text) -> ModifiedContent
```

## Discussion

Use this method to provide an accessibility label for a view that doesn’t display text, like an icon. For example, you could use this method to label a button that plays music with the text “Play”. Don’t include text in the label that repeats information that users already have. For example, don’t use the label “Play button” because a button already has a trait that identifies it as a button.

## See Also

### Deprecated Accessibility Modifiers

func accessibility(value: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a textual description of the value that the view contains.

func accessibility(hidden: Bool) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies whether to hide this view from system accessibility features.

func accessibility(identifier: String) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Uses the specified string to identify the view.

func accessibility(selectionIdentifier: AnyHashable) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets a selection identifier for this view’s accessibility element.

Deprecated

func accessibility(hint: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Communicates to the user what happens after performing the view’s action.

func accessibility(activationPoint: CGPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies the point where activations occur in the view.

func accessibility(activationPoint: UnitPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies the unit point where activations occur in the view.

func accessibility(inputLabels: [Text]) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets alternate input labels with which users identify a view.

func accessibility(addTraits: AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds the given traits to the view.

func accessibility(removeTraits: AccessibilityTraits) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Removes the given traits from this view.

func accessibility(sortPriority: Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

func accessibilityCustomContent&lt;L, V>(L, V, importance: AXCustomContent.Importance) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Add additional accessibility information to the view.

Deprecated

