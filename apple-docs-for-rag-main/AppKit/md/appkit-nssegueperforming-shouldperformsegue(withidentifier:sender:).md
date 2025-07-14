

- AppKit
- NSSeguePerforming
-  shouldPerformSegue(withIdentifier:sender:) 

Instance Method

# shouldPerformSegue(withIdentifier:sender:)

Called immediately prior to the performance of a storyboard segue.

macOS 10.10+

``` source
@MainActor
optional func shouldPerformSegue(
    withIdentifier identifier: NSStoryboardSegue.Identifier,
    sender: Any?
) -> Bool
```

## Parameters 

`identifier`  

The string that identifies the segue to be performed.

Using the Interface Builder inspector, provide a unique identifier string for each segue in a storyboard. The system provides a segue’s identifier to this parameter when it calls this method. The identifier string is used to locate the segue inside the storyboard file that contains the view controller.

Note

This method throws an Exception handling if there is no segue with the specified identifier.

`sender`  

The object that initiated the segue. This object is made available for informational purposes during the segue.

## Return Value

true to allow a segue to proceed or false to stop it from proceeding.

## Discussion

Override this method to return false for cases where you want to prevent the performance of a segue. By default, invocation of a segue results in the segue being performed.

## See Also

### Working with Storyboard Segues

func performSegue(withIdentifier: NSStoryboardSegue.Identifier, sender: Any?)

Performs the specified segue.

func prepare(for: NSStoryboardSegue, sender: Any?)

Called when a segue is about to be performed.

