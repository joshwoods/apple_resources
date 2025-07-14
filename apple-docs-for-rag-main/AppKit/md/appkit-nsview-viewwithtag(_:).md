

- AppKit
- NSView
-  viewWithTag(\_:) 

Instance Method

# viewWithTag(\_:)

Returns the view’s nearest descendant (including itself) with a specific tag, or `nil` if no subview has that tag.

macOS

``` source
@MainActor
func viewWithTag(_ tag: Int) -> NSView?
```

## Parameters 

`tag`  

An integer identifier associated with a view object.

## See Also

### Identifying Views by Tag

var tag: Int

The view’s tag, which is an integer that you use to identify the view within your app.

