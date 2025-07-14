

- AppKit
- NSRulerView
-  NSRulerView.UnitName 

Structure

# NSRulerView.UnitName

macOS

``` source
struct UnitName
```

## Topics

### Ruler Units

static let centimeters: NSRulerView.UnitName

static let inches: NSRulerView.UnitName

static let picas: NSRulerView.UnitName

static let points: NSRulerView.UnitName

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Altering measurement units

class func registerUnit(withName: NSRulerView.UnitName, abbreviation: String, unitToPointsConversionFactor: CGFloat, stepUpCycle: [NSNumber], stepDownCycle: [NSNumber])

Registers a new unit of measurement with the NSRulerView class, making it available to all instances of NSRulerView.

var measurementUnits: NSRulerView.UnitName

The measurement units used by the ruler to `unitName`.

