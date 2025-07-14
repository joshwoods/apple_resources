

- WatchKit
- WKInterfaceController
-  contextForSegue(withIdentifier:) 

Instance Method

# contextForSegue(withIdentifier:)

Returns the context object to pass to the specified interface controller when a button is tapped.

watchOS 2.0+

``` source
@MainActor
func contextForSegue(withIdentifier segueIdentifier: String) -> Any?
```

## Parameters 

`segueIdentifier`  

The identifier of the segue that was triggered. When configuring your interface, specify the identifier for a segue in the Attributes inspector.

## Return Value

The object to pass to the new interface controller. Use this object to communicate important information to the new interface controller, such as the data to be displayed or any relevant state information. You may return `nil` if you want, but doing so is not recommended.

## Mentioned in 

Navigating Between Scenes

## Discussion

When you create a segue from a button to a single interface controller, the system calls this method when that segue is triggered. Use this method to provide the new interface controller with any contextual data it needs to display its content. The object you return is passed directly to the new interface controller’s awake(withContext:) method.

WatchKit calls this method on your WatchKit extension’s main thread. Implementation of this method is optional but is recommended if you use segues in your storyboard file. You do not need to call `super` in your implementation. For segues originating from a table row, use the contextForSegue(withIdentifier:in:rowIndex:) method instead.

## See Also

### Managing segue-based transitions

func contextsForSegue(withIdentifier: String) -> [Any]?

Returns the context objects to pass to a page-based set of interface controllers when a button is tapped.

func contextForSegue(withIdentifier: String, in: WKInterfaceTable, rowIndex: Int) -> Any?

Returns the context object to pass to the specified interface controller when a row in a table is tapped.

func contextsForSegue(withIdentifier: String, in: WKInterfaceTable, rowIndex: Int) -> [Any]?

Returns the context objects to pass to a page-based set of interface controllers when a row in a table is tapped.

