

- AppKit
- NSPrinter
-  NSPrinter.TypeName 

Structure

# NSPrinter.TypeName

The type you use to describe a printer’s make and model.

macOS

``` source
struct TypeName
```

## Topics

### Initializers

init(String)

Creates a printer type name.

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting General Printer Information

class var printerNames: [String]

Returns the names of all available printers.

class var printerTypes: [NSPrinter.TypeName]

Returns descriptions of the makes and models of all available printers.

