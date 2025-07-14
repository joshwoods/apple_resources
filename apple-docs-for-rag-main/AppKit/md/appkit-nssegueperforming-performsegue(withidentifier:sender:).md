

- AppKit
- NSSeguePerforming
-  performSegue(withIdentifier:sender:) 

Instance Method

# performSegue(withIdentifier:sender:)

Performs the specified segue.

macOS 10.10+

``` source
@MainActor
optional func performSegue(
    withIdentifier identifier: NSStoryboardSegue.Identifier,
    sender: Any?
)
```

## Parameters 

`identifier`  

The string that uniquely identifies the segue in the storyboard file.

In Interface Builder, you can provide an identifier string to a segue using the inspector. Pass this string to this parameter.

Note

This method throws an Exception handling if there is no segue with the specified identifier or if the identifier is `nil`.

`sender`  

The object that you want to use to initiate the segue. This parameter makes the object available to your implementation during the segue.

## Discussion

Apps typically do not need to trigger segues programmatically. If needed, you can call this method to trigger a segue for an action that cannot be expressed in a storyboard file, such as a transition between scenes in different storyboards.

Typically, a segue is triggered by a user action, such as clicking a button. In Interface Builder, configure an object, such as a control embedded in the view controller’s view hierarchy, to trigger the segue.

## See Also

### Working with Storyboard Segues

func prepare(for: NSStoryboardSegue, sender: Any?)

Called when a segue is about to be performed.

func shouldPerformSegue(withIdentifier: NSStoryboardSegue.Identifier, sender: Any?) -> Bool

Called immediately prior to the performance of a storyboard segue.

