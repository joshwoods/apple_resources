

- ImageCaptureCore
- ICScannerDevice
-  availableFunctionalUnitTypes 

Instance Property

# availableFunctionalUnitTypes

An array of functional unit types available on this scanner.

macOS 10.4+

``` source
var availableFunctionalUnitTypes: [NSNumber] { get }
```

## Discussion

This array contains NSNumber objects whose values are of type ICScannerFunctionalUnitType.

## See Also

### Selecting a Functional Unit

var selectedFunctionalUnit: ICScannerFunctionalUnit

The currently selected functional unit on the scanner.

func requestSelect(ICScannerFunctionalUnitType)

Requests to select a functional unit on the scanner.

enum ICScannerFunctionalUnitType

The types of scanner functional units.

enum ICScannerFunctionalUnitState

Flags to indicate the state of the scanner functional unit.

