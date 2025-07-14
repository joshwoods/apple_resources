

- CarPlay
- CPMapTemplate
-  hideTripPreviews() 

Instance Method

# hideTripPreviews()

Hides the display of trip previews.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
func hideTripPreviews()
```

## See Also

### Displaying Trip Previews

func showTripPreviews([CPTrip], textConfiguration: CPTripPreviewTextConfiguration?)

Displays the preview for one or more trips, and allows route selection.

func showTripPreviews([CPTrip], selectedTrip: CPTrip?, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the previews for a collection of trips, with a single selected trip.

func showRouteChoicesPreview(for: CPTrip, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the route choices for a single trip.

class CPTripPreviewTextConfiguration

A configuration object for changing the button titles on a trip preview.

