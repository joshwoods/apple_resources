

- MapKit
- MKAnnotationView
-  setSelected(\_:animated:) 

Instance Method

# setSelected(\_:animated:)

Sets the selection state of the annotation view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
@MainActor
func setSelected(
    _ selected: Bool,
    animated: Bool
)
```

## Parameters 

`selected`  

Contains the value true if the view displays in a selected state.

`animated`  

Set to true if the map view animates the change in selection state.

## Discussion

Dont call this method directly. An MKMapView object calls this method in response to user interactions with the annotation.

## See Also

### Related Documentation

func selectAnnotation(any MKAnnotation, animated: Bool)

Selects the specified annotation and displays a callout view for it.

### Managing the selection state

var isSelected: Bool

A Boolean value that indicates whether the annotation view is in a selected state.

