

- UIKit
- UIStoryboardUnwindSegueSource
-  source 

Instance Property

# source

The view controller being dismissed by the unwind segue.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var source: UIViewController { get }
```

## See Also

### Getting the unwind segue attributes

var unwindAction: Selector

The action method associated with the unwind segue.

var sender: Any?

The object that performed the unwind action.

