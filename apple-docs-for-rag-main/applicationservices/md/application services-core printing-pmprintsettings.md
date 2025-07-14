

- Application Services
- Core Printing
-  PMPrintSettings 

Type Alias

# PMPrintSettings

An opaque type that stores the settings in the Print dialog.

macOS 10.0+

``` source
typealias PMPrintSettings = OpaquePointer
```

## Discussion

Your application uses print settings objects to store information such as the number of copies and the range of pages to print in a printing session. To create a print settings object, you use the function PMCreatePrintSettings(_:). A new print settings object is empty and unusable until you call PMSessionDefaultPrintSettings(_:_:) or PMCopyPrintSettings(_:_:) to initialize the settings. You can also use the functions PMSetPrintSettingsExtendedData and PMGetPrintSettingsExtendedData to store and retrieve application-specific data in a print settings object.

