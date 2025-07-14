

- SwiftUI
- DynamicViewContent
-  onMove(perform:) 

Instance Method

# onMove(perform:)

Sets the move action for the dynamic view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func onMove(perform action: Optional Void>) -> some DynamicViewContent
```

## Parameters 

`action`  

A closure that SwiftUI invokes when elements in the dynamic view are moved. The closure takes two arguments that represent the offset relative to the dynamic view’s underlying collection of data. Pass `nil` to disable the ability to move items.

## Return Value

A view that calls `action` when elements are moved within the original view.

## See Also

### Responding to updates

func onDelete(perform: Optional&lt;(IndexSet) -> Void>) -> some DynamicViewContent

Sets the deletion action for the dynamic view. You must delete the corresponding item within `action`, as it will be called after the row has already been removed from the List.

func onInsert(of: [UTType], perform: (Int, [NSItemProvider]) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

func dropDestination&lt;T>(for: T.Type, action: ([T], Int) -> Void) -> some DynamicViewContent

Sets the insert action for the dynamic view.

