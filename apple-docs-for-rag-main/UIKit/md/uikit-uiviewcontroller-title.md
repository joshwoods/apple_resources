

- UIKit
- UIViewController
-  title 

Instance Property

# title

A localized string that represents the view this controller manages.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var title: String? { get set }
```

## Discussion

Set the title to a human-readable string that describes the view. If the view controller has a valid navigation item or tab-bar item, assigning a value to this property updates the title text of those objects.

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

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

