

- SwiftUI
- OutlineGroup
-  init(\_:children:) 

Initializer

# init(\_:children:)

Creates an outline group from a collection of root data elements and a key path to element’s children.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(
    _ data: Data,
    children: KeyPath
) where ID == DataElement.ID, Parent == TableRow, Leaf == TableRow, Subgroup == TableRow, DataElement : Identifiable, DataElement == Data.Element
```

Available when `Data` conforms to `RandomAccessCollection`, `ID` is `Data.Element.ID`, `Parent` conforms to `TableRowContent`, `Parent` is `Leaf`, `Leaf` is `Subgroup`, and `Data.Element` is `Parent.TableRowValue`.

Show all declarations

## Parameters 

`data`  

A collection of tree-structured, identified data.

`children`  

A key path to a property whose non-`nil` value gives the children of `data`. A non-`nil` but empty value denotes an element capable of having children that’s currently childless, such as an empty directory in a file system. On the other hand, if the property at the key path is `nil`, then the outline group treats `data` as a leaf in the tree, like a regular file in a file system.

## Discussion

This initializer provides a default `TableRowBuilder` using `TableRow` for each data element.

This initializer creates an instance that uniquely identifies table rows across updates based on the identity of the underlying data element.

All generated disclosure groups begin in the collapsed state.

## See Also

### Creating an outline group

init(_:children:content:)

Creates an outline group from a binding to a collection of root data elements and a key path to its children.

init(_:id:children:content:)

Creates an outline group from a binding to a collection of root data elements, the key path to a data element’s identifier, and a key path to its children.

