

- UIKit
- UIStoryboardUnwindSegueSource
-  sender 

Instance Property

# sender

The object that performed the unwind action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var sender: Any? { get }
```

## Discussion

Use this property to determine which object in your interface triggered the unwind segue.

## See Also

### Getting the unwind segue attributes

var source: UIViewController

The view controller being dismissed by the unwind segue.

var unwindAction: Selector

The action method associated with the unwind segue.

