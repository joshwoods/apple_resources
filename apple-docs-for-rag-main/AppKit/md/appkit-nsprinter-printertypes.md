

- AppKit
- NSPrinter
-  printerTypes 

Type Property

# printerTypes

Returns descriptions of the makes and models of all available printers.

macOS

``` source
class var printerTypes: [NSPrinter.TypeName] { get }
```

## Return Value

An array of `NSString` objects, each of which contains the make and model information for a supported printer.

## See Also

### Related Documentation

var type: NSPrinter.TypeName

A description of the printer’s make and model.

### Getting General Printer Information

class var printerNames: [String]

Returns the names of all available printers.

struct TypeName

The type you use to describe a printer’s make and model.

