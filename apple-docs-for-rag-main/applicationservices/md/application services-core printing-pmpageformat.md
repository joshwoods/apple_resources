

- Application Services
- Core Printing
-  PMPageFormat 

Type Alias

# PMPageFormat

An opaque type that stores the settings in the Page Setup dialog.

macOS 10.0+

``` source
typealias PMPageFormat = OpaquePointer
```

## Discussion

Your application uses page format objects to store information such as the paper size, orientation, and scale of pages in a printing session. To create a page format object, you use the function PMCreatePageFormat(_:). A new page format object is empty and unusable until you call PMSessionDefaultPageFormat(_:_:) or PMCopyPageFormat(_:_:) to initialize the settings. You can also use the functions PMSetPageFormatExtendedData(_:_:_:_:) and PMGetPageFormatExtendedData(_:_:_:_:) to store and retrieve application-specific data in a page format object.

