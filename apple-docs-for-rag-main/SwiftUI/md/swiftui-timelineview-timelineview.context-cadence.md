

- SwiftUI
- TimelineView
- TimelineView.Context
-  cadence 

Instance Property

# cadence

The rate at which the timeline updates the view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let cadence: TimelineView.Context.Cadence
```

## Discussion

Use this value to hide information that updates faster than the view’s current update rate. For example, you could hide the millisecond component of a digital timer when the cadence is anything slower than TimelineView.Context.Cadence.live.

Because the TimelineView.Context.Cadence enumeration conforms to the Comparable protocol, you can compare cadences with relational operators. Slower cadences have higher values, so you could perform the check described above with the following comparison:

```
let hideMilliseconds = cadence > .live
```

## See Also

### Getting the cadence

enum Cadence

A rate at which timeline views can receive updates.

