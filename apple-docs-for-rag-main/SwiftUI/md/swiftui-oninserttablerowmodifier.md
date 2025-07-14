

- SwiftUI
-  OnInsertTableRowModifier 

Structure

# OnInsertTableRowModifier

A table row modifier that adds the ability to insert data in some base row content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
struct OnInsertTableRowModifier
```

## Topics

### Instance Properties

var body: some _TableRowContentModifier

### Type Aliases

typealias Body

## See Also

### Inserting rows

func onInsert(of: [UTType], perform: (Int, [NSItemProvider]) -> Void) -> ModifiedContent&lt;Self, OnInsertTableRowModifier>

Sets the insert action for the dynamic table rows.

