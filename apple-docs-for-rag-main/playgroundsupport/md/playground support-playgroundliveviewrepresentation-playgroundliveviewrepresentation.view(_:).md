

- Playground Support
- PlaygroundLiveViewRepresentation
-  PlaygroundLiveViewRepresentation.view(\_:) 

Enumeration Case

# PlaygroundLiveViewRepresentation.view(\_:)

An AppKit view that's displayed as the live view.

macOS 11.0+Xcode 12.0+

``` source
case view(NSView)
```

## Discussion

This view must be the root of a view hierarchy (it must not have a superview), and it must not be owned by a view controller.

## See Also

### Displaying AppKit Views

case viewController(NSViewController)

An AppKit view controller whose view is displayed as the live view.

