

- SwiftUI
- View
-  accessibilityRotorEntry(id:in:) 

Instance Method

# accessibilityRotorEntry(id:in:)

Defines an explicit identifier tying an Accessibility element for this view to an entry in an Accessibility Rotor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func accessibilityRotorEntry(
    id: ID,
    in namespace: Namespace.ID
) -> some View where ID : Hashable
```

## Parameters 

`id`  

An arbitrary hashable identifier. Pass this same value when initializing an AccessibilityRotorEntry.

`namespace`  

A namespace created with `@Namespace()`. Pass this same namespace when initializing an `AccessibilityRotorEntry`.

## Discussion

Use this when creating an AccessibilityRotorEntry without a namespace does not allow SwiftUI to automatically find and reveal the element, or when the Rotor entry should be associated with a sub-element of a complex view generated in a ForEach, for example.

## See Also

### Configuring rotors

func accessibilityLinkedGroup&lt;ID>(id: ID, in: Namespace.ID) -> some View

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

func accessibilitySortPriority(Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

