

- AppKit
- NSView
-  viewDidChangeBackingProperties() 

Instance Method

# viewDidChangeBackingProperties()

Responds when the view’s backing store properties change.

macOS 10.7+

``` source
@MainActor
func viewDidChangeBackingProperties()
```

## Discussion

The view gets this message when the backing store scale or color space changes. Provide an implementation if you need to swap assets or make other adjustments when a view’s backing store properties change.

## See Also

### Responding to Appearance Changes

func viewDidChangeEffectiveAppearance()

Informs the view that its effective appearance changed.

