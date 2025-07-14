

- ImageCaptureCore
-  ICScannerFunctionalUnitType 

Enumeration

# ICScannerFunctionalUnitType

The types of scanner functional units.

macOS 10.4+

``` source
enum ICScannerFunctionalUnitType
```

## Topics

### Constants

case documentFeeder

A document feeder functional unit.

case flatbed

A flatbed functional unit.

case negativeTransparency

A transparency functional unit for scanning negatives.

case positiveTransparency

A transparency functional unit for scanning positives.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Selecting a Functional Unit

var availableFunctionalUnitTypes: [NSNumber]

An array of functional unit types available on this scanner.

var selectedFunctionalUnit: ICScannerFunctionalUnit

The currently selected functional unit on the scanner.

func requestSelect(ICScannerFunctionalUnitType)

Requests to select a functional unit on the scanner.

enum ICScannerFunctionalUnitState

Flags to indicate the state of the scanner functional unit.

