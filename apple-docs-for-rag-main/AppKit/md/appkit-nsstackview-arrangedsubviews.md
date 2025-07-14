

- AppKit
- NSStackView
-  arrangedSubviews 

Instance Property

# arrangedSubviews

The array of views arranged by the stack view.

macOS 10.11+

``` source
@MainActor
var arrangedSubviews: [NSView] { get }
```

## Discussion

The stack view ensures that the contents of this array are always a subset of its subviews array.

## See Also

### Managing the Arranged Subviews

func addArrangedSubview(NSView)

Adds the specified view to the end of the arranged subviews list.

func insertArrangedSubview(NSView, at: Int)

Adds the provided view to the array of arranged subviews at the specified index.

func removeArrangedSubview(NSView)

Removes the provided view from the stack’s array of arranged subviews.

