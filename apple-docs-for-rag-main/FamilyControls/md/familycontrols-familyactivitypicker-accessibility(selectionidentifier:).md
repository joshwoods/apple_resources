

- FamilyControls
- FamilyActivityPicker
-  accessibility(selectionIdentifier:) 

Instance Method

# accessibility(selectionIdentifier:)

Sets a selection identifier for this view’s accessibility element.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0–1.0DeprecatedwatchOS 6.0+

``` source
nonisolated
func accessibility(selectionIdentifier: AnyHashable) -> ModifiedContent
```

## Discussion

Picker uses the value to determine what node to use for the accessibility value.

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

