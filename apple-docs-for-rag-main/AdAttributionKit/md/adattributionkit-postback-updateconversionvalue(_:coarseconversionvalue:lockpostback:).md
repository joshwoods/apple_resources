

- AdAttributionKit
- Postback
-  updateConversionValue(\_:coarseConversionValue:lockPostback:) 

Type Method

# updateConversionValue(\_:coarseConversionValue:lockPostback:)

Updates the conversion value with the provided fine and coarse conversion values, and optionally locks the postback, reducing the amount of time the system needs to deliver a signal.

iOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
static func updateConversionValue(
    _ fineConversionValue: Int,
    coarseConversionValue: CoarseConversionValue,
    lockPostback: Bool
) async throws
```

## Parameters 

`fineConversionValue`  

An integer that defines the fine conversion value.

`coarseConversionValue`  

One of the CoarseConversionValue values.

`lockPostback`  

A Boolean value that indicates whether the system can lock the postback, reducing system time to deliver a signal.

## Mentioned in 

Receiving postbacks in multiple conversion windows

Receiving ad attributions and postbacks

Understanding AdAttributionKit and SKAdNetwork interoperability

Identifying the parameters in a postback

Configuring an advertised app

