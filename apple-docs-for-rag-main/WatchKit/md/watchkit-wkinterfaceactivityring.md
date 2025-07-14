

- WatchKit
-  WKInterfaceActivityRing 

Class

# WKInterfaceActivityRing

A view that displays data from a HealthKit activity summary object.

watchOS 2.2+

``` source
class WKInterfaceActivityRing
```

## Overview

The WKInterfaceActivityRing view displays data from an HKActivitySummary object, using the Move, Exercise, and Stand activity rings (see Figure 1).

The activity ring view always appears as a black rectangle with red, green, and blue concentric rings. The rings are centered in the view, and sized to fit the available space (see Figure 2).

The rings have two different ways to display a lack of data. One indicates that the activity summary is missing, and the other indicates that the activity summary’s values are set to zero. If the ring has a `nil`-valued `activitySummary` property, the rings appear empty (see See Figure 3). Use this to indicate that there is no summary data available for the specified day (for example, dates in the future).

If the summary has zero-valued quantities set for its value properties, the ring displays a dot at the top of the ring (see Figure 4). Use this to indicate that the user has not yet burned any active calories, exercised, or earned any stand hours for the specified day.

To display activity summary data from the HealthKit store, use an HKActivitySummaryQuery object. You can also instantiate and display your own HKActivitySummary objects, as needed.

To display data for a ring, the HKActivitySummary object must have a non-`nil` quantity for both the corresponding value property and goal property (see the following table).

| Ring | Value property | Goal property |
|----|----|----|
| Move | activeEnergyBurned | activeEnergyBurnedGoal |
| Exercise | appleExerciseTime | appleExerciseTimeGoal |
| Stand | appleStandHours | appleStandHoursGoal |

The activity ring view colors a percentage of each ring based on these properties, as shown here:

```
ring percent = value property quantity / goal property quantity
```

## Topics

### Setting the Activity Summary

func setActivitySummary(HKActivitySummary?, animated: Bool)

Sets the activity summary displayed by the activity ring view.

### Initializing for SwiftUI

init()

Creates an activity ring view for use in SwiftUI.

## Relationships

### Inherits From

- WKInterfaceObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Controls

class WKInterfaceLabel

An interface element that displays static text.

class WKInterfaceDate

A label that displays the current date or time.

class WKInterfaceTimer

A label that displays a countdown or count-up timer.

class WKInterfaceButton

A button in the user interface of your watchOS app.

class WKInterfaceAuthorizationAppleIDButton

A button that you can use to trigger a Sign in with Apple request.

class WKInterfacePaymentButton

A button that you can use to trigger payments through Apple Pay.

class WKInterfaceTextField

An interface element that displays an editable text area.

class WKInterfaceSwitch

An interface element that toggles between an On and Off state.

class WKInterfaceSlider

An interface element that lets users select a single floating-point value from a range of values.

class WKInterfaceMap

An interface element that displays a noninteractive map for the location you specify.

