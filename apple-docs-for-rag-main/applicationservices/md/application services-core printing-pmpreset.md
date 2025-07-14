

- Application Services
- Core Printing
-  PMPreset 

Type Alias

# PMPreset

An opaque type that stores information about a named preset available for a print job.

macOS 10.3+

``` source
typealias PMPreset = OpaquePointer
```

## Discussion

Your application uses a preset object to identify a named preset in the Print dialog. You typically obtain an instance of this type using the function PMPrinterCopyPresets(_:_:).

