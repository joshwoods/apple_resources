

- HealthKitUI
-  HKActivityRingView 

Class

# HKActivityRingView

A view that uses the Move, Exercise, and Stand activity rings to display data from a HealthKit activity summary object.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
class HKActivityRingView
```

## Mentioned in 

Executing Activity Summary Queries

## Overview

Use HKActivityRingView to display data from an HKActivitySummary object. For example, Figure 1 shows how the rings can display a summary view of the user’s activity.

The activity ring view always appears as a black rectangle with red, green, and blue concentric rings. The rings are centered in the view and are sized to fit the available space (see Figure 2).

The rings have two different ways to display a lack of data. One indicates that the activity summary is missing, and the other indicates that the activity summary’s values are set to zero. If the ring has a `nil`-valued `activitySummary` property, the rings appear empty. Use this to indicate that there is no summary data available for the specified day (for example, dates in the future).

If the summary has zero-valued quantities set for its value properties, the ring displays a dot at the top of the ring. Use this to indicate that the user has not yet burned any active calories, exercised, or earned any stand hours for the specified day.

To display activity summary data from the HealthKit store, use an HKActivitySummaryQuery object. You can also instantiate and display your own HKActivitySummary objects, as needed.

To display data for a ring, the HKActivitySummary object must have a non-`nil` quantity for both the corresponding value property and the goal property (see \

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

### Setting the activity summary

var activitySummary: HKActivitySummary?

The active summary displayed by the activity ring view.

func setActivitySummary(HKActivitySummary?, animated: Bool)

Sets the activity summary displayed by the activity ring view.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Essentials

HealthKit

Access and share health and fitness data while maintaining the user’s privacy and control.

