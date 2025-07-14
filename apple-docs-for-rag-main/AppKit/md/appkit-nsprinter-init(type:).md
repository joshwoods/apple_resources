

- AppKit
- NSPrinter
-  init(type:) 

Initializer

# init(type:)

Creates and returns a printer object initialized to the first available printer with the specified make and model information.

macOS

``` source
init?(type: NSPrinter.TypeName)
```

## Parameters 

`type`  

A string describing the make and model information. You can get this string using the printerTypes method.

## Return Value

An initialized `NSPrinter` object, or `nil` if the specified printer was not available.

## See Also

### Related Documentation

var type: NSPrinter.TypeName

A description of the printer’s make and model.

### Creating the Printer Object

init?(name: String)

Creates and returns a printer object initialized with the specified printer name.

