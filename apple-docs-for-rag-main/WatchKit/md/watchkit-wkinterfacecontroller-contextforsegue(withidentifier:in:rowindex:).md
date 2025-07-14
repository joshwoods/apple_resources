

- WatchKit
- WKInterfaceController
-  contextForSegue(withIdentifier:in:rowIndex:) 

Instance Method

# contextForSegue(withIdentifier:in:rowIndex:)

Returns the context object to pass to the specified interface controller when a row in a table is tapped.

watchOS 2.0+

``` source
@MainActor
func contextForSegue(
    withIdentifier segueIdentifier: String,
    in table: WKInterfaceTable,
    rowIndex: Int
) -> Any?
```

## Parameters 

`segueIdentifier`  

The identifier of the segue that was triggered. Specify the identifier for a segue in the Attributes inspector when configuring your interface.

`table`  

The table object containing the row that was tapped.

`rowIndex`  

The zero-based index of the row that was tapped by the user.

## Return Value

The object to pass to the new interface controller. Use this object to communicate important information to the new interface controller, such as the data to display or any relevant state information. You may specify `nil` if you want, but doing so is not recommended.

## Discussion

WatchKit calls this method when a segue attached to a table row is triggered. Use this method to provide the new interface controller with any contextual data it needs to display its content. The object you return is passed directly to the new interface controller’s awake(withContext:) method.

This method is called on your WatchKit extension’s main thread. Implementation of this method is optional but is recommended if you use segues in your storyboard file. You do not need to call `super` in your implementation. For segues originating from a button, use the contextsForSegue(withIdentifier:) method instead.

## See Also

### Managing segue-based transitions

func contextForSegue(withIdentifier: String) -> Any?

Returns the context object to pass to the specified interface controller when a button is tapped.

func contextsForSegue(withIdentifier: String) -> [Any]?

Returns the context objects to pass to a page-based set of interface controllers when a button is tapped.

func contextsForSegue(withIdentifier: String, in: WKInterfaceTable, rowIndex: Int) -> [Any]?

Returns the context objects to pass to a page-based set of interface controllers when a row in a table is tapped.

