

- SwiftUI
- DynamicViewContent
-  onInsert(of:perform:) 

Instance Method

# onInsert(of:perform:)

Sets the insert action for the dynamic view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func onInsert(
    of supportedContentTypes: [UTType],
    perform action: @escaping (Int, [NSItemProvider]) -> Void
) -> some DynamicViewContent
```

Show all declarations

## Parameters 

`supportedContentTypes`  

An array of UTI types that the dynamic view supports.

`action`  

A closure that SwiftUI invokes when elements are added to the view. The closure takes two arguments: The first argument is the offset relative to the dynamic view’s underlying collection of data. The second argument is an array of NSItemProvider items that represents the data that you want to insert.

## Return Value

A view that calls `action` when elements are inserted into the original view.

