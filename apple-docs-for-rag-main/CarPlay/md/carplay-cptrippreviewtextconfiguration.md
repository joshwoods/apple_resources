

- CarPlay
-  CPTripPreviewTextConfiguration 

Class

# CPTripPreviewTextConfiguration

A configuration object for changing the button titles on a trip preview.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPTripPreviewTextConfiguration
```

## Topics

### Creating a Text Configuration Object

init(startButtonTitle: String?, additionalRoutesButtonTitle: String?, overviewButtonTitle: String?)

Creates a trip preview text configuration object.

### Setting Button Titles

var startButtonTitle: String?

The title displayed on the start button.

var additionalRoutesButtonTitle: String?

The title displayed on the routes button.

var overviewButtonTitle: String?

The title displayed on the overview button.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Displaying Trip Previews

func showTripPreviews([CPTrip], textConfiguration: CPTripPreviewTextConfiguration?)

Displays the preview for one or more trips, and allows route selection.

func showTripPreviews([CPTrip], selectedTrip: CPTrip?, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the previews for a collection of trips, with a single selected trip.

func hideTripPreviews()

Hides the display of trip previews.

func showRouteChoicesPreview(for: CPTrip, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the route choices for a single trip.

