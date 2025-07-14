

- SwiftUI
- OutlineGroup
-  init(\_:children:content:) 

Initializer

# init(\_:children:content:)

Creates an outline group from a binding to a collection of root data elements and a key path to its children.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
init(
    _ data: Binding,
    children: WritableKeyPath,
    @ViewBuilder content: @escaping (Binding) -> Leaf
) where Data == Binding, ID == E.ID, C : MutableCollection, C : RandomAccessCollection, E : Identifiable, E == C.Element
```

Available when `Data` conforms to `RandomAccessCollection`, `ID` is `Data.Element.ID`, `Parent` conforms to `View`, `Parent` is `Leaf`, `Subgroup` is `DisclosureGroup`, and `Data.Element` conforms to `Identifiable`.

Show all declarations

## Parameters 

`data`  

A collection of tree-structured, identified data.

`children`  

A key path to a property whose non-`nil` value gives the children of `data`. A non-`nil` but empty value denotes an element capable of having children that’s currently childless, such as an empty directory in a file system. On the other hand, if the property at the key path is `nil`, then the outline group treats `data` as a leaf in the tree, like a regular file in a file system.

`content`  

A view builder that produces a content view based on an element in `data`.

## Discussion

This initializer creates an instance that uniquely identifies views across updates based on the identity of the underlying data element.

All generated disclosure groups begin in the collapsed state.

Make sure that the identifier of a data element only changes if you mean to replace that element with a new element, one with a new identity. If the ID of an element changes, then the content view generated from that element will lose any current state and animations.

## See Also

### Creating an outline group

init(_:children:)

Creates an outline group from a collection of root data elements and a key path to element’s children.

init(_:id:children:content:)

Creates an outline group from a binding to a collection of root data elements, the key path to a data element’s identifier, and a key path to its children.

