

- AppKit
- NSViewController
-  viewDidLayout() 

Instance Method

# viewDidLayout()

Called immediately after the layout() method of the view controller’s view is called.

macOS 10.10+

``` source
@MainActor
func viewDidLayout()
```

## Discussion

You can override this method to perform tasks to follow the completion of layout of the view controller’s view. If you override this method, call this method on `super` at some point in your implementation in case a superclass also overrides this method.

The default implementation of this method does nothing.

## See Also

### Managing View Layout

var preferredContentSize: NSSize

The desired size of the view controller’s view, in screen units.

func updateViewConstraints()

Called during Auto Layout constraint updating to enable the view controller to mediate the process.

func viewWillLayout()

Called just before the layout() method of the view controller’s view is called.

