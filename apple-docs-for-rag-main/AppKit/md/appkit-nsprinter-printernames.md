

- AppKit
- NSPrinter
-  printerNames 

Type Property

# printerNames

Returns the names of all available printers.

macOS

``` source
class var printerNames: [String] { get }
```

## Return Value

An array of `NSString` objects, each of which contains the name of an available printer.

## Discussion

The user constructs the list of available printers when adding a printer in the Print panel or setting up printers in the Print & Scan preferences pane.

## See Also

### Related Documentation

var name: String

The printer’s name.

### Getting General Printer Information

class var printerTypes: [NSPrinter.TypeName]

Returns descriptions of the makes and models of all available printers.

struct TypeName

The type you use to describe a printer’s make and model.

