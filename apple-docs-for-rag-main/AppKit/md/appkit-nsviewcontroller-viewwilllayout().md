

- AppKit
- NSViewController
-  viewWillLayout() 

Instance Method

# viewWillLayout()

Called just before the layout() method of the view controller’s view is called.

macOS 10.10+

``` source
@MainActor
func viewWillLayout()
```

## Discussion

You can override this method to perform tasks to precede the layout of the view controller’s view, such as adjusting Auto Layout constraints. If you override this method, call this method on `super` at some point in your implementation in case a superclass also overrides this method.

The default implementation of this method does nothing.

## See Also

### Managing View Layout

var preferredContentSize: NSSize

The desired size of the view controller’s view, in screen units.

func updateViewConstraints()

Called during Auto Layout constraint updating to enable the view controller to mediate the process.

func viewDidLayout()

Called immediately after the layout() method of the view controller’s view is called.

