

- AdAttributionKit
- PostbackUpdate
-  init(fineConversionValue:lockPostback:coarseConversionValue:conversionTypes:) 

Initializer

# init(fineConversionValue:lockPostback:coarseConversionValue:conversionTypes:)

Creates a new postback update with the conversions values, conversion types, and lock indication you provide.

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
init(
    fineConversionValue: Int,
    lockPostback: Bool,
    coarseConversionValue: CoarseConversionValue? = nil,
    conversionTypes: [PostbackUpdate.ConversionType]? = nil
)
```

## Parameters 

`fineConversionValue`  

An integer that represents the fine conversion value.

`lockPostback`  

A Boolean value that indicates whether the system can lock the postback, reducing the system time to deliver a signal.

`coarseConversionValue`  

An optional `CoarseConversionValue` enumeration value that represents the coarse conversion value. Defaults to `nil`.

`conversionTypes`  

An optional array of conversion types the system uses to determine which postbacks to update. Defaults to `nil` and the system updates all types of postbacks by default.

