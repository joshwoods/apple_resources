

- Core Foundation
-  CFTreeRemoveAllChildren(\_:) 

Function

# CFTreeRemoveAllChildren(\_:)

Removes all the children of a tree.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeRemoveAllChildren(_ tree: CFTree!)
```

## Parameters 

`tree`  

The tree to modify.

## See Also

### Modifying a Tree

func CFTreeAppendChild(CFTree!, CFTree!)

Adds a new child to a tree as the last in its list of children.

func CFTreeInsertSibling(CFTree!, CFTree!)

Inserts a new sibling after a given tree.

func CFTreePrependChild(CFTree!, CFTree!)

Adds a new child to the specified tree as the first in its list of children.

func CFTreeRemove(CFTree!)

Removes a tree from its parent.

func CFTreeSetContext(CFTree!, UnsafePointer&lt;CFTreeContext>!)

Replaces the context of a tree by releasing the old information pointer and retaining the new one.

