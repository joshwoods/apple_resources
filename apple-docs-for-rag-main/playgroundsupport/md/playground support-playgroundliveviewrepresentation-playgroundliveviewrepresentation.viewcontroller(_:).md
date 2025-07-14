

- Playground Support
- PlaygroundLiveViewRepresentation
-  PlaygroundLiveViewRepresentation.viewController(\_:) 

Enumeration Case

# PlaygroundLiveViewRepresentation.viewController(\_:)

An AppKit view controller whose view is displayed as the live view.

macOS 11.0+Xcode 12.0+

``` source
case viewController(NSViewController)
```

## Discussion

This view controller must be the root of a view controller hierarchy (it must not have a parent view controller), and its view must not have a superview.

## See Also

### Displaying AppKit Views

case view(NSView)

An AppKit view that's displayed as the live view.

