

- AppKit
- NSStackView
-  removeView(\_:) 

Instance Method

# removeView(\_:)

Removes a specified view from the stack view.

macOS

``` source
@MainActor
func removeView(_ view: NSView)
```

## Parameters 

`view`  

The view you want to remove from the stack view.

Important

If you attempt to remove a view that is not in the stack view, the system raises an exception.

## Discussion

This method removes a view from a stack view whether the view is attached or detached. For an attached view only, you can alternatively call the removeFromSuperview() method on the view.

## See Also

### Managing Views in Gravity Areas

func addView(NSView, in: NSStackView.Gravity)

Adds a view to the end of the stack view gravity area.

func insertView(NSView, at: Int, in: NSStackView.Gravity)

Adds a view to a stack view gravity area at a specified index position.

func setViews([NSView], in: NSStackView.Gravity)

Specifies an array of views for a specified gravity area in the stack view, replacing any previous views in that area.

enum Gravity

The gravity areas available in a stack view.

