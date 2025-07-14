

- WatchKit
- WKInterfaceController
-  table(\_:didSelectRowAt:) 

Instance Method

# table(\_:didSelectRowAt:)

Called to let you know that the user selected a row in the table.

watchOS 2.0+

``` source
@MainActor
func table(
    _ table: WKInterfaceTable,
    didSelectRowAt rowIndex: Int
)
```

## Parameters 

`table`  

The table object whose row was selected.

`rowIndex`  

The zero-based index of the row that was selected.

## Discussion

Use this method to respond to row selections in a table. You might use the selection of a row to display a new interface controller or update the state of your app. If you connected an action method to the table in your storyboard file, WatchKit does not call this method.

This method is called on your WatchKit extension’s main thread. Implementation of the method is optional.

