

- AppKit
- NSViewController
-  updateViewConstraints() 

Instance Method

# updateViewConstraints()

Called during Auto Layout constraint updating to enable the view controller to mediate the process.

macOS 10.10+

``` source
@MainActor
func updateViewConstraints()
```

## Discussion

This method gets called, for example, when the user interacts with a view in a way that causes the layout to change. When called, the default implementation of this method in turn calls the updateConstraints() method on the view controller’s view.

You can override this method to update custom view constraints, as an alternative to subclassing the view controller’s view and overriding its updateConstraints() method.

If you override this method, you must call this method on `super` at some point in your implementation or call the updateConstraints() method on the view controller’s view.

This method is called only for apps that link against macOS 10.10 or later.

## See Also

### Managing View Layout

var preferredContentSize: NSSize

The desired size of the view controller’s view, in screen units.

func viewWillLayout()

Called just before the layout() method of the view controller’s view is called.

func viewDidLayout()

Called immediately after the layout() method of the view controller’s view is called.

