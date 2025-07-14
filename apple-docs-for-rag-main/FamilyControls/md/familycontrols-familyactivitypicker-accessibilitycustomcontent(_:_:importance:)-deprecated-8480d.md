

- FamilyControls
- FamilyActivityPicker
-  accessibilityCustomContent(\_:\_:importance:) Deprecated

Instance Method

# accessibilityCustomContent(\_:\_:importance:)

Add additional accessibility information to the view.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func accessibilityCustomContent(
    _ label: L,
    _ value: V,
    importance: AXCustomContent.Importance = .default
) -> ModifiedContent where L : StringProtocol, V : StringProtocol
```

Deprecated

Using non-localized strings for labels is not directly supported. Instead, wrap both the label and the value in a Text struct.

## Parameters 

`label`  

Localized text describing to the user what is contained in this additional information entry. For example: “orientation”.

`value`  

Text value for the additional accessibility information. For example: “landscape.”

`importance`  

Importance of the accessibility information. High-importance information gets read out immediately, while default-importance information must be explicitly asked for by the user.

## Discussion

Use this method to add information you want accessibility users to be able to access about this element, beyond the basics of label, value, and hint. For example, `accessibilityCustomContent` can be used to add information about the orientation of a photograph, or the number of people found in the picture.

Note

Repeated calls of `accessibilityCustomContent` with different labels will create new entries of additional information. Calling `accessibilityAdditionalContent` repeatedly with the same label will instead replace the previous value and importance.

## See Also

### Deprecated Accessibility Modifiers

func accessibility(label: Text) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds a label to the view that describes its contents.

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

