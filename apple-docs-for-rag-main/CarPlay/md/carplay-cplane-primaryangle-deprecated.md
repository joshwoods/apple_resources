

- CarPlay
- CPLane
-  primaryAngle Deprecated

Instance Property

# primaryAngle

A value that represents the angle the framework highlights if this lane is preferred or good.

iOS 17.4–18.0DeprecatediPadOS 17.4–18.0DeprecatedMac Catalyst 17.4–18.0Deprecated

``` source
var primaryAngle: Measurement { get set }
```

Deprecated

Use highlightedAngle to get value, use -\[CPLane initAngles:highlightedAngle:isPreferred:\] to create a CPLane with highlightedAngle set

## Discussion

If `primaryAngle` is present it can’t be included in secondaryAngles.

## See Also

### Properties

var secondaryAngles: [Measurement&lt;UnitAngle>]

A list of the remaining angles of this lane guidance.

Deprecated

var status: CPLaneStatus

A value that describes the lane’s status.

