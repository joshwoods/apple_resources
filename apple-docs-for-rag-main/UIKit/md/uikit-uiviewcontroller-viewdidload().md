

- UIKit
- UIViewController
-  viewDidLoad() 

Instance Method

# viewDidLoad()

Called after the controller’s view is loaded into memory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func viewDidLoad()
```

## Mentioned in 

Displaying and managing views with a view controller

Customizing a document-based app’s launch experience

Making a view into a drag source

## Discussion

This method is called after the view controller has loaded its view hierarchy into memory. This method is called regardless of whether the view hierarchy was loaded from a nib file or created programmatically in the loadView() method. You usually override this method to perform additional initialization on views that were loaded from nib files.

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

func loadViewIfNeeded()

Loads the view controller’s view if it’s not loaded yet.

var title: String?

A localized string that represents the view this controller manages.

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

