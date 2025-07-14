

- CarPlay
-  CPMapTemplate 

Class

# CPMapTemplate

A template that displays a navigation overlay that your app draws on the map.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CPMapTemplate
```

## Overview

After CarPlay calls your scene delegate’s templateApplicationScene(_:didConnect:to:) method, create a map template and set it as the root template by calling setRootTemplate(_:animated:completion:) on the interface controller the method provides.

The map template appears as an overlay on top of the base view. The template is the control layer, providing a navigation bar and map buttons that users interact with through the CarPlay screen.

Note

The base view is where your app draws its map. CarPlay doesn’t support direct user interactions in this view. Instead, your app uses templates, which overlay the base view, to allow users to interact with your app through the CarPlay screen.

When the user begins to interact with your app through the CarPlay screen, the system displays the navigation bar, hiding it after a brief period of inactivity. You can change this behavior by setting the automaticallyHidesNavigationBar and hidesButtonsWithNavigationBar properties.

The navigation bar includes up to two leading and two trailing buttons. You can change the buttons, including their titles and icon images, by setting the leadingNavigationBarButtons and trailingNavigationBarButtons properties on your template.

You can display additional map buttons by providing an array of CPMapButton objects to mapButtons. Use these buttons to provide users access to actions, such as entering panning mode or zooming in and out on the map.

## Topics

### Configuring Map Templates

var automaticallyHidesNavigationBar: Bool

A Boolean value that indicates whether the template should automatically hide the navigation bar.

var hidesButtonsWithNavigationBar: Bool

A Boolean value that tells the system to hide the map buttons when hiding the navigation bar.

var guidanceBackgroundColor: UIColor

The background color the map template uses when displaying guidance.

### Handling Map Template Events

var mapDelegate: (any CPMapTemplateDelegate)?

The object that serves as the delegate of the map template.

protocol CPMapTemplateDelegate

The protocol an object implements to handle events from a map template.

### Managing Map Buttons

var mapButtons: [CPMapButton]

An array of map buttons on the trailing bottom corner of the map template.

class CPMapButton

A button that represents an action that a map template displays on the CarPlay screen.

### Displaying Trip Previews

func showTripPreviews([CPTrip], textConfiguration: CPTripPreviewTextConfiguration?)

Displays the preview for one or more trips, and allows route selection.

func showTripPreviews([CPTrip], selectedTrip: CPTrip?, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the previews for a collection of trips, with a single selected trip.

func hideTripPreviews()

Hides the display of trip previews.

func showRouteChoicesPreview(for: CPTrip, textConfiguration: CPTripPreviewTextConfiguration?)

Displays the route choices for a single trip.

class CPTripPreviewTextConfiguration

A configuration object for changing the button titles on a trip preview.

### Navigating a Trip

func startNavigationSession(for: CPTrip) -> CPNavigationSession

Begins navigational guidance for a trip.

class CPNavigationSession

An object that represents an active route guidance session.

### Providing Trip Estimates

func updateEstimates(CPTravelEstimates, for: CPTrip)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip.

func update(CPTravelEstimates, for: CPTrip, with: CPTimeRemainingColor)

Updates travel estimates, such as arrival time and the remaining time and distance for a trip, with the specified time-remaining color.

enum CPTimeRemainingColor

The color the system uses when displaying the time remaining for a trip.

var tripEstimateStyle: CPTripEstimateStyle

The style that the map template uses when displaying trip estimates during active nagivation.

enum CPTripEstimateStyle

The set of display styles for trip estimates.

### Displaying a Navigation Alert

func present(navigationAlert: CPNavigationAlert, animated: Bool)

Displays a navigation alert on the map template.

func dismissNavigationAlert(animated: Bool, completion: (Bool) -> Void)

Tells the map template to dismiss the visable navigation alert.

var currentNavigationAlert: CPNavigationAlert?

The visible navigation alert.

class CPNavigationAlert

An alert that displays map- or navigation-related information to the user.

### Panning the Map

func showPanningInterface(animated: Bool)

Shows the panning interface on the map.

func dismissPanningInterface(animated: Bool)

Dismisses the panning interface.

var isPanningInterfaceVisible: Bool

A Boolean value that indicates whether the map template is displaying the panning interface.

## Relationships

### Inherits From

- CPTemplate

### Conforms To

- CPBarButtonProviding
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Navigation

Integrating CarPlay with Your Navigation App

Configure your navigation app to work with CarPlay by displaying your custom map and directions.

class CPTemplateApplicationDashboardScene

A CarPlay scene that controls your app’s dashboard navigation window.

protocol CPTemplateApplicationDashboardSceneDelegate

The methods for responding to the life-cycle events of your navigation app’s dashboard scene.

class CPSearchTemplate

A template that provides the ability to search for a destination and see a list of search results.

class CPVoiceControlTemplate

A template that displays a voice control indicator during audio input.

