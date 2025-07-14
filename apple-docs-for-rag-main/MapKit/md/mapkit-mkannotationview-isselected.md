

- MapKit
- MKAnnotationView
-  isSelected 

Instance Property

# isSelected

A Boolean value that indicates whether the annotation view is in a selected state.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
var isSelected: Bool { get set }
```

## Discussion

Don’t set the value of this property directly. If the property contains true, the annotation view is displaying a callout.

## See Also

### Managing the selection state

func setSelected(Bool, animated: Bool)

Sets the selection state of the annotation view.

