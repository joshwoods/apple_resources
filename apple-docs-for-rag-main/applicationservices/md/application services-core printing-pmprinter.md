

- Application Services
- Core Printing
-  PMPrinter 

Type Alias

# PMPrinter

An opaque type that represents a printer.

macOS 10.0+

``` source
typealias PMPrinter = OpaquePointer
```

## Discussion

You typically obtain a printer object using the function PMSessionGetCurrentPrinter(_:_:) or PMServerCreatePrinterList(_:_:).

