

- AppKit
- NSText
-  isRulerVisible 

Instance Property

# isRulerVisible

A Boolean value that indicates whether the receiver’s enclosing scroll view shows its ruler.

macOS

``` source
@MainActor
var isRulerVisible: Bool { get }
```

## Discussion

true if the receiver’s enclosing scroll view shows its ruler, otherwise false.

## See Also

### Using the ruler

func toggleRuler(Any?)

This action method shows or hides the ruler, if the receiver is enclosed in a scroll view.

