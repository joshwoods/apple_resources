

- FamilyControls
- FamilyActivityPicker
-  accessibilityHidden(\_:) 

Instance Method

# accessibilityHidden(\_:)

Specifies whether to hide this view from system accessibility features.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

``` source
nonisolated
func accessibilityHidden(_ hidden: Bool) -> ModifiedContent
```

## See Also

### Accessibility Elements

func accessibilityElement(children: AccessibilityChildBehavior) -> some View

Creates a new accessibility element, or modifies the `AccessibilityChildBehavior` of the existing accessibility element.

func accessibilityChildren&lt;V>(children: () -> V) -> some View

Replaces the existing accessibility element’s children with one or more new synthetic accessibility elements.

