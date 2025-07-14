

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:shouldShowNotificationFor:) 

Instance Method

# mapTemplate(\_:shouldShowNotificationFor:)

Asks the delegate whether the system should display the maneuver as a notification when the app is in the background.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    shouldShowNotificationFor maneuver: CPManeuver
) -> Bool
```

## Parameters 

`mapTemplate`  

The current map template.

`maneuver`  

The current maneuver.

## Return Value

true if the system should display the maneuver as a notification; otherwise, false.

## See Also

### Displaying Notifications

func mapTemplate(CPMapTemplate, shouldUpdateNotificationFor: CPManeuver, with: CPTravelEstimates) -> Bool

Asks the delegate whether the system should display the maneuver with updated travel estimates as a notification when the app is in the background.

func mapTemplate(CPMapTemplate, shouldShowNotificationFor: CPNavigationAlert) -> Bool

Asks the delegate whether the system should display the navigation alert as a notification when the app is in the background.

