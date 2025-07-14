

- CarPlay
-  CPMapTemplateDelegate 

Protocol

# CPMapTemplateDelegate

The protocol an object implements to handle events from a map template.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
protocol CPMapTemplateDelegate : NSObjectProtocol
```

## Topics

### Setting the Display Style

func mapTemplate(CPMapTemplate, displayStyleFor: CPManeuver) -> CPManeuverDisplayStyle

Asks the delegate for the maneuver’s display style.

struct CPManeuverDisplayStyle

A display style that determines the visual layout for a maneuver.

### Handling Navigation Events

func mapTemplate(CPMapTemplate, selectedPreviewFor: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to preview.

func mapTemplate(CPMapTemplate, startedTrip: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to navigate.

func mapTemplateDidCancelNavigation(CPMapTemplate)

Tells the delegate that the system canceled the navigation.

func mapTemplateShouldProvideNavigationMetadata(CPMapTemplate) -> Bool

Asks the delegate whether the template should provide navigation metadata

### Displaying Notifications

func mapTemplate(CPMapTemplate, shouldShowNotificationFor: CPManeuver) -> Bool

Asks the delegate whether the system should display the maneuver as a notification when the app is in the background.

func mapTemplate(CPMapTemplate, shouldUpdateNotificationFor: CPManeuver, with: CPTravelEstimates) -> Bool

Asks the delegate whether the system should display the maneuver with updated travel estimates as a notification when the app is in the background.

func mapTemplate(CPMapTemplate, shouldShowNotificationFor: CPNavigationAlert) -> Bool

Asks the delegate whether the system should display the navigation alert as a notification when the app is in the background.

### Handling Navigation Alerts

func mapTemplate(CPMapTemplate, willShow: CPNavigationAlert)

Tells the delegate that the system will show the navigation alert.

func mapTemplate(CPMapTemplate, didShow: CPNavigationAlert)

Tells the delegate that the system showed the navigation alert.

func mapTemplate(CPMapTemplate, willDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system is preparing to dismiss the navigation alert.

func mapTemplate(CPMapTemplate, didDismiss: CPNavigationAlert, dismissalContext: CPNavigationAlert.DismissalContext)

Tells the delegate that the system dismissed the navigation alert.

enum DismissalContext

A set of reasons for dismissing a navigation alert.

### Panning the Map

func mapTemplateDidShowPanningInterface(CPMapTemplate)

Tells the delegate that the panning interface is visible on the map.

func mapTemplateWillDismissPanningInterface(CPMapTemplate)

Tells the delegate that the panning interface will disappear from the map.

func mapTemplateDidDismissPanningInterface(CPMapTemplate)

Tells the delegate that the panning interface is no longer visible on the map.

func mapTemplateDidBeginPanGesture(CPMapTemplate)

Tells the delegate that the pan gesture has started.

func mapTemplate(CPMapTemplate, panBeganWith: CPMapTemplate.PanDirection)

Tells the delegate that the user is starting to pan the map.

func mapTemplate(CPMapTemplate, panWith: CPMapTemplate.PanDirection)

Tells the delegate that the user is panning in a certain direction on the map.

func mapTemplate(CPMapTemplate, panEndedWith: CPMapTemplate.PanDirection)

Tells the delegate that the user stopped panning the map.

struct PanDirection

The directions a user can pan (or move) a map displayed on the CarPlay screen.

func mapTemplate(CPMapTemplate, didEndPanGestureWithVelocity: CGPoint)

Tells the delegate that the pan gesture ended with the specified velocity.

func mapTemplate(CPMapTemplate, didUpdatePanGestureWithTranslation: CGPoint, velocity: CGPoint)

Tells the delegate that the pan gesture changed.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Handling Map Template Events

var mapDelegate: (any CPMapTemplateDelegate)?

The object that serves as the delegate of the map template.

