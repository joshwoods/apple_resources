

- UIKit
- UISplitViewController
-  delegate 

Instance Property

# delegate

The delegate you use to manage changes to a split view interface.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
weak var delegate: (any UISplitViewControllerDelegate)? { get set }
```

## Discussion

The split view controller uses its delegate to manage showing and hiding related view controllers. For more information about the methods you can implement in your delegate, see UISplitViewControllerDelegate.

## See Also

### Customizing the split view transitions

protocol UISplitViewControllerDelegate

The methods adopted by the object you use to manage changes to a split view interface.

