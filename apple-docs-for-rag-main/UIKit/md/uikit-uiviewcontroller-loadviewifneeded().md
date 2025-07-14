

- UIKit
- UIViewController
-  loadViewIfNeeded() 

Instance Method

# loadViewIfNeeded()

Loads the view controller’s view if it’s not loaded yet.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func loadViewIfNeeded()
```

## Discussion

Calling this method loads the view controller’s view from its storyboard file, or creates the view as needed based on the established rules.

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

var title: String?

A localized string that represents the view this controller manages.

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

