

- UIKit
- UIStoryboardUnwindSegueSource
-  unwindAction 

Instance Property

# unwindAction

The action method associated with the unwind segue.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var unwindAction: Selector { get }
```

## Discussion

Each unwind segue has an associated action method. The view controller that’s the destination of the unwind segue must implement this action method.

## See Also

### Getting the unwind segue attributes

var source: UIViewController

The view controller being dismissed by the unwind segue.

var sender: Any?

The object that performed the unwind action.

