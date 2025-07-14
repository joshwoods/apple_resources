

- CarPlay
- CPMapTemplate
-  showTripPreviews(\_:textConfiguration:) 

Instance Method

# showTripPreviews(\_:textConfiguration:)

Displays the preview for one or more trips, and allows route selection.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func showTripPreviews(
    _ tripPreviews: [CPTrip],
    textConfiguration: CPTripPreviewTextConfiguration?
)
```

## Parameters 

`tripPreviews`  

A list of trips to preview, limited to 12 trips.

`textConfiguration`  

A text configuration object containing the titles to display on trip preview buttons.

## Discussion

Use this method to display upcoming trips or multiple trip options, such as for search results. Trip previews can appear over the active navigation session.

## See Also

### Displaying Trip Previews

func showTripPreviews([CPTrip], selectedTrip: CPTrip?, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the previews for a collection of trips, with a single selected trip.

func hideTripPreviews()

Hides the display of trip previews.

func showRouteChoicesPreview(for: CPTrip, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the route choices for a single trip.

class CPTripPreviewTextConfiguration

A configuration object for changing the button titles on a trip preview.

