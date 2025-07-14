

- AdAttributionKit
- PostbackUpdate
-  conversionTypes 

Instance Property

# conversionTypes

An array conversion type the system uses to determine which postbacks to update with this postback update.

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
let conversionTypes: [PostbackUpdate.ConversionType]?
```

## Discussion

If `nil`, the system updates all types of postbacks by default.

