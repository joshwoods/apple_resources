

- SwiftUI
- TableRowContent
-  itemProvider(\_:) 

Instance Method

# itemProvider(\_:)

Provides a closure that vends the drag representation for a particular data element.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func itemProvider(_ action: (() -> NSItemProvider?)?) -> ModifiedContent
```

## See Also

### Managing interaction

func draggable&lt;T>(@autoclosure () -> T) -> some TableRowContent&lt;Self.TableRowValue> 

Activates this row as the source of a drag and drop operation.

func dropDestination&lt;T>(for: T.Type, action: ([T]) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Defines the entire row as a destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func onHover(perform: (Bool) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Adds an action to perform when the pointer moves onto or away from the entire row.

struct ItemProviderTableRowModifier

A table row modifier that associates an item provider with some base row content.

