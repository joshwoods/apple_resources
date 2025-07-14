

- ImageCaptureCore
-  ICScannerFunctionalUnitState 

Enumeration

# ICScannerFunctionalUnitState

Flags to indicate the state of the scanner functional unit.

macOS 10.4+

``` source
enum ICScannerFunctionalUnitState
```

## Topics

### Constants

case ready

A flag indicating that the functional unit is ready for operation.

case overviewScanInProgress

A flag indicating that the functional unit is performing an overview scan.

case scanInProgress

A flag indicating that the functional unit is performing a scan.

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

enum ICScannerFunctionalUnitType

The types of scanner functional units.

