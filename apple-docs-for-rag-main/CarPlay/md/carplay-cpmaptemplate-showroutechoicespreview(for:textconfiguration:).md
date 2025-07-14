

- CarPlay
- CPMapTemplate
-  showRouteChoicesPreview(for:textConfiguration:) 

Instance Method

# showRouteChoicesPreview(for:textConfiguration:)

Displays the route choices for a single trip.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func showRouteChoicesPreview(
    for tripPreview: CPTrip,
    textConfiguration: CPTripPreviewTextConfiguration?
)
```

## Parameters 

`tripPreview`  

The trip to preview.

`textConfiguration`  

A text configuration object containing the titles to display on trip preview buttons.

## Discussion

The trip preview can appear over an active navigation session.

## See Also

### Displaying Trip Previews

func showTripPreviews([CPTrip], textConfiguration: CPTripPreviewTextConfiguration?)

Displays the preview for one or more trips, and allows route selection.

func showTripPreviews([CPTrip], selectedTrip: CPTrip?, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the previews for a collection of trips, with a single selected trip.

func hideTripPreviews()

Hides the display of trip previews.

class CPTripPreviewTextConfiguration

A configuration object for changing the button titles on a trip preview.

