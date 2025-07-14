

- SwiftUI
- View
-  accessibilityLinkedGroup(id:in:) 

Instance Method

# accessibilityLinkedGroup(id:in:)

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func accessibilityLinkedGroup(
    id: ID,
    in namespace: Namespace.ID
) -> some View where ID : Hashable
```

## Parameters 

`id`  

A hashable identifier used to separate sets of linked elements within the same namespace. Elements with matching `namespace` and `id` will be linked together.

`namespace`  

The namespace to use to organize linked accessibility elements. All elements marked with `accessibilityLink` in this namespace and with the specified `id` will be linked together.

## Discussion

This can be useful to allow quickly jumping between content in a list and the same content shown in a detail view, for example. All elements marked with `accessibilityLinkedGroup` with the same namespace and identifier will be linked together.

## See Also

### Configuring rotors

func accessibilityRotorEntry&lt;ID>(id: ID, in: Namespace.ID) -> some View

Defines an explicit identifier tying an Accessibility element for this view to an entry in an Accessibility Rotor.

func accessibilitySortPriority(Double) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Sets the sort priority order for this view’s accessibility element, relative to other elements at the same level.

