

- AppKit
- NSRulerView
-  measurementUnits 

Instance Property

# measurementUnits

The measurement units used by the ruler to `unitName`.

macOS

``` source
@MainActor
var measurementUnits: NSRulerView.UnitName { get set }
```

## Discussion

`unitName` must have been registered with the NSRulerView class object prior to invoking this method. See the description of the class method registerUnit(withName:abbreviation:unitToPointsConversionFactor:stepUpCycle:stepDownCycle:) for a list of predefined units.

## See Also

### Altering measurement units

class func registerUnit(withName: NSRulerView.UnitName, abbreviation: String, unitToPointsConversionFactor: CGFloat, stepUpCycle: [NSNumber], stepDownCycle: [NSNumber])

Registers a new unit of measurement with the NSRulerView class, making it available to all instances of NSRulerView.

struct UnitName

