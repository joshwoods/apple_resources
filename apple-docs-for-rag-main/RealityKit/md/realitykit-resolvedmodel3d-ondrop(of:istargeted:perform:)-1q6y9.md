

- RealityKit
- ResolvedModel3D
-  onDrop(of:isTargeted:perform:) 

Instance Method

# onDrop(of:isTargeted:perform:)

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+macOS 11.0+visionOS

``` source
nonisolated
func onDrop(
    of supportedContentTypes: [UTType],
    isTargeted: Binding?,
    perform action: @escaping ([NSItemProvider], CGPoint) -> Bool
) -> some View
```

## Parameters 

`supportedContentTypes`  

The uniform type identifiers that describe the types of content this view can accept through drag and drop. If the drag and drop operation doesn’t contain any of the supported types, then this drop destination doesn’t activate and `isTargeted` doesn’t update.

`isTargeted`  

A binding that updates when a drag and drop operation enters or exits the drop target area. The binding’s value is `true` when the cursor is inside the area, and `false` when the cursor is outside.

`action`  

A closure that takes the dropped content and responds appropriately. The first parameter to `action` contains the dropped items, with types specified by `supportedContentTypes`. The second parameter contains the drop location in this view’s coordinate space. Return `true` if the drop operation was successful; otherwise, return `false`.

## Return Value

A view that provides a drop destination for a drag operation of the specified types.

## Discussion

The drop destination is the same size and position as this view.

