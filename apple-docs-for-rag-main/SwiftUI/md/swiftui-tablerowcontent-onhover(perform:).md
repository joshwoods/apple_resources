

- SwiftUI
- TableRowContent
-  onHover(perform:) 

Instance Method

# onHover(perform:)

Adds an action to perform when the pointer moves onto or away from the entire row.

macOS 14.0+

``` source
@MainActor @preconcurrency
func onHover(perform action: @escaping (Bool) -> Void) -> some TableRowContent
```

## See Also

### Managing interaction

func draggable&lt;T>(@autoclosure () -> T) -> some TableRowContent&lt;Self.TableRowValue> 

Activates this row as the source of a drag and drop operation.

func dropDestination&lt;T>(for: T.Type, action: ([T]) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Defines the entire row as a destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func itemProvider((() -> NSItemProvider?)?) -> ModifiedContent&lt;Self, ItemProviderTableRowModifier>

Provides a closure that vends the drag representation for a particular data element.

struct ItemProviderTableRowModifier

A table row modifier that associates an item provider with some base row content.

