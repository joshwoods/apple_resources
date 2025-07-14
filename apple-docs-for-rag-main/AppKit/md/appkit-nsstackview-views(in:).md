

- AppKit
- NSStackView
-  views(in:) 

Instance Method

# views(in:)

Returns the array of views in the specified gravity area in the stack view.

macOS

``` source
@MainActor
func views(in gravity: NSStackView.Gravity) -> [NSView]
```

## Parameters 

`gravity`  

The gravity area whose view array you want to get. Valid values are those in the NSStackView.Gravity enumeration, according to the stack view’s layout direction..

## Return Value

The array of views in a specified gravity area.

## Discussion

The returned array contains all of the views in the specified gravity area of the stack view, regardless of whether they are attached. The index position of each view in the array matches the view ordering within the gravity area. A detached view’s index position is its gravity area position when attached.

## See Also

### Inspecting a Stack View

var views: [NSView]

The array of views owned by the stack view.

var detachedViews: [NSView]

An array that contains the detached views from all the stack view’s gravity areas.

func clippingResistancePriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for resisting clipping of views in the stack view when Auto Layout attempts to reduce the stack view’s size.

func huggingPriority(for: NSLayoutConstraint.Orientation) -> NSLayoutConstraint.Priority

Returns the Auto Layout priority for the stack view to minimize its size to fit its contained views as closely as possible, for a specified user interface axis.

