

- UIKit
- UIViewController
-  loadView() 

Instance Method

# loadView()

Creates the view that the controller manages.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func loadView()
```

## Discussion

You should never call this method directly. The view controller calls this method when its view property is requested but is currently `nil`. This method loads or creates a view and assigns it to the view property.

If the view controller has an associated nib file, this method loads the view from the nib file. A view controller has an associated nib file if the nibName property returns a non-`nil` value, which occurs if the view controller was instantiated from a storyboard, if you explicitly assigned it a nib file using the init(nibName:bundle:) method, or if iOS finds a nib file in the app bundle with a name based on the view controller’s class name. If the view controller does not have an associated nib file, this method creates a plain UIView object instead.

If you use Interface Builder to create your views and initialize the view controller, you must not override this method.

You can override this method in order to create your views manually. If you choose to do so, assign the root view of your view hierarchy to the view property. The views you create should be unique instances and should not be shared with any other view controller object. Your custom implementation of this method should not call `super`.

If you want to perform any additional initialization of your views, do so in the viewDidLoad() method.

## See Also

### Related Documentation

var nibName: String?

The name of the view controller’s nib file, if one was specified.

### Managing the view

var view: UIView!

The view that the controller manages.

var viewIfLoaded: UIView?

The view controller’s view, or `nil` if the view isn’t yet loaded.

var isViewLoaded: Bool

A Boolean value indicating whether the view is currently loaded into memory.

func viewDidLoad()

Called after the controller’s view is loaded into memory.

func loadViewIfNeeded()

Loads the view controller’s view if it’s not loaded yet.

var title: String?

A localized string that represents the view this controller manages.

var preferredContentSize: CGSize

The preferred size for the view controller’s view.

