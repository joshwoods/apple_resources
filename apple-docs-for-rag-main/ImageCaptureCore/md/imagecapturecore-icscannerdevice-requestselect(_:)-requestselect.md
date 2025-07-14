

- ImageCaptureCore
- ICScannerDevice
-  requestSelect(\_:) 

Instance Method

# requestSelect(\_:)

Requests to select a functional unit on the scanner.

macOS 10.4+

``` source
func requestSelect(_ type: ICScannerFunctionalUnitType)
```

## Discussion

When the request has completed, scannerDevice(_:didSelect:error:) is called on the delegate.

## See Also

### Selecting a Functional Unit

var availableFunctionalUnitTypes: [NSNumber]

An array of functional unit types available on this scanner.

var selectedFunctionalUnit: ICScannerFunctionalUnit

The currently selected functional unit on the scanner.

enum ICScannerFunctionalUnitType

The types of scanner functional units.

enum ICScannerFunctionalUnitState

Flags to indicate the state of the scanner functional unit.

