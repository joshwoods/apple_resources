

- CarPlay
- CPLane
-  secondaryAngles Deprecated

Instance Property

# secondaryAngles

A list of the remaining angles of this lane guidance.

iOS 17.4–18.0DeprecatediPadOS 17.4–18.0DeprecatedMac Catalyst 17.4–18.0Deprecated

``` source
var secondaryAngles: [Measurement] { get set }
```

Deprecated

Use angles to get value, Use -\[CPLane initWithAngles:\] or -\[CPLane initAngles:highlightedAngle:isPreferred:\] to create a CPLane with angles

### Discussion

This doesn’t include the `primaryAngle`.

## See Also

### Properties

var primaryAngle: Measurement&lt;UnitAngle>

A value that represents the angle the framework highlights if this lane is preferred or good.

Deprecated

var status: CPLaneStatus

A value that describes the lane’s status.

