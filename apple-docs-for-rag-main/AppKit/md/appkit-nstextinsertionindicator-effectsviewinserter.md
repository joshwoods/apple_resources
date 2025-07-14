

- AppKit
- NSTextInsertionIndicator
-  effectsViewInserter 

Instance Property

# effectsViewInserter

An optional closure the system calls during dictation.

macOS 14.0+

``` source
@MainActor
var effectsViewInserter: ((NSView) -> Void)? { get set }
```

## Mentioned in 

Adopting the system text cursor in custom text views

## Discussion

Use this property to add the view that displays the trailing glow to the view hierarchy. The system calls the closure when it needs to display the glow effect view.

During dictation the indicator displays a glow effect above the text view and below the insertion indicator. It’s the closure’s responsibility to add the glow effect view to the view hierarchy.

## See Also

### Configuring indicators

var color: NSColor!

The color of this indicator.

