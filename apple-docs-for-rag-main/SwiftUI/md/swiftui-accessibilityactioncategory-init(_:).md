

- SwiftUI
- AccessibilityActionCategory
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom action category labeled by `name`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(_ name: Text)
```

Show all declarations

## Discussion

Extension AccessibilityActionCategory { static let table = AccessibilityActionCategory(“Table Options”) }

var body: some View { TableCellView() .accessibilityActions(category: .table) { ForEach(tableCellActions) { action in Button(action.title) { action() } } } }

- Parameter:

  - name: The name for the category of the accessibility actions.

