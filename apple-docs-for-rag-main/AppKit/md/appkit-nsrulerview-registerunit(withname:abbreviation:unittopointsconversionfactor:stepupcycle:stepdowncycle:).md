

- AppKit
- NSRulerView
-  registerUnit(withName:abbreviation:unitToPointsConversionFactor:stepUpCycle:stepDownCycle:) 

Type Method

# registerUnit(withName:abbreviation:unitToPointsConversionFactor:stepUpCycle:stepDownCycle:)

Registers a new unit of measurement with the NSRulerView class, making it available to all instances of NSRulerView.

macOS

``` source
@MainActor
class func registerUnit(
    withName unitName: NSRulerView.UnitName,
    abbreviation: String,
    unitToPointsConversionFactor conversionFactor: CGFloat,
    stepUpCycle: [NSNumber],
    stepDownCycle: [NSNumber]
)
```

## Discussion

`unitName` is the name of the unit in English, in plural form and capitalized by convention—“Inches”, for example. The unit name is used as a key to identify the measurement units and so shouldn’t be localized. `abbreviation` is a localized short form of the unit name, such as “in” for Inches. `conversionFactor` is the number of PostScript points in the specified unit; there are 72.0 points per inch, for example. `stepUpCycle` and `stepDownCycle` are arrays of NSNumbers that specify how hash marks are calculated, as explained in Setting Up a Ruler View. All numbers in `stepUpCycle` should be greater than 1.0, those in `stepDownCycle` should be less than 1.0.

NSRulerView supports these units by default:

| Unit Name / Abbreviation | Points/Unit | Step-Up Cycle | Step-Down Cycle |
|--------------------------|-------------|---------------|-----------------|
| Inches / in              | 72.0        | 2.0           | 0.5             |
| Centimeters / cm         | 28.35       | 2.0           | 0.5, 0.2        |
| Points / pt              | 1.0         | 10.0          | 0.5             |
| Picas / pc               | 12.0        | 10.0          | 0.5             |

## See Also

### Altering measurement units

var measurementUnits: NSRulerView.UnitName

The measurement units used by the ruler to `unitName`.

struct UnitName

