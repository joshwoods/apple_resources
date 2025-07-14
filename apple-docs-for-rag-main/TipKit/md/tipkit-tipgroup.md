

- TipKit
-  TipGroup 

Class

# TipGroup

A collection of tips that can be presented one at a time using a specific order or based on the first tip eligible for display.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
final class TipGroup
```

## Overview

Use this class to group multiple tips together and have them presented one at a time. You display tips in a specific order with an ordered priority or display the first tip eligible for display with a firstAvailable priority.

TipGroup has a firstAvailable default priority.

```
struct TrailDetails: View {
    let trail: Trail

    @State
    var trailDetailTips = TipGroup {
        FindTrailheadTip()
        ExposureRatingTip()
        SlopeProfileTip()
    }

    var body: some View {
        ScrollView(.vertical) {
            // Trail title
            Text(trail.name)
                .font(.title)
            NavigateToTrailButton(trailLocation: trail.location)
                .popoverTip(trailDetailTips.currentTip as? FindTrailheadTip)

            // Trail exposure rating
            TipView(trailDetailTips.currentTip as? ExposureRatingTip, arrowEdge: .bottom)
            Text("Exposure Rating: \(trail.exposureRating)")

            // Trail slope angle
            TipView(trailDetailTips.currentTip as? SlopeProfileTip, arrowEdge: .bottom)
            Text("Slope Angle: \(trail.slopeAngle)°")
        }
    }
}
```

## Topics

### Creating a tip group

init(TipGroup.Priority, () -> [any Tip])

Creates a tip group with the specified presentation priority.

### Controlling the display order of a TipGroup’s tips

enum Priority

Order priority for a TipGroup.

### Getting the currently available tip

var currentTip: (any Tip)?

Returns the current tip available for display.

var currentTipUpdates: some AsyncSequence&lt;any Tip, Never>

Stream of tips that become eligible for display.

## Relationships

### Conforms To

- Copyable
- Observable
- Sendable

## See Also

### Content

protocol Tip

A type that sets a tip’s content, as well as the conditions for when it displays.

