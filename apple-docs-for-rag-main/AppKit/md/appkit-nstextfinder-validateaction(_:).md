

- AppKit
- NSTextFinder
-  validateAction(\_:) 

Instance Method

# validateAction(\_:)

Allows validation of the find action before performing.

macOS 10.7+

``` source
func validateAction(_ op: NSTextFinder.Action) -> Bool
```

## Parameters 

`op`  

The sender’s tag.

## Return Value

true if the operation is valid; otherwise false.

## Discussion

Responders the `NSResponder` method performTextFinderAction(_:) should call this method.

This method should be called by an implementation of validateUserInterfaceItem(_:) to properly validate items with an action of performTextFinderAction(_:). The responder’s validateUserInterfaceItem(_:) or validateMenuItem: implementation should pass the tag as the action for this method..

## See Also

### Validating and Performing Text Finding

func performAction(NSTextFinder.Action)

Performs the specified text finding action.

func cancelFindIndicator()

Cancels the find indicator immediately.

