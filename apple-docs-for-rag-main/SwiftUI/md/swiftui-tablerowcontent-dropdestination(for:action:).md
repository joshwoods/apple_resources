

- SwiftUI
- TableRowContent
-  dropDestination(for:action:) 

Instance Method

# dropDestination(for:action:)

Defines the entire row as a destination of a drag and drop operation that handles the dropped content with a closure that you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func dropDestination(
    for payloadType: T.Type = T.self,
    action: @escaping ([T]) -> Void
) -> some TableRowContent where T : Transferable
```

## Parameters 

`payloadType`  

The expected type of the dropped models.

`action`  

A closure that takes the dropped content and responds with `true` if the drop operation was successful; otherwise, return `false`.

## Return Value

A row that provides a drop destination for a drag operation of the specified type.

## See Also

### Managing interaction

func draggable&lt;T>(@autoclosure () -> T) -> some TableRowContent&lt;Self.TableRowValue> 

Activates this row as the source of a drag and drop operation.

func onHover(perform: (Bool) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Adds an action to perform when the pointer moves onto or away from the entire row.

func itemProvider((() -> NSItemProvider?)?) -> ModifiedContent&lt;Self, ItemProviderTableRowModifier>

Provides a closure that vends the drag representation for a particular data element.

struct ItemProviderTableRowModifier

A table row modifier that associates an item provider with some base row content.

