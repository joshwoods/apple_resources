

- SwiftUI
- DynamicViewContent
-  onDelete(perform:) 

Instance Method

# onDelete(perform:)

Sets the deletion action for the dynamic view. You must delete the corresponding item within `action`, as it will be called after the row has already been removed from the List.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func onDelete(perform action: Optional Void>) -> some DynamicViewContent
```

## Parameters 

`action`  

The action that you want SwiftUI to perform when elements in the view are deleted. SwiftUI passes a set of indices to the closure that’s relative to the dynamic view’s underlying collection of data.

## Return Value

A view that calls `action` when elements are deleted from the original view.

## Mentioned in 

Picking container views for your content

## See Also

### Responding to updates

func onInsert(of: [UTType], perform: (Int, [NSItemProvider]) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

func onMove(perform: Optional&lt;(IndexSet, Int) -> Void>) -> some DynamicViewContent

Sets the move action for the dynamic view.

func dropDestination&lt;T>(for: T.Type, action: ([T], Int) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

