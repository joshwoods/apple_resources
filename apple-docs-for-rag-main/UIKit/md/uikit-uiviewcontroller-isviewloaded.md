

- UIKit
- UIViewController
-  isViewLoaded 

Instance Property

# isViewLoaded

A Boolean value indicating whether the view is currently loaded into memory.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isViewLoaded: Bool { get }
```

## Discussion

The value of this property is true when the view is in memory or false when it is not. Accessing this property does not attempt to load the view if it is not currently in memory.

## See Also

### Managing the view

var view: UIView!

The view that the controller manages.

var viewIfLoaded: UIView?

The view controller’s view, or `nil` if the view isn’t yet loaded.

func loadView()

Creates the view that the controller manages.

func viewDidLoad()

Called after the controller’s view is loaded into memory.

func loadViewIfNeeded()

Loads the view controller’s view if it’s not loaded yet.

var title: String?

A localized string that represents the view this controller manages.

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

