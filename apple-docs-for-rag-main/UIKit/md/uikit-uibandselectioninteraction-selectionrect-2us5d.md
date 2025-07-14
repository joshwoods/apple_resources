

- UIKit
- UIBandSelectionInteraction
-  selectionRect 

Instance Property

# selectionRect

The selection rectangle for an in-progress interaction.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
var selectionRect: CGRect? { get }
```

## Discussion

The rectangle is in the coordinate system of the view that owns the interaction object. If no interaction is active, the value of this propety is `nil`.

