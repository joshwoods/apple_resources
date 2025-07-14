

- AppKit
- NSViewController
-  storyboard 

Instance Property

# storyboard

The storyboard from which the view controller was loaded.

macOS 10.10+

``` source
@MainActor
var storyboard: NSStoryboard? { get }
```

## Discussion

If the view controller was not loaded from a storyboard, the value of this property is `nil`.

## See Also

### Using a Storyboard

func dismiss(Any?)

