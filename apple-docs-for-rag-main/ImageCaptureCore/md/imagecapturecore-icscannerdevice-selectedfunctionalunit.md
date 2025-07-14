

- ImageCaptureCore
- ICScannerDevice
-  selectedFunctionalUnit 

Instance Property

# selectedFunctionalUnit

The currently selected functional unit on the scanner.

macOS 10.4+

``` source
var selectedFunctionalUnit: ICScannerFunctionalUnit { get }
```

## See Also

### Selecting a Functional Unit

var availableFunctionalUnitTypes: [NSNumber]

An array of functional unit types available on this scanner.

func requestSelect(ICScannerFunctionalUnitType)

Requests to select a functional unit on the scanner.

enum ICScannerFunctionalUnitType

The types of scanner functional units.

enum ICScannerFunctionalUnitState

Flags to indicate the state of the scanner functional unit.

