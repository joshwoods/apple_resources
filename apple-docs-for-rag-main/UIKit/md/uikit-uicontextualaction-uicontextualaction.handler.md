

- UIKit
- UIContextualAction
-  UIContextualAction.Handler 

Type Alias

# UIContextualAction.Handler

The handler block to call in response to the selection of an action.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
typealias Handler = (UIContextualAction, UIView, @escaping (Bool) -> Void) -> Void
```

## Parameters 

`action`  

The object containing information about the selected action.

`sourceView`  

The view in which the action was displayed.

`completionHandler`  

The handler block for you to execute after you have performed the action. This block has no return value and takes the following parameter:

actionPerformed  
A Boolean value indicating whether you performed the action. Specify true if you performed the action or false if you were unable to perform the action for some reason.

## See Also

### Getting the configuration details

var handler: UIContextualAction.Handler

The handler block to execute when the user selects the action.

var style: UIContextualAction.Style

The style that applies to the action button.

enum Style

Constants indicating the style information that applies to the action button.

