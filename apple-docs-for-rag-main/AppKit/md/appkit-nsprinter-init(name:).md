

- AppKit
- NSPrinter
-  init(name:) 

Initializer

# init(name:)

Creates and returns a printer object initialized with the specified printer name.

macOS

``` source
init?(name: String)
```

## Parameters 

`name`  

The name of the printer.

## Return Value

An initialized `NSPrinter` object, or `nil` if the specified printer was not available.

## See Also

### Related Documentation

var name: String

The printer’s name.

Printing Programming Guide for Mac

class var printerNames: [String]

Returns the names of all available printers.

### Creating the Printer Object

init?(type: NSPrinter.TypeName)

Creates and returns a printer object initialized to the first available printer with the specified make and model information.

