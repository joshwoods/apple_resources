

- Application Services
- Core Printing
-  PMObject 

Type Alias

# PMObject

The base type for all the opaque types used in Core Printing.

macOS 10.0+

``` source
typealias PMObject = UnsafeRawPointer
```

## Discussion

`PMObject` is the base type for opaque types such as `PMPrintSession`, `PMPageFormat`, `PMPrintSettings`, `PMPrinter`, `PMPaper`, `PMPreset`, and `PMServer`. `PMObject` is used in functions such as PMRetain(_:) and PMRelease(_:) that operate on any opaque type.

