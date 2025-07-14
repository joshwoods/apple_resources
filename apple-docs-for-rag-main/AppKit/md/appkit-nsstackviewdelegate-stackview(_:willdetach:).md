

- AppKit
- NSStackViewDelegate
-  stackView(\_:willDetach:) 

Instance Method

# stackView(\_:willDetach:)

Called when the stack view is about to automatically detach one or more of its views.

macOS 10.9+

``` source
@MainActor
optional func stackView(
    _ stackView: NSStackView,
    willDetach views: [NSView]
)
```

## Parameters 

`stackView`  

The stack view that is about to detach one or more of its views.

`views`  

An array of one or more views, managed by the stack view, that are about to be automatically detached.

## Discussion

To configure a custom class to respond to the automatic detachment of views from a stack view’s view hierarchy, implement this method in the class. This method is not called when your code explicitly removes a view from a stack view’s views array.

## See Also

### Responding to View Detachment and Reattachment

func stackView(NSStackView, didReattach: [NSView])

Called when the stack view has automatically reattached one or more previously-detached views.

