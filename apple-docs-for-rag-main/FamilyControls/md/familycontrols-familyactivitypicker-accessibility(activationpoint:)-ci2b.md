

- FamilyControls
- FamilyActivityPicker
-  accessibility(activationPoint:) 

Instance Method

# accessibility(activationPoint:)

Specifies the unit point where activations occur in the view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func accessibility(activationPoint: UnitPoint) -> ModifiedContent
```

## See Also

### Accessibility Activation Point

func accessibility(activationPoint: CGPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Specifies the point where activations occur in the view.

func accessibilityActivationPoint(CGPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The activation point for an element is the location assistive technologies use to initiate gestures.

func accessibilityActivationPoint(UnitPoint) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

The activation point for an element is the location assistive technologies use to initiate gestures.

