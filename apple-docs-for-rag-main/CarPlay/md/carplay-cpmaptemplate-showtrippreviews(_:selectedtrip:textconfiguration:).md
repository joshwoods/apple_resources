

- CarPlay
- CPMapTemplate
-  showTripPreviews(\_:selectedTrip:textConfiguration:) 

Instance Method

# showTripPreviews(\_:selectedTrip:textConfiguration:)

Displays the previews for a collection of trips, with a single selected trip.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func showTripPreviews(
    _ tripPreviews: [CPTrip],
    selectedTrip: CPTrip?,
    textConfiguration: CPTripPreviewTextConfiguration?
)
```

## Parameters 

`tripPreviews`  

An array of trips to preview.

`selectedTrip`  

The trip to select when CarPlay presents the list of trip previews.

`textConfiguration`  

A configuration object that contains the various titles a trip preview button can display.

## Discussion

Use this method to display upcoming trips or multiple trip options, such as search results. Trip previews can appear over an active navigation session. Provide an array of up to twelve CPTrip objects to preview. If the array contains more objects, CarPlay displays only the first twelve.

The trip you want to select must be a member of the `tripPreviews` array.

## See Also

### Displaying Trip Previews

func showTripPreviews([CPTrip], textConfiguration: CPTripPreviewTextConfiguration?)

Displays the preview for one or more trips, and allows route selection.

func hideTripPreviews()

Hides the display of trip previews.

func showRouteChoicesPreview(for: CPTrip, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the route choices for a single trip.

class CPTripPreviewTextConfiguration

A configuration object for changing the button titles on a trip preview.

