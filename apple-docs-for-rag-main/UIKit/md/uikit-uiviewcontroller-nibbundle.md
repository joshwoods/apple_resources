

- UIKit
- UIViewController
-  nibBundle 

Instance Property

# nibBundle

The view controller’s nib bundle if it exists.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var nibBundle: Bundle? { get }
```

## See Also

### Related Documentation

init(nibName: String?, bundle: Bundle?)

Creates a view controller with the nib file in the specified bundle.

### Getting the storyboard and nib information

var storyboard: UIStoryboard?

The storyboard from which the view controller originated.

var nibName: String?

The name of the view controller’s nib file, if one was specified.

