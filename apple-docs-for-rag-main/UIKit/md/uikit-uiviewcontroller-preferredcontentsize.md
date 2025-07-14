

- UIKit
- UIViewController
-  preferredContentSize 

Instance Property

# preferredContentSize

The preferred size for the view controller’s view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var preferredContentSize: CGSize { get set }
```

## Discussion

The value in this property is used primarily when displaying the view controller’s content in a popover but may also be used in other situations. Changing the value of this property while the view controller is being displayed in a popover animates the size change; however, the change is not animated if you specify a width or height of `0.0`.

## See Also

### Managing the view

var view: UIView!

The view that the controller manages.

var viewIfLoaded: UIView?

The view controller’s view, or `nil` if the view isn’t yet loaded.

var isViewLoaded: Bool

A Boolean value indicating whether the view is currently loaded into memory.

func loadView()

Creates the view that the controller manages.

func viewDidLoad()

Called after the controller’s view is loaded into memory.

func loadViewIfNeeded()

Loads the view controller’s view if it’s not loaded yet.

var title: String?

A localized string that represents the view this controller manages.

