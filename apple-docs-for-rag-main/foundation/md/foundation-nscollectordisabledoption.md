

- Foundation
-  NSCollectorDisabledOption 

Global Variable

# NSCollectorDisabledOption

Specifies that the block is retained, and therefore ineligible for collection. Specifying this option is equivalent to invoking disableCollectorForPointer: with the returned block as the argument.

macOS 10.0+

``` source
var NSCollectorDisabledOption: Int { get }
```

## See Also

### Constants

var NSScannedOption: Int

Specifies allocation of scanned memory.

