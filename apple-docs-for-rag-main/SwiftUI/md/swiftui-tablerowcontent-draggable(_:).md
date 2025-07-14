

- SwiftUI
- TableRowContent
-  draggable(\_:) 

Instance Method

# draggable(\_:)

Activates this row as the source of a drag and drop operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func draggable(_ payload: @autoclosure @escaping () -> T) -> some TableRowContent where T : Transferable
```

## Parameters 

`payload`  

A closure that returns a single instance or a value conforming to Transferable that represents the draggable data from this view.

## Return Value

A row that activates this row as the source of a drag and drop operation.

## Discussion

Applying the `draggable(_:)` modifier adds the appropriate gestures for drag and drop to this row.

## See Also

### Managing interaction

func dropDestination&lt;T>(for: T.Type, action: ([T]) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Defines the entire row as a destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func onHover(perform: (Bool) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Adds an action to perform when the pointer moves onto or away from the entire row.

func itemProvider((() -> NSItemProvider?)?) -> ModifiedContent&lt;Self, ItemProviderTableRowModifier>

Provides a closure that vends the drag representation for a particular data element.

struct ItemProviderTableRowModifier

A table row modifier that associates an item provider with some base row content.

