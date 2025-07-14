

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  accessibilityLinkedGroup(id:in:) 

Instance Method

# accessibilityLinkedGroup(id:in:)

Links multiple accessibility elements so that the user can quickly navigate from one element to another, even when the elements are not near each other in the accessibility hierarchy.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+

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

