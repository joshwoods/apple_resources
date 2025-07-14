

- AppKit
- NSStackViewDelegate
-  stackView(\_:didReattach:) 

Instance Method

# stackView(\_:didReattach:)

Called when the stack view has automatically reattached one or more previously-detached views.

macOS 10.9+

``` source
@MainActor
optional func stackView(
    _ stackView: NSStackView,
    didReattach views: [NSView]
)
```

## Parameters 

`stackView`  

The stack view that has reattached one or more detached views.

`views`  

An array of one or more views, managed by the stack view, that were reattached.

## Discussion

To configure a custom class to respond to the automatic reattachment of views to a stack view’s view hierarchy, implement this method in the class. This method is not called when your code explicitly adds a view to a stack view’s views array.

## See Also

### Responding to View Detachment and Reattachment

func stackView(NSStackView, willDetach: [NSView])

Called when the stack view is about to automatically detach one or more of its views.

