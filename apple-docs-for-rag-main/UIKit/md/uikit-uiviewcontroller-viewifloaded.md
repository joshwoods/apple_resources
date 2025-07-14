

- UIKit
- UIViewController
-  viewIfLoaded 

Instance Property

# viewIfLoaded

The view controller’s view, or `nil` if the view isn’t yet loaded.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var viewIfLoaded: UIView? { get }
```

## Discussion

If the view controller’s view has already been loaded, this property contains that view. If the view has not yet been loaded, this property is set to `nil`.

## See Also

### Managing the view

var view: UIView!

The view that the controller manages.

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

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

