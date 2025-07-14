

- UIKit
- UIViewController
-  storyboard 

Instance Property

# storyboard

The storyboard from which the view controller originated.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var storyboard: UIStoryboard? { get }
```

## Discussion

If the view controller was not instantiated from a storyboard, this property is `nil`.

## See Also

### Getting the storyboard and nib information

var nibName: String?

The name of the view controller’s nib file, if one was specified.

var nibBundle: Bundle?

The view controller’s nib bundle if it exists.

