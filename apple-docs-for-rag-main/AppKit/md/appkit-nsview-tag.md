

- AppKit
- NSView
-  tag 

Instance Property

# tag

The view’s tag, which is an integer that you use to identify the view within your app.

macOS

``` source
@MainActor
var tag: Int { get }
```

## Discussion

The default value of this property is `–1`. Subclasses can override this property to provide individual tags for views, possibly redefining the property as `readwrite` so that you can modify it more easily.

## See Also

### Identifying Views by Tag

func viewWithTag(Int) -> NSView?

Returns the view’s nearest descendant (including itself) with a specific tag, or `nil` if no subview has that tag.

